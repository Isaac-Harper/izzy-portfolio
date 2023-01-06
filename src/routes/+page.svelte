<script>
	import Options from '$lib/Options.svelte';

	const titles = ['art making', 'teaching', 'about me // resume', 'contact me'];
	const links = ['/works', '/Teaching', '/About', '/Contact'];
</script>

<svelte:head>
	<style>
		body {
			background: var(--background-home);
		}
	</style>
</svelte:head>

<img class="background" src="/artwork/CactusAnts.jpeg" alt="bench" />

<Options {titles} {links} />

<style>
	.background {
		object-fit: cover;
		height: 100%;
		width: 100%;
		background-color: black;
		max-width: 70rem;
	}
</style>
