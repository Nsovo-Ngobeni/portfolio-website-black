<template>
	<div id='header'>
		<TextField :name=name />
		<img src='../assets/images/my-photo.jpg' />
	</div>
</template>

<script>
	import TextField from './Header Components/TextField.vue'
	export default {
		name: 'Header',
		props: {
			name: String,
		}, 
		components: {
			TextField
		}
	}
</script>

<style scoped>

	#header {
		display: grid;
		grid-template-columns: 1fr 1fr;
		align-content: center;
		margin-top: -7.5vh;
		height: 85vh;
		background-image: linear-gradient(rgba(0, 0, 0, 0.35), rgba(0, 0, 0, 0.70)),
		url('../assets/images/CodeWall.jpg');
		background-size: cover;
		background-position: centre;
		
	}

	img {
		height: 50vh;
		border-radius: 75px;
		display: block;
		margin: auto;
	}

	@media screen and (max-width: 750px) {
    #header {
			grid-template-columns: 1fr;
			grid-template-rows: 1fr 1fr;
		}

		img {
			height: 25vh;
		}
  }

</style>