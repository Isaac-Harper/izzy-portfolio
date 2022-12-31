<script>
	import Star from '$lib/Star.svelte';
</script>

<div class="center">
	<div class="interests">
		<a href="/Works" class="box"> art making </a>
		<a href="/Teaching" class="box"> teaching </a>
		<a href="/About" class="box"> about me // resume </a>
		<a href="/Contact" class="box"> contact me </a>
	</div>

	<Star />
</div>

<style>
	.center {
		display: flex;
		justify-content: center;
		align-items: center;
		flex-direction: column;
	}
	.interests {
		display: grid;
		grid-template-columns: 1fr 1fr;
		grid-template-rows: 1fr 1fr;

		justify-items: center;
		align-items: center;
		gap: 1rem;
		padding: 2rem;
		width: 100%;
		max-width: 60rem;

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
