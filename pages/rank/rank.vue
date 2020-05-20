<template>
	<view>
		<search></search>
		<view class="book-typys">
			<view class="book-typs-name">玄幻魔法</view>
			<view class="book-typs-name">修真武侠</view>
			<view class="book-typs-name">修真武侠</view>
			<view class="book-typs-name">修真武侠</view>
			<view class="book-typs-name">修真武侠</view>
			<view class="book-typs-name">修真武侠</view>
		</view>
		<view class="book-type-list">
			<view class="book-type-list-div">
				<view class="book-type-list-name">超神机械师</view>
				<view class="book-type-list-author">作者:小草</view>
			</view>
			<view class="book-type-list-div">
				<view class="book-type-list-name">超神机械师</view>
				<view class="book-type-list-author">作者:小草</view>
			</view>
			<view class="book-type-list-div">
				<view class="book-type-list-name">超神机械师</view>
				<view class="book-type-list-author">作者:小草</view>
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
.book-typys {
		display: flex;
		flex-wrap: wrap;
		padding: 1rem 2.5rem;
		justify-content:space-between
	}
	.book-typs-name {
		width: 40%;
		text-align: center;
		padding: .3rem;
		margin-bottom: .8rem;
		border: .04rem solid #d6d6d6;
		color: #5f6779;
		border-radius: 5px;

	}
	.book-type-list-div {
		margin-left: 2.5rem;
		margin-right: 2.5rem;
		padding-bottom: .5rem;
		margin-bottom: .5rem;
		border-bottom: .04rem solid #e8eaec;
		color:#5f6779;
	}
	.book-type-list-div:last-child {
		border-bottom: none;
	}
	.book-type-list-name {
		margin-bottom: .2rem;
	}
	.book-type-list-author {
		font-size: 30upx;
		color: #00000073;
	}
</style>
