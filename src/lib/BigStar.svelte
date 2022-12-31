<script>
	let hue = Math.floor(Math.random() * 360);

	setInterval(() => {
		hue++;
	}, 50);
</script>

<div class="five-pointed-star" style="--star-color:hsl({hue}, 50%, 50%);" />

<style>
	.five-pointed-star {
		position: absolute;
		top: 0.5rem;
		left: 0.5rem;
		--star-color: orange;
		font-size: 2em;
		position: relative;
		display: block;
		width: 0px;
		height: 0px;
		border-right: 1em solid transparent;
		border-bottom: 0.7em solid var(--star-color);
		border-left: 1em solid transparent;
		transform: rotate(15deg);
	}
	.five-pointed-star:before {
		border-bottom: 0.8em solid var(--star-color);
		border-left: 0.3em solid transparent;
		border-right: 0.3em solid transparent;
		position: absolute;
		height: 0;
		width: 0;
		top: -0.45em;
		left: -0.65em;
		display: block;
		content: '';
		transform: rotate(-35deg);
	}
	.five-pointed-star:after {
		position: absolute;
		display: block;
		top: 0.03em;
		left: -1.05em;
		width: 0;
		height: 0;
		border-right: 1em solid transparent;
		border-bottom: 0.7em solid var(--star-color);
		border-left: 1em solid transparent;
		transform: rotate(-70deg);
		content: '';
	}
</style>
