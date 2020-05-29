<template>
	<view class="d-flex">
		<image :src="resdata.big.src" 
		lazy-load
		style="width: 373upx;height: 530upx;border-right: 2upx solid #f5f5f5;"
		@tap="event(resdata.big)"
		mode=""></image>
		
		<view class="d-flex flex-column">
			<image :src="resdata.smalltop.src"
			 style="width: 375upx; height: 264upx;border-bottom: 2upx solid #f5f5f5;"
			 @tap="event(resdata.smalltop)"
			 mode=""></image>
			 
			 <image :src="resdata.smallbottom.src"
			  style="width: 375upx; height: 264upx;"
			  @tap="event(resdata.smallbottom)"
			  mode=""></image>
		</view>
	</view>
</template>

<script>
	export default {
		props:{
			resdata:Object
		},
		methods:{
			event(obj){
				console.log(obj)
			}
		}
	}
</script>

<style>
</style>
