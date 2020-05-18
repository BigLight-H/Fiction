<template>
	<view class="content">
		<view class="text-area">
			<text class="title">{{title}}</text>
		</view>
		<view class="button-sp-area" id="button-id">
			<button type="primary" plain="true">开启小说之旅</button>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				title: 'Shine Book'
			}
		},
		onLoad() {
			// 获取可视区域高度，减去固定高度
			uni.getSystemInfo({
				success: res => {
					let h = res.windowHeight - uni.upx2px(82);
				}
			});
		},
		methods: {
			
		}
	}
</script>

<style>
	 @font-face {
		font-family: 'iconfont';
		src: url('http://book.tiny-app.top/static/fonts/smt.737bf92.ttf');
	}
	body {
		background-color: #e0e0e0;
	}
	.content {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}

	.text-area {
		display: flex;
		justify-content: center;
	}

	.title {
		color: #8f8f94;
		font-family: iconfont;
		font-size: 100upx;
		margin-top: 300upx;
	}
	
	.button-sp-area {
		width: 100%;
		margin-top: 550upx;
	}
	.button-sp-area button {
		width: 70%;
		font-size: 30rpx;
		line-height: 75rpx;
		height: 75rpx;
		border: 1upx solid;
		border-color: #555555 !important;
		color:#555555 !important;
	}
</style>
