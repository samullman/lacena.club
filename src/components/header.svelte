<script>
	import links from '../data/links.json';
	import Drawer from './drawer.svelte';
</script>

<div class="wrapper">
	<header>
		<div class="title">
			<a href="/" class="cancel-background">
				<img src="/la-cena-logo-alt.svg" alt="La Cena Logo" />
			</a>

			<!-- <a href="/" class="cancel-background">
				lacena.club
			</a> -->
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
		// background: $background;
	}

	.title {
		font-weight: bold;
		font-family: $header-font;
		max-width: 280px;
		margin: 1rem 0;

		@media screen and (min-width: $breakpoint) {
			max-width: 400px;
			margin-bottom: 2rem;
			margin-top: 1rem;
		}

		a:hover {
			color: $red;
		}
	}

	header {
		padding: 1rem;

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
			font-family: $body-font;
			// font-family: Space Mono;
			font-size: 1.32rem;

			@media screen and (max-width: $breakpoint) {
				display: none;
			}
		}

		max-width: $max-width;
		margin: 0 auto;
	}
</style>
