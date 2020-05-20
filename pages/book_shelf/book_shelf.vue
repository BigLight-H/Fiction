<template>
	<view>
		<search></search>
		<view class="book-shelf">
			<view class="book-shelf-div">
				<image src="http://r.m.kuxiaoshuo.com/cover/aHR0cDovL2Jvb2tjb3Zlci55dWV3ZW4uY29tL3FkYmltZy8zNDk1NzMvMTAxNDk1MjY0NS8xODA=" mode=""></image>
				<view class="book-name">超神道术</view>
			</view>
			<view class="book-shelf-div">
				<image src="http://r.m.kuxiaoshuo.com/cover/aHR0cDovL2Jvb2tjb3Zlci55dWV3ZW4uY29tL3FkYmltZy8zNDk1NzMvMTAxNDk1MjY0NS8xODA=" mode=""></image>
				<view class="book-name">超神道术</view>
			</view>
			<view class="book-shelf-div">
				<image src="http://r.m.kuxiaoshuo.com/cover/aHR0cDovL2Jvb2tjb3Zlci55dWV3ZW4uY29tL3FkYmltZy8zNDk1NzMvMTAxNDk1MjY0NS8xODA=" mode=""></image>
				<view class="book-name">超神道术</view>
			</view>
			<view class="book-shelf-div">
				<image src="http://r.m.kuxiaoshuo.com/cover/aHR0cDovL2Jvb2tjb3Zlci55dWV3ZW4uY29tL3FkYmltZy8zNDk1NzMvMTAxNDk1MjY0NS8xODA=" mode=""></image>
				<view class="book-name">超神道术</view>
			</view>
			<view class="book-shelf-div">
				<image src="http://r.m.kuxiaoshuo.com/cover/aHR0cDovL2Jvb2tjb3Zlci55dWV3ZW4uY29tL3FkYmltZy8zNDk1NzMvMTAxNDk1MjY0NS8xODA=" mode=""></image>
				<view class="book-name">超神道术</view>
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
	.book-shelf {
		display: flex;
		flex-wrap:wrap;
		margin-left: 2rem;
		margin-right: 2rem;
	}
	.book-shelf-div {
		width: 26%;
		margin-left: 5.5%;
		margin-bottom: .5rem;
	}
	.book-shelf-div image {
		width: 100%;
		height: 8rem;
		border-radius: 5px;
	}
	.book-name {
		text-align: center;
		font-size: 25rpx;
		text-overflow: -o-ellipsis-lastline;
		overflow: hidden;
		text-overflow: ellipsis;
		display: -webkit-box;
		-webkit-line-clamp: 1;
		line-clamp: 1;
		-webkit-box-orient: vertical;
	}
</style>
