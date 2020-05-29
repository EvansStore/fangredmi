<template>
<view class="d-flex mian-text-color font-md line-h">
					<text class="a-self-start font-sm ">￥</text>{{price}}
				</view>
</template>

<script>
	export default {
		props:{
			price:[String,Number]
		}
	}
</script>

<style>
</style>
