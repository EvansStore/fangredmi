<template>
	<view style="width: 375upx;">
		<image :src="item.cover"
		 lazy-load
		 mode="widthFix"></image>
	<view class="p-2 pt-1">
		<view class="font-md">{{item.title}}</view>
		<text class="d-block font text-light-muted">{{item.desc}}</text>
		<view class="d-flex my-1">
			<price :price="item.oprice"/>
			<view class="font-sm text-light-muted line-through ml-1 a-self-end line-h">￥{{item.pprice}}</view>
			</view>
	</view>
	</view>
</template>

<script>
	import price from "../../components/common/price.vue"
export default {
	components:{
		price
	},
	props:{
		item:Object,
		index:Number
	}
}

</script>

<style>
</style>
