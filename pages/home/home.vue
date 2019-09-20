<template>
	<view class='home'>
		<view class='zh_header'>
			<img class='maxImg' src="../../static/homeImg/banner1.png" alt="">
		</view>
		<view class='gridBox'>
			<zh-grind></zh-grind>
		</view>
	</view>
</template>

<script>
	import zhGrind from '../../components/zhGrid.vue'
	export default {
		components:{
			zhGrind
		},
		data() {
			return {
				
			};
		}
	}
</script>

<style lang="less">

</style>
