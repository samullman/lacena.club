<script>
	function handleSubmit(e) {
		e.preventDefault();
	}
</script>

<div class="email-wrapper">
	<div class="nest">
		<h2>Subscribe!</h2>

		<form class="email-capture" on:submit={handleSubmit}>
			<input placeholder="example@gmail.com" type="email" required />

			<button> Submit </button>
		</form>
	</div>
</div>

<style lang="scss">
	input,
	textarea {
		width: 100%;
		font-family: Space Mono;
		font-size: 1.1rem;
		padding: 0.2rem 0.5rem;
		background: $off-white;
		width: 20rem;
		border-radius: 0.25rem;
	}

	.email-wrapper {
		background: $red;

		.nest {
			padding: 1rem;
			max-width: $max-width;
			margin: 1rem auto;

			@media screen and (min-width: $breakpoint) {
				margin: 2rem auto;
			}
		}

		h2 {
			font-style: italic;
			color: $dark-white;
			font-size: 2rem;
			margin-top: 0;
			font-family: $header-font;

			@media screen and (min-width: $breakpoint) {
				font-size: 2.4rem;
			}
		}

		.email-capture {
			display: flex;
			flex-wrap: wrap;
			gap: 1rem;
		}
	}
</style>
