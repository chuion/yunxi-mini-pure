<template>
	<view class="content">
		<image class="logo" src="/static/logo.png"></image>
		<view class="text-area">
			<text>123123</text>
			<text class="title">{{title}}</text>
			<uni-card title="基础卡片" extra="额外信息">
				<text>这是一个基础卡片示例，内容较少，此示例展示了一个没有任何属性不带阴影的卡片。</text>
			</uni-card>
		</view>
	</view>
</template>

<script setup>
	import {ref} from 'vue'
const title = ref('Hello')
console.log('>>> title: ', title)
</script>

<style scoped lang='scss'>
	.content {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		
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
			flex-direction: column;
		}
		
		.title {
			font-size: 36rpx;
			color: #8f8f94;
		}
	}


</style>
