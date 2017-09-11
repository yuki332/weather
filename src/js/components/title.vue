<template>
	<div>
		<nav>
			<span class="symbol">&#43;</span>
			<h1>TENKI</h1>
			<span class="symbol">&#8451;</span>
		</nav>
	</div>
</template>
<script>
	export default{
		name: 'title',
		data() {
			return {
			}
		},
		props: ['title', 'background'],
	}
</script>
<style lang="scss" scoped>
	nav {
		display: flex;
		justify-content: space-between;
		margin: 3rem auto;
	}
	h1 {
		margin: 0;
		font-size: 3rem;
	}
	.symbol{
		font-size: 3rem;
	}
	.message {
		color: #dddddd;
	}
</style>