<svelte:head>
	<style>
		body {
			background: var(--background-works);
		}
	</style>
</svelte:head>

<div class="container">
	<h2>Photography</h2>

	<div class="examples">
		<div class="box">a</div>
		<div class="box">a</div>
		<div class="box">a</div>
	</div>
</div>

<style>
	.container {
		width: 100%;
		padding: 1rem;
		max-width: 50rem;
	}

	.examples {
		display: flex;
		gap: 2rem;
		flex-direction: column;
	}

	.box {
		background-color: lightgreen;
		aspect-ratio: 3 / 1;
		border-radius: 2rem;
		padding: 1rem;
	}
</style>
