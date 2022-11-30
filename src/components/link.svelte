<script>
	let url = true;
</script>

{#if true}
	<a href={url} />
{:else}
	<a href={url} target="_blank" rel="noopener noreferrer" />
{/if}
