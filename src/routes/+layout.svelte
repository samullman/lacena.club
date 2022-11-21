<script>
	import '../../src/app.scss';
	import Header from '../components/header.svelte';
	import Footer from '../components/footer.svelte';

	// import { page } from '$app/stores';
	// import pageViews from '../stores/page';
	// import { beforeUpdate } from 'svelte';

	// $pageViews;

	// beforeUpdate(() => {
	// 	$pageViews[$page.url.pathname] = true;
	// 	pageViews.set($pageViews);
	// });
</script>

<Header />

<main>
	<slot />
</main>

<Footer />

<style lang="scss">
</style>
