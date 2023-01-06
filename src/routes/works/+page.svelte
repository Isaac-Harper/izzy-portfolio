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

<svelte:head>
	<style>
		body {
			background: var(--background-works);
		}
	</style>
</svelte:head>

<img class="background" src="/artwork/11.png" alt="bench" />

<h2>Statement about art making</h2>

<Options {titles} {links} />

<style>
	.background {
		object-fit: cover;
		width: 100%;
		background-color: black;
		max-width: 70rem;
	}
</style>
