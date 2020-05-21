<template>
	<view>
		<view class="">
			<view class="book-detail-img">
				<image src="http://r.m.kuxiaoshuo.com/cover/aHR0cDovL3FpZGlhbi5xcGljLmNuL3FkYmltZy8zNDk1NzMvMTAxMDg2ODI2NC8xODA=" mode=""></image>
			</view>
			<view class="book-name">诡秘之主</view>
			<view class="book-author">作者:我是作者</view>
			<view class="book-jj">蒸汽与机械的浪潮中，谁能触及非凡？历史和黑暗的迷雾里，又是谁在耳语？我从诡秘中醒来，睁眼看见这个世界：枪械，大炮，巨舰，飞空艇，差分机；魔药，占卜，诅咒，倒吊人，封印物……光明依旧照耀，神秘从未远离，这是一段“愚者”的传说。</view>
			<view class="book-btn">
				<button type="default">加入书签</button>
				<button type="default">立即阅读</button>
			</view>
		</view>
		<view class="book-list">
			<view class="book-list-name">全部章节</view>
			<view class="book-lists">
				<view class="book-list-zj">第一张 哈哈哈</view>
				<view class="book-list-zj">第一张 哈哈哈</view>
				<view class="book-list-zj">第一张 哈哈哈</view>
				<view class="book-list-zj">第一张 哈哈哈</view>
				<view class="book-list-zj">第一张 哈哈哈</view>
			
			</view>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			}
		},
		methods: {
			
		}
	}
</script>

<style>
	.book-detail-img {
		text-align: center;
		background: #f3f3f3;
		padding: 1rem;
	}
	.book-detail-img image {
		width: 10rem;
		border-radius: 5px;
	}
	.book-name {
		font-size: 1.2rem;
		margin-left: 2rem;
		margin-right: 2rem;
		padding-top: .5rem;
		border-top: .04rem solid #f3f3f3;
		border-left: .04rem solid #f3f3f3;
		border-right: .04rem solid #f3f3f3;
		border-radius: 5px 5px 0 0;
		margin-top: .5rem;
		padding-left: .5rem;
	}
	.book-author {
		margin-left: 2rem;
		margin-right: 2rem;
		margin-bottom: .5rem;
		padding-bottom: .5rem;
		border-left: .04rem solid #f3f3f3;
		border-right: .04rem solid #f3f3f3;
		border-bottom: .04rem solid #f3f3f3;
		color: #999999;
		border-radius: 0 0 5px 5px;
		padding-left: .5rem;
	}
	.book-jj {
		margin-left: 2rem;
		margin-right: 2rem;
		color: #999999;
		border-radius: 5px;
		padding: .5rem;
		border: .04rem solid #f3f3f3;
		margin-bottom: 1rem;
	}
	.book-btn {
		display: flex;
	}
	.book-btn button:first-child {
		height: 2rem;
		font-size: .5rem;
		background-color: #2db7f5;
		border-color: #2db7f5;
		color: #FFFFFF;
	}
	.book-btn button:last-child {
		height: 2rem;
		font-size: .5rem;
		background-color: #19be6b;
		border-color: #19be6b;
		color: #FFFFFF;
	}
	.book-list {
		margin-left: 2rem;
		margin-right: 2rem;
		border: .04rem solid #f3f3f3;
		margin-top: 1rem;
		padding: .5rem;
		border-radius: 5px;
	}
	.book-list-name {
		padding: .5rem 0;
	}
	.book-lists {
		font-size: 26upx;
	}
	.book-list-zj {
		padding-top: .5rem;
		padding-bottom: .5rem;
		border-bottom: .04rem dashed #dadada;
		color: #999999;
	}
	.book-list-zj:last-child {
		border-bottom: none;
	}
</style>
