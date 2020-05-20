<template>
	<view class="button-btn">
		<view class="button-btn-div">
			<navigator url="/pages/home/home">
				<view class="floor-icon-div">
					<view v-if="msg == 1" class="iconfont icon-color">&#xe7bb;</view>
					<view v-else class="iconfont">&#xe7bb;</view>
					<view class="floor-icon-div-name">主页</view>
				</view>
			</navigator>
		</view>
		<view class="button-btn-div">
			<navigator url="/pages/types/types">
				<view class="floor-icon-div">
					<view v-if="msg == 2" class="iconfont icon-color">&#xe7f8;</view>
					<view v-else class="iconfont">&#xe7f8;</view>
					<view class="floor-icon-div-name">分类</view>
				</view>
			</navigator>
		</view>
		<view class="button-btn-div">
			<view class="floor-icon-div">
				<view v-if="msg == 3" class="iconfont icon-color">&#xe61a;</view>
				<view v-else class="iconfont">&#xe61a;</view>
				<view class="floor-icon-div-name">排行</view>
			</view>
		</view>
		<view class="button-btn-div">
			<view class="floor-icon-div">
				<view v-if="msg == 4" class="iconfont icon-color">&#xe605;</view>
				<view v-else class="iconfont">&#xe605;</view>
				<view class="floor-icon-div-name">完本</view>
			</view>
		</view>
		<view class="button-btn-div">
			<view class="floor-icon-div">
				<view v-if="msg == 5" class="iconfont icon-color">&#xe617;</view>
				<view v-else class="iconfont">&#xe617;</view>
				<view class="floor-icon-div-name">我的</view>
			</view>
		</view>
	</view>
</template>

<script>
	export default {
		props: {
		    msg: Number
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
	@font-face {font-family: "iconfont";
	  src: url('https://at.alicdn.com/t/font_1827807_4rnivnk3ow.eot?t=1589857482844'); /* IE9 */
	  src: url('https://at.alicdn.com/t/font_1827807_4rnivnk3ow.eot?t=1589857482844#iefix') format('embedded-opentype'), /* IE6-IE8 */
	  url('data:application/x-font-woff2;charset=utf-8;base64,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') format('woff2'),
	  url('https://at.alicdn.com/t/font_1827807_4rnivnk3ow.woff?t=1589857482844') format('woff'),
	  url('https://at.alicdn.com/t/font_1827807_4rnivnk3ow.ttf?t=1589857482844') format('truetype'), /* chrome, firefox, opera, Safari, Android, iOS 4.2+ */
	  url('https://at.alicdn.com/t/font_1827807_4rnivnk3ow.svg?t=1589857482844#iconfont') format('svg'); /* iOS 4.1- */
	}
	
	.iconfont {
	  font-family: "iconfont" !important;
	  font-size: 50upx;
	  font-style: normal;
	  -webkit-font-smoothing: antialiased;
	  -moz-osx-font-smoothing: grayscale;
	  margin-top: .5rem;
	}
	
	.iconleimupinleifenleileibie2:before {
	  content: "\e7f8";
	}
	
	.iconshezhi:before {
	  content: "\e6ed";
	}
	
	.iconsort:before {
	  content: "\e60e";
	}
	
	.iconwode:before {
	  content: "\e617";
	}
	
	.iconshujia:before {
	  content: "\e620";
	}
	
	.iconV:before {
	  content: "\e729";
	}
	
	.iconzhuye:before {
	  content: "\e7bb";
	}
	
	.iconshuji:before {
	  content: "\e605";
	}
	
	.iconpaihangbang:before {
	  content: "\e61a";
	}
	
	.iconlishi:before {
	  content: "\e75f";
	}

	.button-btn {
		display: flex;
		justify-content: space-between;
		position: fixed;
		bottom: 0;
		right: 0;
		left: 0;
		text-align: center;
		background: #f5f5f5;
		height: 4rem;
		border-top: 1px solid #c1c1c1;
		padding-left: 1rem;
		padding-right:1rem;
		color: #515a6e;
	}
	.icon-color {
		color: #0066CC;
	}
	.floor-icon-div {
		position: relative;
	}
	.floor-icon-div-name {
		position: absolute;
		top: 59upx;
		font-size: 26upx;
		text-align: center;
		width: 100%;
		
	}
	.button-btn-div{
		width: 10%;
	}
</style>
