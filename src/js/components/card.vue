<template>
	<div class="card">
		<div class="detail">
			<div class="city">{{ city }}</div>
			<div class="weather">SUNNY</div>
			<div class="temp">25</div>
		</div>
		<div class="icon">
			<img src="icons/sunny.svg" alt="">
		</div>
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
		margin-bottom: 1rem;
		justify-content: space-between;
		align-items: center;
	}
	.city{
		font-size: 11px;
		font-weight: 100;
		color: #666666;
		letter-spacing: .1rem;
	}
	.weather{
		letter-spacing: .1rem;
	}
	.temp{
		font-weight: 600;
		font-size: 2rem;
		&::after{
			content: "\00b0";
		}
	}
</style>