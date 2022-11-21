<script>
	import LazyImage from '../../components/lazy-image.svelte';
</script>

<svelte:head>
	<title>About</title>
	<meta name="description" content="Humans coming together." />
</svelte:head>

<div class="h1-wrapper">
	<h1>Our Story</h1>
</div>

<div class="page">
	<p class="title">Born out of the desire to break bread.</p>

	<p class="title">
		We're exploding throughout the world to bring the best vibes available to dinner goers
		everywhere.
	</p>

	<p>We love food – and know the power of bringing people together.</p>

	<LazyImage src="/dinner-ppl.jpeg" alt="Dinner People" />

	<p>Let's to meet and have a conversation over a bottle of wine and beef bourguignon.</p>

	<p>See you next time,</p>

	<p>La Cena Team</p>
</div>

<style lang="scss">
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
