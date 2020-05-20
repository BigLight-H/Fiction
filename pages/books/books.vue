<template>
	<view>
		<search></search>
		<view class='book-text'>关键词为"哈哈"的搜所结果:</view>
		<view class="books-list">
			<view class="books-list-text">
				<view class="list-name text-hidden">我是哈哈哈</view>
				<view class="list-text text-hidden">最新章节</view>
				<view class="list-text text-hidden">作者:最新章节</view>
				<view class="list-text text-hidden">来源:最新章节</view>
			</view>
			<view class="books-list-img">
				<image src="http://www.vipzw.com/files/article/image/41/41902/41902s.jpg" mode=""></image>
			</view>
		</view>
	</view>
</template>

<script>
	import search from "../../component/search.vue"
	export default {
		components: {
		    search
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
	.book-text {
		font-size: 25rpx;
		color: #C8C7CC;
		padding-bottom: 1rem;
		margin-left: 2rem;
		margin-right: 2rem;
	}
	.books-list {
		display: flex;
		margin-left: 2rem;
		margin-right: 2rem;
		padding: .5rem 1rem;
		background: #f7f7f7;
		border-radius: 5px;
		margin-bottom: 1rem;

	}
	.books-list-text {
		width: 70%;
		padding-top: 1rem;
	}
	.books-list-img {
		width: 30%;
	}
	.books-list-img image{
		width: 100%;
		height: 8rem;
	}
	.list-name {
		
	}
	.list-text {
		font-size: 27upx;
		color: #999999;
	}
	.text-hidden {
		text-overflow: -o-ellipsis-lastline;
		overflow: hidden;
		text-overflow: ellipsis;
		display: -webkit-box;
		-webkit-line-clamp: 1;
		line-clamp: 1;
		-webkit-box-orient: vertical;
	}
</style>
