<template>
	<view class="content">

		<view class="pic">
			<image src="../../static/banner-home.jpg" mode="scaleToFill" class="pic_img"></image>
		</view>


		<uni-grid :data="[
    {image:'https://img-cdn-qiniu.dcloud.net.cn/img/shu.png',text:'用户绑定'},
    {image:'https://img-cdn-qiniu.dcloud.net.cn/img/lindang.png',text:'个人资料'},
    {image:'https://img-cdn-qiniu.dcloud.net.cn/img/laoren.png',text:'加载动画'},
    {image:'https://img-cdn-qiniu.dcloud.net.cn/img/liwu.png',text:'列表'},
    {image:'https://img-cdn-qiniu.dcloud.net.cn/img/maozi.png',text:'详情'},
    {image:'https://img-cdn-qiniu.dcloud.net.cn/img/shoutao.png',text:'新增'},
    {image:'https://img-cdn-qiniu.dcloud.net.cn/img/xueqiao.png',text:'状态'},
    {image:'https://img-cdn-qiniu.dcloud.net.cn/img/xunlu.png',text:'商品类别'},
    {image:'https://img-cdn-qiniu.dcloud.net.cn/img/xuehua.png',text:'图标'}]">
		</uni-grid>






		
	</view>
</template>

<script>
	import uniGrid from '../../components/uni-grid.vue'
	export default {
		components: {
			uniGrid
		},
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
	.content {
		width: 100%;
	}

	.pic {
		width: 100%;
		height: 250upx;
	}

	.pic_img {
		width: 100%;
		height: 100%;
	}


	.nine {
		position: relative;
		width: 100%;
		height: 0;
		padding-bottom: 100%;
		margin-bottom: 15upx;
	}


	.list {
		position: absolute;
		top: 0;
		left: 0;
		width: 100%;
		height: 100%;
	}

	.list>view {
		width: calc(98% / 3);
		height: calc(98% / 3);
		margin-right: 1%;
		margin-bottom: 1%;
		overflow: hidden
	}

	.flex {
		display: flex;
		flex-wrap: wrap;
	}

	.flex>view {
		flex-grow: 1;
		background-color: #e4e4e4;
		text-align: center;
		color: #fff;
		font-size: 80upx;
		line-height: 2;
	}

	.flex>view:nth-of-type(3n) {
		margin-right: 0;
	}

	.flex>view:nth-of-type(n+7) {
		margin-bottom: 0;
	}

	.icoN {
		width: 100%;
		height: 100%;
		position: relative;
	}

	.ptitle {
		width: 50%;
		font-size: 30%;
		position: relative;
		top: 20%;
		left: -20%;
	}
</style>
