<script>
	import Options from '$lib/Options.svelte';

	const titles = ['art making', 'teaching', 'about me // resume', 'contact me'];
	const links = ['/works', '/Teaching', '/About', '/Contact'];
</script>

<img class="background" src="/artwork/CactusAnts.jpeg" alt="bench" />

<Options {titles} {links} />

<style>
	:global(body) {
		background-color: blue;
	}
	.background {
		object-fit: cover;
		height: 100%;
		width: 100%;
		background-color: black;
	}
</style>
