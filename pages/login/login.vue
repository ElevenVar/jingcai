<template>
	<view class='zh_login'>
		<view class='zh_login_Input'>
			<view class='zh_imgTitle'>
				<img src="../../static/loginImg/sjh.png" alt="">
			</view>
			<input type="text" placeholder="请输入账号">
		</view>
		<view class='zh_login_Input'>
			<view class='zh_imgTitle'>
				<img src="../../static/loginImg/yzm.png" alt="">
			</view>
			<input type="password" placeholder="请输入密码">
		</view>
		<view class='zh_login_Input blue' @tap='subMit'>登录</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			};
		},
		methods:{
			//登录
			subMit(){
				console.log(0)
				uni.switchTab({
					url:"../home/home"
				})
			}
		}
	}
</script>

<style lang="less">
	.blue{
		background-color: #2292DD !important;color:#fff !important;text-align: center;
	}
	.zh_login{
		padding:20px;font-size:14px;
		.zh_login_Input{
				background-color:#f2f2f2;border-radius:5px;margin-bottom:25px;height:40px;overflow: hidden;position:relative;line-height:40px;
				.zh_imgTitle{
					position:absolute;width:17px;height:17px;left:15px;top:5px;
					img{
						width:100%;height:100%;
					}
				}
				input{
					display: block;width:100%;border:none;background-color:#f2f2f2;height:100%;text-indent:5px;padding-left:40px;
				}
		}
	}
</style>
