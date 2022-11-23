<script>
	/** @type {import('./$types').PageData} */
	export let data;
	import events from '../../../data/events.json';
	const key = data.slug;
	const { title, website, place, about, seats } = events.find((el) => el.slug === key);
</script>

<div class="h1-wrapper">
	<h1>{title}</h1>
</div>

<div class="page">
	<p>
		Seats: {seats}
	</p>

	<p>
		About: {about}
	</p>
	<a href={website} target="_blank">
		<button>
			Website
		</button>
	</a>

	<a href={place} target="_blank">
	<button>
			Directions
		</button>
	</a>
</div>

<style lang="scss">
</style>
