<template>
	<div class="container">
		<div class="date">SUNDAY | NOV 28</div>
		<card></card>
		<card></card>
		<card></card>
		<card></card>
		<card></card>
	</div>
</template>
<script>
	import card from './card.vue';
	export default{
		name: 'container',
		components: {
			card
		},
		data() {
			return {
			}
		}
	}
</script>
<style lang="scss" scoped>
	.container {
		margin-right: 3rem;
		margin-left: 3rem;
	}
	.date {
		font-size: 2rem;
		margin-bottom: 1rem;
	}
</style>