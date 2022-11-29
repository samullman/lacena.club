<script>
	import LazyImage from '../../components/lazy-image.svelte';
</script>

<svelte:head>
	<title>Story</title>
	<meta name="description" content="Humans coming together." />
</svelte:head>

<div class="h1-wrapper">
	<h1>Our story</h1>
</div>

<div class="page">
	
	<p>La Cena ("The Dinner") Club was born out of the desire to break bread with fresh company in the Austin area.</p>

	<p>
		We believe amazing things happen when great people get together over delicious food.
	</p>

	<p>
		This is your opportunity to experience unique, full-course meals in a socially driven environment at some of Austin's top culinary destinations. 
	</p>

	<p>
		Hope to see you soon. 
	</p>

	<a href="/calendar">
		<button>
			Calendar
		</button>
	</a>

	<!-- <p>We're setting up unique opportunities to dine at some of Austin's finest culinary destinations.

		This is a unique opportunity to bring humans human together and share time over an amazing
		dinner and company.</p>

	<p>
		What better way to get together than over a curated, one-time multiple course meal at some of
		the best dining establishments in Texas. Tickets are available on a first come first serve basis
		and available to all.
	</p>

	<p>
		We believe great things happen when we get together over an amazing meal. love food – and know
		the power of bringing people together.
	</p> -->
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
