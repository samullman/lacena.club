<script>
	/** @type {import('./$types').PageData} */
	export let data;
	import persons from '../../../data/persons.json';
	const key = data.slug;
	const { name, bio } = persons[key];
</script>

<div class="h1-wrapper">
	<h1>{name}</h1>
</div>

<div class="page">
	<p>
		{bio}
	</p>
</div>

<style lang="scss">
</style>
