<div class="contact-container">
	<div class="grid">
		<!-- <img src="/contact-image.jpeg" alt="Tamiko Andrews in a photo shoot session" /> -->
		<div class="form-container">
			<p style="margin: 0;">For an estimate or professional evaluation of your project, please fill out the form below.</p>
			<form name="netlify-form-example" method="POST" netlify-honeypot="bot-field" data-netlify="true" netlify>
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
					<label for="address">Address</label>
					<textarea name="address" id="address" type="text" />
				</div>
				<div class="input-container">
					<label for="project">Project Details</label>
					<textarea name="project" id="project" type="text" />
				</div>
				<input class="btnfos btnfos-5" type="submit" value="Submit" />
			</form>
		</div>
	</div>
</div>

<style>
	.contact-container {
		max-width: 1440px;
		width: 100%;
		margin: 0 auto;
	}
	.grid {
		display: grid;
		grid-template-columns: 5fr 5fr;
		gap: 64px;
		padding: 24px;
	}

	@media (max-width: 900px) {
		.grid {
			grid-template-columns: 1fr;
			gap: 24px;
		}
	}

	.form-container {
		display: grid;
		gap: 24px;
	}

	form {
		display: grid;
		gap: 24px;
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
</style>
