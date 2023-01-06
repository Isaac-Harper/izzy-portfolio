<svelte:head>
	<style>
		body {
			background: var(--background-contact);
		}
	</style>
</svelte:head>

<div class="box">
	<div class="container">
		<div class="contact">
			<h2>Contact me!</h2>
			<p>
				I teach visual art in all contexts: birthday parties for all ages, non-profits, camps,
				school events and field trips, and much more!
			</p>
			<p>Tucson, AZ</p>
			<p>iry@email.arizona.edu</p>
		</div>
		<img src="/portrait.jpg" alt="portrait" />
		<form>
			<label for="name">Name</label>
			<input type="text" />
			<label for="email">E-mail</label>
			<input type="email" name="email" id="email" required />
			<label for="phone">Phone</label>
			<input
				type="tel"
				id="phone"
				name="phone"
				pattern="[0-9]{3}-[0-9]{3}-[0-9]{4}"
				placeholder="123-4567-8901"
				required
			/>
			<label for="message">Message</label>
			<textarea name="message" id="message" cols="20" rows="5" class="message" maxlength="120" />
			<button type="submit">submit</button>
		</form>
	</div>
</div>

<style>
	form {
		display: grid;
		grid-template-columns: 2fr 8fr;
		align-items: center;
		justify-content: center;
		column-gap: 1rem;
		row-gap: 0.5rem;
		max-width: 20rem;
		background-color: #05878a;
		padding: 2rem;
		border-radius: 2rem;
		grid-area: form;
	}

	.message {
		max-width: 14rem;
	}
	.container {
		background-color: #dd9933;
		padding: 2rem;
		border-radius: 2rem;
		max-width: 70rem;

		display: grid;

		grid-template-areas:
			'info photo'
			'form photo';
		gap: 2rem;
	}

	.box {
		display: flex;
		justify-content: center;
	}

	.contact {
		background-color: #e52a6f;
		padding: 2rem;
		border-radius: 2rem;
		max-width: 20rem;
		grid-area: info;
	}

	img {
		grid-area: photo;
		border-radius: 2rem;
		object-fit: cover;
	}
</style>
