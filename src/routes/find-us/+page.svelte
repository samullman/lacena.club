<script>
	import LazyImage from '../../components/lazy-image.svelte';
</script>

<svelte:head>
	<title>Find Us</title>
	<meta name="description" content="Humans coming together." />
</svelte:head>

<div class="h1-wrapper">
	<h1>Find Us</h1>
</div>

<div class="page">
	<h3>Book with your favorite platform below:</h3>
	<ul>
		<li>Eventbrite</li>

		<li>Meetup.com</li>

		<li>Foursquare</li>
	</ul>

	<br />

	<LazyImage src="/sunset.png" alt="Sunset" />

	<br />

	<p class="title">
		<a href="/contact" title="Contact">Contact</a>.
	</p>

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
