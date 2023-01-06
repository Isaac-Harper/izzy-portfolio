<script>
	import Star from '$lib/Star.svelte';
</script>

<svelte:head>
	<style>
		body {
			background: var(--background-teaching);
		}
	</style>
</svelte:head>
<img class="background" src="/artwork/1.png" alt="bench" />

<h2>Statement about teaching</h2>

<div class="center">
	<div class="interests">
		<a href="/Works" class="box"> art lesson plans <br /> & <br /> experience </a>
		<a href="/Teaching" class="box"> teaching philosophy </a>
		<a href="/About" class="box">
			jewish education lesson <br /> plans <br /> & <br /> experience
		</a>
		<a href="/Contact" class="box">
			outdoor education lesson <br /> plans <br /> & <br /> experience
		</a>
	</div>

	<Star />
</div>

<style>
	.background {
		object-fit: cover;
		height: 100%;
		width: 100%;
		background-color: black;
		max-width: 70rem;
	}

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
