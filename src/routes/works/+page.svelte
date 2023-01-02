<script>
	import Options from '$lib/Options.svelte';

	const titles = [
		'ink & charcoal',
		'graphic design \n illustration \n digital work',
		'3D works',
		'Photography'
	];
	const links = ['/works/inkcharcoal', '/works/digital', '/works/3d', '/works/photography'];
</script>

<img class="background" src="/artwork/11.png" alt="bench" />

<h2>Statement about art making</h2>

<Options {titles} {links} />

<style>
	:root {
		background-color: green;
	}

	.background {
		object-fit: cover;
		width: 100%;
		background-color: black;
	}
</style>
