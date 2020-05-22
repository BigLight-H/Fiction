<template>
	<view>
		<view>
			<uni-section title="左侧滑出" type="line"></uni-section>
			<view class="example-body">
				<view class="word-btn draw-cotrol-btn" hover-class="word-btn--hover" :hover-start-time="20" :hover-stay-time="70" @click="show('left')"><text class="word-btn-white">显示Drawer</text></view>
				<uni-drawer :visible="showLeft" mode="left" @close="closeDrawer('left')">
					<!-- #ifndef MP-BAIDU || MP-ALIPAY || MP-TOUTIAO -->
					<uni-list>
						<uni-list-item title="Item1" />
						<uni-list-item title="Item2" />
						<uni-list-item :show-badge="true" title="Item3" badge-text="12" />
					</uni-list>
					<!-- #endif -->
					<!-- #ifdef MP-BAIDU || MP-ALIPAY || MP-TOUTIAO -->
					<view class="uni-list">
						<uni-list-item title="Item1" />
						<uni-list-item title="Item2" />
						<uni-list-item :show-badge="true" title="Item3" badge-text="12" />
					</view>
					<!-- #endif -->
					<view class="close">
						<view class="word-btn" hover-class="word-btn--hover" :hover-start-time="20" :hover-stay-time="70" @click="hide"><text class="word-btn-white">关闭Drawer</text></view>
					</view>
				</uni-drawer>
			</view>
			<uni-section title="右侧滑出" type="line"></uni-section>
			<view class="example-body">
				<view class="word-btn draw-cotrol-btn" hover-class="word-btn--hover" :hover-start-time="20" :hover-stay-time="70" @click="show('right')"><text class="word-btn-white">显示Drawer</text></view>
				<uni-drawer :visible="showRight" mode="right" @close="closeDrawer('right')">
					<!-- #ifndef MP-BAIDU || MP-ALIPAY || MP-TOUTIAO -->
					<uni-list>
						<uni-list-item title="Item1" />
						<uni-list-item title="Item2" />
						<uni-list-item class="last-list-item" :show-badge="true" title="Item3" badge-text="12" />
					</uni-list>
					<!-- #endif -->
					<!-- #ifdef MP-BAIDU || MP-ALIPAY || MP-TOUTIAO -->
					<view class="uni-list">
						<uni-list-item title="Item1" />
						<uni-list-item title="Item2" />
						<uni-list-item class="last-list-item" :show-badge="true" title="Item3" badge-text="12" />
					</view>
					<!-- #endif -->
					<view class="close">
						<view class="word-btn" hover-class="word-btn--hover" :hover-start-time="20" :hover-stay-time="70" @click="hide"><text class="word-btn-white">关闭Drawer</text></view>
					</view>
				</uni-drawer>
			</view>
		</view>
	</view>
</template>

<script>
	import uniDrawer from '../../component/uni-drawer/uni-drawer.vue'
	export default {
		components: {
			uniDrawer
		},
		data() {
			return {
				showRight: false,
				showLeft: false
			}
		},
		methods: {
			show(e) {
				console.log("show", e);
				if (e === 'left') {
					this.showLeft = true
				} else {
					this.showRight = true
				}
			},
			hide() {
				console.log("hide");
				this.showLeft = false
				this.showRight = false
			},
			closeDrawer(e) {
				if (e === 'left') {
					this.showLeft = false
				} else {
					this.showRight = false
				}
			},
			confirm() {}
		},
		onNavigationBarButtonTap(e) {
			this.showRight = !this.showRight
		},
		onBackPress() {
			if (this.showRight || this.showLeft) {
				this.hide()
				return true
			}
		}
	}
</script>

<style>

</style>
