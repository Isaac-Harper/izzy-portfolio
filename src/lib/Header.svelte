<script>
	import NavButton from './NavButton.svelte';
	import BigStar from './BigStar.svelte';
	import LittleStar from './LittleStar.svelte';
</script>

<div class="header">
	<a href="/">
		<h1>ISABELLE YOUNG</h1>
	</a>
	<div class="space" />
	<div class="star">
		<BigStar />
		<LittleStar />
	</div>
</div>

<style>
	.header {
		position: sticky;
		top: 0;

		display: flex;
		align-items: center;

		padding: 1rem;
		gap: 1rem;

		background-color: #f4eae7;
	}

	.space {
		flex: 1;
	}

	.star {
		position: relative;
	}

	a {
		text-decoration: none;
		color: black;
	}
</style>
