<template>
	<div>
		<h2>About Me</h2>
		<p>
			Greetings! My name is Nsovo Ngobeni and I'm a 
			passionate web designer and developer from South Africa.
			My experience has taught me that good design is not created 
			in a moment of inspiration. It is a iterative process 
			requiring coloboration between multiple teams and your end
			users.
		</p>
	</div>
</template>

<script>
	export default {
		name: 'About' 
	}
</script>

<style scoped>
	div {
		margin: auto;
		margin-top: 10vh;
		width: 75%;
		text-align: center;
	}

	h2 {
		font-weight: normal;
		font-size: 175%;
	}

	h2:after {
		content: '';
		display: block;
		background-color: var(--emphasised-color);
		width: 175px;
		height: 3px;
		margin: auto;
	}

	p {
		margin-top: 5.5vh;
	}
</style>