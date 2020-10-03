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
		margin: 10vh auto 10vh auto;
		width: 75%;
		text-align: center;
		background-color: var(--main-background-color);
	}

	h2 {
		font-weight: normal;
	}

	h2:after {
		content: '';
		display: block;
		background-color: var(--emphasised-color);
		width: 150px;
		height: 3px;
		margin: auto;
	}

	p {
		margin-top: 2.5vh;
	}
</style>