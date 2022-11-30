<script>
	import LazyImage from '../components/lazy-image.svelte';
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Let's do dinner." />
</svelte:head>

<div class="h1-wrapper">
	<h1>Welcome to the club!</h1>
</div>

<div class="page">
	<LazyImage src="/silver-fruit.jpeg" alt="Lemon" />

	<p>
		La Cena ("The Dinner") Club was born out of the desire to break bread with fresh company in the
		Austin area.
	</p>

	<p>We believe amazing things happen when great people get together over incredible food.</p>

	<p>
		This is your opportunity to experience unique, full-course meals in a socially driven
		environment at some of Austin's top culinary destinations.
	</p>

	<p>
		Hope to <a href="/calendar">see you soon</a>.
	</p>
</div>

<style lang="scss">
</style>
