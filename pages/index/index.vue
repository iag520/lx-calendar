<template>
	<view class="content">

		<lxCalendar :value="'2020-10-01'" @change="change"></lxCalendar>
	</view>
</template>

<script>
	import lxCalendar from '../../components/lx-calendar/lx-calendar.vue'
	export default {
		components:{
			lxCalendar,
		},
		data() {
			return {
				title: 'Hello'
			}
		},

		onLoad() {

		},
		methods: {
			change(e){
				console.log(e);
			}

		}
	}
</script>

<!-- 		<picker mode="date" start="2019-12-30">试试</picker>
		<view @click="to_member">会员</view> -->

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
</style>
