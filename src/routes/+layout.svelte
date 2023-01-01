<script>
	import Footer from '$lib/Footer.svelte';
	import Header from '$lib/Header.svelte';
</script>

<svelte:head>
	<link rel="stylesheet" href="/css/reset.css" />
</svelte:head>

<Header />

<slot />

<Footer />
