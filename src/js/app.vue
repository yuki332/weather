<template>
	<div>
		<appTitle></appTitle>
		<container></container>
	</div>
</template>
<script>
	import container from './components/container.vue';
	import appTitle from './components/title.vue';
	export default{
		name: 'app',
		components: {
			appTitle,
			container
		},
		data(){
			return {
				title: 'We are Sorry...',
				message: 'The App is Under Construction...'
			}
		}
	}
</script>
<style lang="scss" scoped>
	$primary: #AEAEAE;
	$title: 3rem;
	* {
		font-family: 'Raleway', sans-serif;
		font-weight: 100;
	}
	h1 {
		font-size: $title;
	}
	.flex-center {
		display: flex;
		justify-content: center;
		align-items: center;
	}
	.full-height{
		height: 100vh;
	}
	.message{
		text-align: center;
		color: $primary;
	}
</style>