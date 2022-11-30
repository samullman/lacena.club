<div class="wrapper">
	<img transition:spin src="/flower.png" />
</div>

<style lang="scss">
	.wrapper {
		background: #f5efe655;
		backdrop-filter: blur(4px);
		animation: spin 10s linear infinite;
		position: fixed;
		top: -2.5rem;
		left: -2.5rem;
		width: 8rem;
		height: 8rem;
		border-radius: 50%;
		padding: 0.5rem;
		display: none;
		z-index: 1;

		@media screen and (min-width: 60rem) {
			display: block;
			top: -2.5rem;
			left: -2.5rem;
			width: 8rem;
			height: 8rem;
		}

		text-align: center;

		img {
		}
	}

	@keyframes spin {
		from {
			transform: rotate(0deg);
		}
		to {
			transform: rotate(360deg);
		}
	}
</style>
