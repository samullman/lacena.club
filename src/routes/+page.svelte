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
	<h2>
		Let's do <a href="/calendar">dinner</a>.
	</h2>

	<p>
		We're cooking up some of the best opportunities to dine with fellow Austintines. Tickets are
		available on a first-come, first-serve basis and seating is limited!
	</p>

	<LazyImage src="/dinner-table.jpeg" alt="Dinner Table" />
</div>

<style lang="scss">
</style>
