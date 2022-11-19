<script>
	import LazyImage from '../components/lazy-image.svelte';
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Meeting with humans." />
</svelte:head>

<h1>Let's do dinner.</h1>

<div class="image-styles">
	<LazyImage src="/sunset.png" alt="Sunset" />
</div>

<br />
<br />

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
