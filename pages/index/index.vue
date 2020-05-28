<template>
	<view class="content">
		<swiper :indicator-dots="true" :autoplay="true" :interval="3000" :duration="1000">
			<swiper-item>
				<view class="swiper-item">
					<image src="../../static/images/demo/demo4.jpg" 
					lazy-load
					style="height: 350upx;"
					></image>
				</view>
			</swiper-item>
			<swiper-item>
				<view class="swiper-item">
					<image src="../../static/images/demo/demo4.jpg" 
					lazy-load
					style="height: 350upx;"
					></image>
				</view>
			</swiper-item>
			</swiper>
		
	</view>
</template>

<script>
	export default {
		data() {
			return {
			
			}
		},
		onLoad() {

		},
		methods: {
			
		}
	}
</script>

<style>
	
</style>
