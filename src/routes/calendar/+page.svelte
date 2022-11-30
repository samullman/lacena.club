<script>
	import LazyImage from '../../components/lazy-image.svelte';
	import EmailCapture from '../../components/email-capture.svelte';
</script>

<svelte:head>
	<title>Calendar</title>
	<meta name="description" content="Humans coming together." />
</svelte:head>

<div class="h1-wrapper">
	<h1>Calendar</h1>
</div>

<div class="page">
	<h2>Coming soon...</h2>
	<!-- 
	<ul>
		<li>
			<a href="/event/de-nada-11-11-22"> De Nada</a> Austin, TX (12/12/22)
		</li>

		<li>
			<a href="/event/de-nada"> Launderette</a> Austin, TX (12/04/22)
		</li>
	</ul>

	<h2>November</h2>

	<ul>
		<li>
			<s>
				<a href="/event/de-nada"> Kemuri Tatsu-Ya</a> Austin, TX (12/04/22)
			</s>
		</li>
	</ul> -->
</div>

<EmailCapture />

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
