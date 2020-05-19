<template>
	<view class="home-book">
		<search></search>
		<view class="">
			<view class="home-title">
				<view class="home-title-paihang">
					点击排行
				</view>
				<view class="home-title-gengduo">
					更多
				</view>
			</view>
			<view class="home-book-hot">
				<view class="home-book-hot-img">
					<image src="http://r.m.kuxiaoshuo.com/cover/aHR0cDovL3FpZGlhbi5xcGljLmNuL3FkYmltZy8zNDk1NzMvMTAxMDg2ODI2NC8xODA=" mode=""></image>
				</view>
				<view class="home-book-con">
					<view class="home-book-con-name">
						诡秘之主
					</view>
					<view class="home-book-con-author">
						作    者：爱潜水的乌贼
					</view>
					<view class="home-book-con-jj">
						蒸汽与机械的浪潮中，谁能触及非凡？历史和黑暗的迷雾里，又是谁在耳语？我从诡秘中醒来，睁眼看见这个世界：枪械，大炮，巨舰，飞空艇，差分机；魔药，占卜，诅咒，倒吊人，封印物……光明依旧照耀，神秘从未远离，这是一段“愚者”的传说。
					</view>
				</view>
			</view>
		</view>
		<view>
			<view class="book-list">
				<view class="book-list-type">
					【 军事 】
				</view>
				<view class="">
					<view class="book-list-name">伏天氏</view>
					<view class="book-list-author">
						作者:我是小草
					</view>
				</view>
			</view>
		</view>
		<floor :msg="1"></floor>
	</view>
</template>

<script>
	import search from "../../component/search.vue"
	import floor from "../../component/floor.vue"
	export default {
		components: {
		    search,
			floor
		},
		data() {
			return {
			
			}
		},
		methods: {
			
		}
	}
</script>

<style>
	.home-book {
		
	}
	.home-title {
		display: flex;
		justify-content: space-between;
		padding-left: 1rem;
		padding-right: 1rem;
		padding-right: 1rem;
	}
	.home-title-paihang {
		font-size: 35upx;
	}
	.home-title-gengduo {
		color: #0A98D5;
	}
	.home-book-hot {
		padding-left: 1rem;
		padding-right: 1rem;
		padding-top: .5rem;
		padding-bottom: .5rem;
		display: flex;
	}
	.home-book-hot-img {
		width: 40%;
	}
	.home-book-hot-img image{
		width: 100%;
	}
	.home-book-con {
		padding-left: .5rem;
		width: 60%;
		padding-top: .8rem;
	}
	.home-book-con-author {
		padding-bottom: .5rem;
		padding-top: .5rem;
	}
	.home-book-con-name {
		font-size: 35upx;
	}
	.home-book-con-jj {
		text-overflow: -o-ellipsis-lastline;
		overflow: hidden;
		text-overflow: ellipsis;
		display: -webkit-box;
		-webkit-line-clamp: 7;
		line-clamp: 7;
		-webkit-box-orient: vertical;
	}
	.book-list {
		margin-left: 1rem;
		margin-right: 1rem;
		display: flex;
		padding-top: .5rem;
		padding-bottom: .5rem;
		border-bottom: .04rem solid #e8eaec;
	}
	.book-list-type {
		line-height: 3rem;
	}
	.book-list-name {
		font-size: 28upx;
	}
	.book-list-author {
		color: #00000073;
	}
	.book-list:last-child {
		border-bottom: none;
	}
</style>
