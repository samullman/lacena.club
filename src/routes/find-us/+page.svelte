<script>
	import LazyImage from '../../components/lazy-image.svelte';
</script>

<svelte:head>
	<title>Find us</title>
	<meta name="description" content="Humans coming together." />
</svelte:head>

<div class="h1-wrapper">
	<h1>Find us</h1>
</div>

<div class="page">
	<h2>Stay in touch!</h2>
	<ul>
		<li>
			<a href="https://meetup.com/" target="_blank"> Meetup.com </a>
		</li>

		<li>
			<a href="https://eventbrite.com/" target="_blank"> Eventbrite </a>
		</li>

		<li>
			<a href="https://instagram.com/lacenaclub" target="_blank"> Instagram </a>
		</li>
	</ul>

	<br />
</div>

<style lang="scss">
	p {
		font-size: 1.1rem;
	}

	.logo-grid {
		display: flex;
		flex-wrap: wrap;
		gap: 2rem;

		img {
			@media screen and (max-width: $breakpoint) {
				max-width: 50px;
			}

			@media screen and (min-width: $breakpoint) {
				max-width: 80px;
			}

			cursor: pointer;
			transition: all 0.2s ease;
			object-fit: contain;

			&:hover {
				transform: scale(1.04);
				opacity: 0.9;
			}

			&:active {
				transform: scale(0.94);
				opacity: 1;
			}
		}
	}

	.breaker-img {
		max-height: 400px;
		max-width: 800px;
		margin: 2rem auto;
		display: block;
	}

	.profile-img {
		text-align: center;

		img {
			width: 10rem;
			height: 10rem;
			border-radius: 50%;
		}
	}
</style>
