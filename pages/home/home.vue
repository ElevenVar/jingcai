<template>
	<view class='home'>
		<view class='zh_header'>
			<img class='maxImg' src="../../static/homeImg/banner1.png" alt="">
		</view>
		<view class='gridBox zh_pd10'>
			<zh-grid
				:zhGridData = "GridItem"
				@click = 'onClick'
			>
			</zh-grid>
		</view>
		<view class='listBox'>
			<zh-list></zh-list>
		</view>
	</view>
</template>

<script>
	import zhGrid from '../../components/zhGrid.vue';
	import zhList from '../../components/zhList.vue';
	export default {
		components:{
			zhGrid,zhList
		},
		data() {
			return {
				GridItem: [{
						url: '../../static/homeImg/hfcz.png',
						text: '学杂费'
					},
					{
						url: '../../static/homeImg/hfcz.png',
						text: '成绩查询'
					},
					{
						url: '../../static/homeImg/hfcz.png',
						text: '课程'
					},
					{
						url: '../../static/homeImg/hfcz.png',
						text: '消息'
					},
				],
			};
		},
		methods:{
			onClick(data){
				console.log(data)
			}
		}
	}
</script>

<style lang="less">

</style>
