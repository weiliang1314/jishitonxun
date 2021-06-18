<template>
	<view class="content">
		<view class="topbar">
			<view class="left"><image src="../../static/images/img-one/tou1.jpeg"></image></view>
		
		<view class="center"><image src=""></image></view>
		
		<view class="right"><view class="search"><image src="../../static/images/img-one/搜索.png"></image></view>
		<view class="search"><image src="../../static/images/img-one/+.png"></image></view></view>
		</view>
		<view class="main"><view class="friends">
			<view class="frinendlist">
				<view class="friendl">
					<text class="tip">1</text>
					<image src="../../static/images/img-one/好友申请.png"></image>
				</view>
				<view class="friendr">
					<view class="top">
						<view class="name">好友申请</view>
						<view class="time">14:39</view>
					</view>
					<view class="conents">你有新朋友</view>
				</view>
			</view>
		</view>
		<view class="friends">
			<view class="frinendlist">
				<view class="friendl">
					<text class="tip">1</text>
					<image src="../../static/images/img-one/tou2.jpeg"></image>
				</view>
				<view class="friendr">
					<view class="top">
						<view class="name">未完待续</view>
						<view class="time">14:39</view>
					</view>
					<view class="conents">哈市的地方已确定是否时qjhhjsagdyg舍不得花洒电锯惊魂规划局</view>
				</view>
			</view>
		</view></view>
		</view>
</template>

<script>
	export default {
		data() {
			return {
				title: 'Hello'
			}
		},
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style lang="scss">
	.content {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}
	.topbar{
		z-index: 1000;
		height:88rpx;
		width: 100%;
		position: fixed;
		display: flex;
		left: 0;
		top:0;
		background: $uni-bg-color;
		box-shadow: 0px 1px 0px 0px rgba(0,0,0,0.1);
		view{
			
			display: flex;
			justify-content: center;
			align-items: center;
			
		}
		.left{
			padding: 10rpx 15rpx;
			image{
				height: 68rpx;
				width: 68rpx;
				border-radius: 16rpx;
			}
		}
		.center{
			flex: 1;
			image{
				height: 88rpx;
				width: 108rpx;
				
			}
		}
		.right{
			padding: 10rpx 15rpx;
			.search{
				margin-right: 25rpx;
			}
			
			image{
				height: 42rpx;
				width: 42rpx;
				
			}
		}
		
	}
.main{
	padding:88rpx $uni-spacing-col-base;
	width: 100%;
}
	.frinendlist{
	padding: 16rpx 0;
	display: flex;
	
		.friendl{
		  position:relative;
			padding: 0 10rpx;
			image{
				height: 88rpx;
				width: 88rpx;
				border-radius: 16rpx;
			}
			.tip{
				
				position: absolute;
				z-index: 10;
				top:-6rpx;
				left: 78rpx;
				height: 30rpx;
				width:30rpx;
				font-size: $uni-font-size-sm;
				color: $uni-text-color-inverse;
				background: $uni-color-warning;
				border-radius: $uni-border-radius-circle;
				line-height: 30rpx;
				text-align: center;
				
			}
		}
		.friendr{
			flex: 1;
		padding: 0 $uni-spacing-col-base ;
		
		.top{
			overflow:hidden;
			height: 50rpx;
			.name{
				float:left;
				font-size: 36rpx;
				font-weight: 400;
				color: rgba(39,40,50,1);
				text-align: center;
				line-height: 50rpx;
				
			}
			.time{
				overflow: hidden;
				margin-left: 550rpx;
			line-height: 50rpx;
			text-align: center;
			font-size: $uni-font-size-sm;
			color:$uni-text-color-grey
				
			}
		}
		.conents{
			font-size: $uni-font-size-sm;
			color:$uni-text-color-grey;
			line-height: 40rpx;
			display: -webkit-box;
			-webkit-box-orient:vertical;
			-webkit-line-clamp:1;
			overflow: hidden;
				
		}
		}
	}
</style>
