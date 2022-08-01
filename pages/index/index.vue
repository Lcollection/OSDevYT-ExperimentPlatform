<template>
	<view class="content">
		<!-- 接下来会有两个图片作为跳转页面的工具，这两个图片都有一个点击事件 -->
		<view class="pic1">
			<image src="../../static/Laboratory.jpg" @click="goLab()"></image>
		</view>
		<view class="pic2">
			<image src="../../static/BreedingRoom.jpg" @click="goBreed()"></image>
		</view>
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
			// 这是两个点击事件触发后的行为
			goLab() {
				uni.navigateTo({
					url:'../Lab/Lab'
				})
			},
			goBreed() {
				uni.navigateTo({
					url:'../Breed/Breed'
				})
			}
		}
	}
</script>

<style>
	.content {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}

	.logo {
		height: 200rpx;
		width: 200rpx;
		margin-top: 200rpx;
		margin-left: auto;
		margin-right: auto;
		margin-bottom: 50rpx;
	}

	.text-area {
		display: flex;
		justify-content: center;
	}

	.title {
		font-size: 36rpx;
		color: #8f8f94;
	}
	.pic1 {
		padding-top: 200px;
	}
	.pic2 {
		padding-top: 50px;
	}
</style>
