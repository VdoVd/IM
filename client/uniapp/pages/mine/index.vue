<template>
	<view class="box">
		
		<view>mine</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				tel: '',
				pass: ''
			}
		},
		// onLoad() {
		// 	setTimeout(()=>{
		// 		this.submit()
		// 	},3000)
		// },
		methods:{
			submit(){
				uni.navigateTo({
					url:'/pages/index/index'
				}),
				uni.showToast({
					data:"login"
				})
			}
		}
	}
</script>
<style lang="scss" scoped>
	.box{
		// background-color: rgba(0,0,0,0.2);
		display: flex;
		width: 100vw;
		height: 100vh;
		flex-direction: column;
		row-gap: 70rpx;
		align-items: center;
		justify-content: center;
		padding: 20rpx;
		.input{
			background-color: $uni-bg-color-grey;
			width: 80vw;
			text-align: start;
		}
		.button{
			width: 80vw;
		}
	}
</style>
