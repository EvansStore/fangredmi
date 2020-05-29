<template>
	<view >
		<!-- 轮播图 -->
		<swiperImage :resdata="imgs"></swiperImage>
		
		<!-- 首页分类 -->
		<indexNav :resdata="indexnavs"></indexNav>
		<!-- 分割线 -->
		<divider></divider>
		
		<!-- 大广告 -->
		<threeAdv :resdata="threeAdv"></threeAdv>
		
		<!-- 大图广告 -->
		<card>
			<block slot="title">精选货物</block>
			<image src="../../static/images/demo/demo5.jpg" mode="widthFix"></image>
		</card>
		
		<!-- 公共列表组件 -->
		<view class="row j-sb">
			<block v-for="(item,index) in commonList" :key="index">
		<commonList :item="item" :index="index"></commonList>
		</block>
		</view>
		
	</view>
</template>

<script>
	import swiperImage from "@/components/index/swiper-image.vue"
	import indexNav from "@/components/index/index-nav.vue"
	import threeAdv from "@/components/index/three-adv.vue"
	import card from "@/components/common/card.vue"
	
	import commonList from "../../components/common/common-List.vue"
	export default {
		components:{
			swiperImage,
			indexNav,
			threeAdv,
			card,
	
			commonList
		},
		data() {
			return {
				imgs:[
					{src:"../../static/images/demo/demo4.jpg"},
					{src:"../../static/images/demo/demo4.jpg"},
					{src:"../../static/images/demo/demo4.jpg"}
				],
				
				indexnavs:[
				{src:"../../static/images/indexnav/1.png",text:"新品发布"},
				{src:"../../static/images/indexnav/2.gif",text:"新品发布"},
				{src:"../../static/images/indexnav/3.gif",text:"新品发布"},
				{src:"../../static/images/indexnav/4.gif",text:"新品发布"},
				{src:"../../static/images/indexnav/5.gif",text:"新品发布"},
				{src:"../../static/images/indexnav/6.gif",text:"新品发布"},
				{src:"../../static/images/indexnav/7.gif",text:"新品发布"},
				{src:"../../static/images/indexnav/8.gif",text:"新品发布"},
				{src:"../../static/images/indexnav/9.gif",text:"新品发布"},
				{src:"../../static/images/indexnav/10.gif",text:"新品发布"},
				],
				
				threeAdv:{
					big:{
						 src:"/static/images/demo/demo1.jpg" 
					},
					smalltop:{
						src:"/static/images/demo/demo2.jpg"
					},
					smallbottom:{
						src:"/static/images/demo/demo3.jpg"
					}
				},
				
				commonList:[
					{
						cover:"../../static/images/demo/cate_05.png",
						title:"米家空调",
						desc:"1.5匹变频",
						oprice:2699,
						pprice:1399
					},
					{
						cover:"../../static/images/demo/cate_05.png",
						title:"米家空调",
						desc:"1.5匹变频",
						oprice:2699,
						pprice:1399
					},
					{
						cover:"../../static/images/demo/cate_05.png",
						title:"米家空调",
						desc:"1.5匹变频",
						oprice:2699,
						pprice:1399
					},
					{
						cover:"../../static/images/demo/cate_05.png",
						title:"米家空调",
						desc:"1.5匹变频",
						oprice:2699,
						pprice:1399
					}
				]
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
