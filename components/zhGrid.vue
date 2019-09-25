<template>
	<view class='zhGrid'>
		<view class='zhGrid-Item'
			:class='column'
			:key='index'
			v-for='(item,index) in zhGridData'
			@click='zhGrid(item,index)'
		>
			<view class='zhGrid-Item-Img'>
				<image class='maxImg' :src="item.url" mode="图片路径不对"></image>
			</view>
			<text class='zh_fs14'>{{item.text}}</text>
		</view>
	</view>
</template>

<script>
	export default {
		name:'zhGrid',
		props:{
			//数据
			zhGridData:{
				type:[Boolean, Array],
				default:false
			},
			// 几列显示
			column:{
				type:[Boolean,String],
				default:false
			}
		},
		data() {
			return {

			};
		},
		methods:{
			//列表点击
			zhGrid(item,index){
				this.$emit("click",{item,index})
			}
		},
		mounted(){

		}
	}
</script>

<style lang="less">
</style>
