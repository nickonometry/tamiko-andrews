<div class="contact-container">
	<form name="netlify-form-example" method="POST" netlify-honeypot="bot-field" data-netlify="true" netlify>
		<p style="margin: 0;">I'd love to work at your wedding! Please fill out the form below and we can discuss the details further. Hope to hear from you soon.</p>
		<input type="hidden" name="form-name" value="netlify-form-example" />
		<div class="input-container">
			<label for="name">Name</label>
			<input name="name" id="name" required type="text" />
		</div>
		<div class="input-container">
			<label for="email">Email</label>
			<input name="email" id="email" required type="email" />
		</div>
		<div class="input-container">
			<label for="phone">Phone number</label>
			<input name="phone" id="phone" required type="phone" />
		</div>
		<div class="input-container">
			<label for="wedding-date">Wedding Date</label>
			<input name="wedding-date" id="wedding-date" required type="date" />
		</div>
		<div class="input-container">
			<label for="project">Project Details</label>
			<textarea name="project" id="project" type="text" />
		</div>
		<input class="btn" type="submit" value="Submit" />
	</form>
</div>

<style>
	.contact-container {
		max-width: 1440px;
		width: 100%;
		height: 100%;
		width: 100%;
		margin: 0 auto;
		padding: 24px;
	}

	form {
		display: grid;
		gap: 24px;
		max-width: 768px;
		width: 100%;
		margin: 0 auto;
	}

	.input-container {
		display: grid;
		gap: 4px;
	}

	label {
		font-size: 0.95rem;
	}

	input {
		height: 56px;
		padding-inline: 16px;
	}

	textarea {
		height: 100px;
	}

	input[type='submit'] {
		display: grid;
		place-content: center;
		border: 4px solid #d4d1cd;
		border-radius: 64px;
		background-color: transparent;
		font-size: 18px;
		letter-spacing: 0.045em;
		color: #847d75;
		font-weight: 800;
		font-family: 'Playfair Display', serif;
	}
</style>
