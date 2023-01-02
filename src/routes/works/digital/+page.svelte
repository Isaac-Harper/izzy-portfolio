<div class="outer">
	<div class="container">
		<div class="element" />

		<div class="element" />
	</div>
</div>

<style>
	.outer {
		display: flex;
		justify-content: center;
	}
	.container {
		max-width: 50rem;
		display: flex;
		flex-direction: column;
		gap: 2rem;
		width: 100%;
	}

	.element {
		background-color: violet;
		aspect-ratio: 2 / 1;
		border-radius: 2rem;
	}
</style>
