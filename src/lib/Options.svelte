<script>
	import Star from '$lib/Star.svelte';

	export let titles = ['one', 'two', 'three', 'four'];
	export let links = ['/', '/', '/', '/'];
</script>

<div class="interests">
	{#each titles as title, i}
		<a href={links[i]} class="box">{title}</a>
	{/each}
</div>

<style>
	.interests {
		display: grid;
		grid-template-columns: 1fr 1fr;
		grid-template-rows: 1fr 1fr;

		justify-items: center;
		align-items: center;
		gap: 2rem;
		padding: 2rem;
		width: 100%;
		max-width: 50rem;

		flex: 1;
	}

	.box {
		width: 100%;
		aspect-ratio: 1 / 1;
		background-color: #d3bfc8;
		display: flex;
		align-items: center;
		justify-content: center;
		border-radius: 2rem;

		text-decoration: none;
		color: black;
		white-space: pre-line;
		text-align: center;
	}

	.box:visited {
		background-color: hsla(333, 18.5%, 73.8%, 1);
	}

	.box::after {
		content: '';
		border-radius: 2rem;
		box-shadow: 0 0 2rem rgba(0, 0, 0, 0.8);
		opacity: 0;
		transition: all 0.6s cubic-bezier(0.1, 0.8, 0.4, 1);
	}

	.box:hover {
		border: solid #f4eae7;
	}

	.box:hover::after {
		opacity: 1;
	}
</style>
