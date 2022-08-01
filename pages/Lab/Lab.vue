<template>
	<view>
		<!-- //三个按钮控件，分别有一个点击事件，跳转到各个页面 -->
		<button class="button1" @click="goReady()">准备室门口</button>
		<button class="button2" @click="goTrans()">传递舱</button>
		<button class="button3" @click="goLabTable()">试验台</button>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			}
		},
		methods: {
			//三个事件的行为
			goReady() {
				uni.navigateTo({
					url:'../ReadyRoom/ReaydRoom'
				})
			},
			goTrans() {
				uni.navigateTo({
					url:'../Trans/Trans'
				})
			},
			goLabTable() {
				uni.navigateTo({
					url:'../LabTable/LabTable'
				})
			}
		}
	}
</script>

<style>

</style>
