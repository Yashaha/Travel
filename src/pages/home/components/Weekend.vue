<template>
	<div>
		<div class="weekend-title">周末去哪儿</div>
		<ul>
			<li class="item border-bottom" v-for="item of recommendList" :key="item.id">
				<div class="item-img-wrapper">
					<img class="item-img" :src="item.imgUrl" />
				</div>
				<div class="item-info">
					<p class="item-title">{{item.title}}</p>
					<p class="item-desc">{{item.desc}}</p>
				</div>
			</li>
		</ul>
	</div>
</template>

<script>
export default {
	name: 'HomeWeekend',
	data () {
		return {
			recommendList: [{
				id: '0001',
				imgUrl: 'http://img1.qunarzz.com/sight/source/1505/92/580e9ea4f37a1b.jpg_r_640x214_72112761.jpg',
				title: '广州长隆旅游度假区',
				desc: '10086条评论'
			}, {
				id: '0002',
				imgUrl: 'http://img1.qunarzz.com/sight/source/1505/92/580e9ea4f37a1b.jpg_r_640x214_72112761.jpg',
				title: '广州长隆旅游度假区',
				desc: '10086条评论'
			}, {
				id: '0003',
				imgUrl: 'http://img1.qunarzz.com/sight/source/1505/92/580e9ea4f37a1b.jpg_r_640x214_72112761.jpg',
				title: '广州长隆旅游度假区',
				desc: '10086条评论'
			}, {
				id: '0004',
				imgUrl: 'http://img1.qunarzz.com/sight/source/1505/92/580e9ea4f37a1b.jpg_r_640x214_72112761.jpg',
				title: '广州长隆旅游度假区',
				desc: '10086条评论'
			}, {
				id: '0005',
				imgUrl: 'http://img1.qunarzz.com/sight/source/1505/92/580e9ea4f37a1b.jpg_r_640x214_72112761.jpg',
				title: '广州长隆旅游度假区',
				desc: '10086条评论'
			}, {
				id: '0006',
				imgUrl: 'http://img1.qunarzz.com/sight/source/1505/92/580e9ea4f37a1b.jpg_r_640x214_72112761.jpg',
				title: '广州长隆旅游度假区',
				desc: '10086条评论'
			}]
		}
	}
}
</script>

<style lang="stylus" scoped>
	@import '~styles/mixins.styl'
	.weekend-title
		line-height: .8rem
		background: #eee
		text-intent: .2rem
		margin-top: .2rem
	.item-img-wrapper
		overflow: hidden
		height: 0
		padding-bottom: 33.9%
	.item-img
		width: 100%
	.item-info
		flex: 1
		padding: .1rem
		min-width: 0
		.item-title
			line-height: .54rem
			font-size: .32rem
			ellipsis()
		.item-desc
			line-height: .4rem
			color: #ccc
			ellipsis()
</style>