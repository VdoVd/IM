<template>
	<view class="box">
		<u-field
			v-model="tel"
			label="telphone"
			placeholder="please input phone"
		>
		</u-field>
		<u-field
			v-model="pass"
			label="password"
			placeholder="please input password"
		>
		</u-field>
		<u-button type="primary" class="button">login</u-button>

	</view>
</template>

<script>
	export default {
		data() {
			return {
				tel: '',
				pass: ''
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
		.button{
			width: 80vw;
		}
	}
</style>
