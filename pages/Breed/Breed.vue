<template>
	<view>
		<button class="button1" @click="goReadrRoom()">准备室门口</button>
		<button class="button2" @click="goTrans()">传递舱</button>
		<button class="button3" @click="goBreedRoom()">饲养室</button>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			}
		},
		methods: {
			goReadrRoom() {
				uni.navigateTo({
					url:'../ReadyRoom/ReaydRoom'
				})
			},
			goTrans() {
				uni.navigateTo({
					url:'../Trans/Trans'
				})
			},
			goBreedRoom() {
				uni.navigateTo({
					url:'../BreedRoom/BreedRoom'
				})
			}
		}
	}
</script>

<style>

</style>
