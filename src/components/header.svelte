<script>
	import links from '../data/links.json';
	import Drawer from './drawer.svelte';
</script>

<div class="wrapper">
	<header>
		<div>
			<a href="/" class="cancel-background">
				<img src="/la-cena-logo.svg" alt="La Cena Logo" />
			</a>
		</div>

		<div>
			<nav>
				<ul>
					{#each links as link}
						<li>
							<a href={link.url} title={link.title}>
								{link.title}
							</a>
						</li>
					{/each}
				</ul>
			</nav>
		</div>
	</header>
</div>

<Drawer />

<style lang="scss">
	.wrapper {
		background: $background;
	}

	header {
		padding: 0.75rem;

		@media screen and (min-width: $breakpoint) {
			padding: 2rem;
		}
	}

	header,
	nav {
		ul {
			display: flex;
			flex-direction: row;
			gap: 1.5rem;
			padding-left: 0;
			list-style: none;
			font-family: $header-font;
			font-size: 1.2rem;

			@media screen and (max-width: $breakpoint) {
				display: none;
			}
		}

		max-width: $max-width;
		margin: 0 auto;
	}
</style>
