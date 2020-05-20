<template>
	<view class="content">
		<view class="text-area">
			<text class="title">{{title}}</text>
		</view>
		<view class="button-sp-area" id="button-id">
			<button type="primary" plain="true" @click="jump">开启小说之旅</button>
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
			
		},
		methods: {
			jump(){
				// uni.login({
				//   provider: 'weixin',
				//   success: function (loginRes) {
				//     console.log(loginRes.authResult);
				//     // 获取用户信息
				//     uni.getUserInfo({
				//       provider: 'weixin',
				//       success: function (infoRes) {
				//         console.log('用户昵称为：' + infoRes.userInfo.nickName);
				//       }
				//     });
				//   }
				// });
				uni.switchTab({
				    url: '/pages/home/home'
				});
			}
		}
	}
</script>

<style>
	 @font-face {
		font-family: 'iconfont';
		src: url('http://book.tiny-app.top/static/fonts/smt.737bf92.ttf');
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
		position: fixed;
		bottom: 20%;
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
