<script>
	import LazyImage from '../../components/lazy-image.svelte';
	import EmailCapture from '../../components/email-capture.svelte';
</script>

<svelte:head>
	<title>Story</title>
	<meta name="description" content="Humans coming together." />
</svelte:head>

<div class="h1-wrapper">
	<h1>Our story</h1>
</div>

<div class="page">
	<p>We decided post-pandemic to start a dinner club. With all the comotion</p>

	<p>And where do the best memories happen? At the dinner table of course!</p>

	<p>
		La Cena ("The Dinner") Club was born out of the desire to break bread with fresh company in the
		Austin area.
	</p>

	<p>We believe amazing things happen when great people get together over delicious food.</p>

	<p>
		This is your opportunity to experience unique, full-course meals in a socially driven
		environment at some of Austin's top culinary destinations.
	</p>

	<p>Hope to see you soon.</p>

	<a href="/calendar">
		<button> Calendar </button>
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

<EmailCapture />

<style lang="scss">
</style>
