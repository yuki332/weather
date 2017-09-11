<template>
	<div class="card">
		<div class="city">{{ city }}</div>
	</div>
</template>
<script>
	export default{
		name: 'card',
		data() {
			return {
				city: 'Salt Lake, UT'
			}
		},
		props: ['title', 'background'],
	}
</script>
<style lang="scss" scoped>
	$gray: #eee;
	.card {
		display: flex;
		background: $gray;
		padding: 1rem;
		border-radius: 10px;
		margin-bottom: 1rem;
	}
	.city{
		font-size: 2rem;
		font-weight: 600;
	}
</style>