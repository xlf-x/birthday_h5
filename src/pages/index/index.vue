<template>
	<view class="content"
		@click="playBgm">
		<div class="bokeh"></div>
		<div class="bokeh"></div>
		<div class="bokeh"></div>
		<div class="bokeh"></div>
		<div class="bokeh"></div>
		<div class="bokeh"></div>
		<div class="bokeh"></div>
		<div class="bokeh"></div>
		<div class="bokeh"></div>
		<div class="bokeh"></div>
		<div class="bokeh"></div>
		<div class="bokeh"></div>
		<div class="bokeh"></div>
		<div class="bokeh"></div>
		<div class="bokeh"></div>
		<div class="bokeh"></div>
		<div class="bokeh"></div>
		<div class="bokeh"></div>
		<div class="bokeh"></div>
		<div class="bokeh"></div>
		<div class="bokeh"></div>
		<div class="bokeh"></div>
		<div class="bokeh"></div>
		<div class="bokeh"></div>
		<div class="bokeh"></div>
		<div class="bokeh"></div>
		<div class="bokeh"></div>
		<div class="bokeh"></div>
		<div class="bokeh"></div>
		<div class="bokeh"></div>
		<div class="bokeh"></div>
		<div class="bokeh"></div>
		<div class="bokeh"></div>
		<div class="bokeh"></div>
		<div class="bokeh"></div>
		<div class="bokeh"></div>
		<div class="bokeh"></div>
		<div class="bokeh"></div>
		<div class="bokeh"></div>
		<div class="bokeh"></div>
		<div class="bokeh"></div>
		<div class="bokeh"></div>
		<div class="bokeh"></div>
		<div class="bokeh"></div>
		<div class="bokeh"></div>

		<div class="center-box">
			<p class="title-1">世界上最可爱的小徐生日快乐！</p>
			<p class="title-2">超级超级爱你</p>
			<!-- <span>🎉</span> -->
			<div class="candle">
				<div id="flame" class="lit"></div>
			</div>

			<div class="cake"></div>
			<div class="plate"></div>
		</div>
	</view>
</template>

<script>
import bokeh from '@/components/bokeh'
export default {
	components: {
		bokeh,
	},
	data() {
		return {
			innerAudioContext: '',
		}
	},
	onLoad() {
		this.innerAudioContext = uni.createInnerAudioContext()
		this.innerAudioContext.autoplay = true
		this.innerAudioContext.src = 'https://win-web-nf01-sycdn.kuwo.cn/92d26fd9fb306790293fbc27c397185b/63eb54d1/resource/n2/96/49/2798292777.mp3'
	},
	methods: {
		playBgm () {
			this.innerAudioContext.play()
		}
	}
}
</script>

<style src="./index.css" scoped>
</style>
