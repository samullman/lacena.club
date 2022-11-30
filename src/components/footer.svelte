<script>
	import { page } from '$app/stores';
</script>

<footer>
	<div>
		<a href="/" data-sveltekit-prefetch>
			{$page.url.host}
		</a>
	</div>

	<div class="built-with">
		Built with <a href="https://kit.svelte.dev/" target="_blank" rel="noreferrer">SvelteKit</a> 🤯
	</div>
</footer>

<style lang="scss">
	footer {
		max-width: $max-width;
		margin: 0 auto;
		margin-top: 1rem;
		margin-bottom: 1rem;
		display: flex;
		padding: 1rem;
		flex-direction: column;
		justify-content: left;

		@media screen and (min-width: $breakpoint) {
			justify-content: space-between;
			flex-direction: row;

			padding: 2rem;
		}
	}
</style>
