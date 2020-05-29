<template>
	<view class="card">
		<!-- 头部 -->
		<view class=" p-2 border-bottom mian-border-color">
			<slot name="title">
				<text v-if="headTitle" class="font-md font-weight"> {{headTitle}} </text>
			</slot>
		</view>
		
		<!-- body -->
		<view>
			<image v-if="bodyCover" :src="bodyCover" mode="widthFix"></image>
			<slot />
		</view>
	</view>
</template>
 
<script>
	export default {
		props:{
			headTitle:String,
			bodyCover:String
		}
	}
</script>

<style>
</style>
