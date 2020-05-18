<template>
	<view class="home-book">
		<view class="uni-form-item uni-column">
			<input class="uni-input" focus placeholder="搜索小说" />
		</view>
		<view class="">
			<view class="home-title">
				<view class="home-title-paihang">
					点击排行
				</view>
				<view class="">
					更多
				</view>
			</view>
			<view class="home-book-hot">
				<view class="">
					<image src="../../static/logo.png" mode=""></image>
				</view>
			</view>
		</view>
	</view>
</template>

<script>
</script>

<style>
	.home-book {
		
	}
	.uni-column {
		padding: 3% 10%;
		height: 80upx;
		padding-top: 20upx;
	}
	.uni-input {
		height: 1.8rem;
		border: .04rem solid #555555;
		padding: 7upx;
		border-radius: 11upx;
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
</style>
