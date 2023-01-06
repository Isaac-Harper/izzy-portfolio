<script>
	import Footer from '$lib/Footer.svelte';
	import Header from '$lib/Header.svelte';
</script>

<svelte:head>
	<link rel="stylesheet" href="/css/reset.css" />
</svelte:head>

<Header />
<div class="container">
	<slot />
</div>

<Footer />

<style>
	.container {
		display: flex;
		justify-content: center;
		align-items: center;
		flex-direction: column;
	}
</style>
