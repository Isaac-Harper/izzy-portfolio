<script>
	let hue = Math.floor(Math.random() * 360);

	setInterval(() => {
		hue++;
	}, 70);
</script>

<div class="outer">
	<div class="container" style="background-color:hsl({hue}, 30%, 50%); opacity: 100%">
		<img src="/instagram.svg" alt="insta" class="instagram" />
	</div>
</div>

<style>
	.outer {
		padding: 1rem;
		position: fixed;
		bottom: 0;
		left: 0;
		right: 0;
	}

	.container {
		color: white;
		height: 5rem;
		border-radius: 2rem;
		display: flex;
		justify-content: center;
		align-items: center;
	}

	.instagram {
		height: 2rem;
		width: 2rem;
	}
</style>
