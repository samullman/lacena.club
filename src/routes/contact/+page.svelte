<script>
	import EmailCapture from '../../components/email-capture.svelte';

	const socials = [
		{
			title: 'Calendly',
			target: 'https://www.calendly.com/samullman/',
			image: '/calendly.png'
		}
	];

	function handleSubmit(e) {
		e.preventDefault();
		var status = document.querySelectorAll('.status')[0];
		var data = new FormData(e.target);
		fetch(e.target.action, {
			method: 'POST',
			body: data,
			headers: {
				Accept: 'application/json'
			}
		})
			.then((response) => {
				if (response.ok) {
					debugger;
					status.innerHTML = 'Thanks for your submission!';
					document.querySelectorAll('form')[0].reset();
				} else {
					response.json().then((data) => {
						if (Object.hasOwn(data, 'errors')) {
							debugger;
							status.innerHTML = data['errors'].map((error) => error['message']).join(', ');
						} else {
							debugger;
							status.innerHTML = 'Oops! There was a problem submitting your form';
						}
					});
				}
			})
			.catch((error) => {
				debugger;
				status.innerHTML = 'Oops! There was a problem submitting your form';
			});
	}
</script>

<svelte:head>
	<title>Contact | Massive</title>
	<meta name="description" content="Humans coming together." />
</svelte:head>

<div class="h1-wrapper">
	<h1>Contact</h1>
</div>

<div class="page">
	<p>
		Lorem ipsum ipsum lorem
		<a href="https://www.calendly.com/samullman/meeting" target="_blank">Calendly</a>.
	</p>

	<br />

	<div class="grid">
		<form
			class="form"
			action="https://formspree.io/f/mqknbjry"
			method="POST"
			on:submit={handleSubmit}
		>
			<div>
				<label for="name">Name</label>
				<input name="name" required />
			</div>

			<div>
				<label for="email">Email</label>
				<input type="email" name="name" required />
			</div>

			<div>
				<label for="phone">Phone</label>
				<input type="tel" name="name" />
			</div>

			<div>
				<label for="organization">Organization</label>
				<input name="organization" />
			</div>

			<div>
				<label for="message">Message</label>
				<textarea name="message" rows="5" />
			</div>

			<div>
				<button type="submit"> Submit </button>
			</div>
		</form>

		<br />

		<div class="status" />
	</div>
</div>

<EmailCapture />

<!-- <div class="logo-grid">
	{#each socials as item}
		<a class="cancel-background" href={item.target} target="_blank">
			<img src={item.image} alt={item.title} />
		</a>
	{/each}
</div> -->
<style lang="scss">
	label {
		display: block;
		font-size: 0.9rem;
		margin-bottom: 0.25rem;
	}

	.form {
		display: flex;
		flex-direction: column;
		gap: 1rem;
	}

	select {
		max-width: 10rem;
	}

	input,
	textarea {
		width: 100%;
		font-family: Space Mono;
		font-size: 1.3rem;
		padding: 0.2rem 0.5rem;
	}

	input {
		max-width: 20rem;
	}

	textarea {
		max-width: 90%;
	}

	.logo-grid {
		display: flex;
		flex-wrap: wrap;
		gap: 2rem;

		img {
			@media screen and (max-width: 500px) {
				max-width: 100px;
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
</style>
