<script>
	import LazyImage from '../components/lazy-image.svelte';
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Humans coming together." />
</svelte:head>

<div class="h1-wrapper">
	<h1>Let’s do dinner.</h1>
</div>

<div class="page">
	<p>
		Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut
		labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco
		laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in
		voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat
		non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
	</p>

	<h3>Find us on:</h3>
	<ul>
		<li>Eventbrite</li>

		<li>Meetup.com</li>

		<li>Foursquare</li>
	</ul>

	<div class="image-styles">
		<LazyImage src="/sunset.png" alt="Sunset" />
	</div>

	<br />
	<br />
</div>

<style lang="scss">
	.image-styles {
		position: relative;
		max-height: 400px;
		max-width: 800px;
		margin-top: 2rem;
		margin-bottom: 1rem;
		display: block;
	}

	.icon {
		width: 0.8rem;
		position: relative;
		top: 0.1rem;
		left: 0.12rem;
	}
</style>
