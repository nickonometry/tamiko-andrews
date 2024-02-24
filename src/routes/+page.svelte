<script>
	import AnchorButton from '../lib/anchor-button.svelte';
</script>

<main>
	<div class="mobile-image"></div>
	<div class="grid-container">
		<div class="bg-box">
			<div class="image">
				<img src="tamiko1.jpeg" alt="Tamiko photoshoot" />
			</div>
		</div>
		<div class="about">
			<h1>Hi! I'm Tamiko Andrews</h1>
			<p>
				Meet Tamiko Andrews, an accomplished hairstylist with eight years of expertise, focusing on precision haircuts and elegant up styles. She currently thrives at House of J Henry in Portland,
				Maine, where her talent and passion for hairstyling shine through every client she touches.
			</p>
			<p>
				Originally from Lewiston, Maine, Tamiko now resides in the picturesque coastal town of Old Orchard Beach with her husband, Nick, and their loyal companion, Harley, their beloved dog. When
				she's not creating stunning looks at the salon, you'll likely find Tamiko spending leisurely mornings with brides, making them feel radiant on their special day.
			</p>
			<p>
				Beyond her artistic pursuits, Tamiko embraces the outdoors with enthusiasm, whether she's carving through snow-covered slopes while skiing, soaking up the sun on the beach, or gliding
				peacefully across the water on her paddleboard. With her dedication to her craft and zest for life, Tamiko Andrews embodies the true essence of beauty and adventure.
			</p>
			<div class="button-container">
				<AnchorButton buttonText="View my work" link="http://www.instagram.com/tandrews_style" linkTarget="_blank" />
				<AnchorButton buttonText="Contact me" link="/contact" linkTarget="" />
			</div>
		</div>
	</div>
</main>

<style>
	main {
		height: 100dvh;
		padding: 0;
		margin: 0;
		display: grid;
		grid-template-rows: 1fr;
		place-content: center;
	}

	@media screen and (max-width: 960px) {
		main {
			display: grid;
			grid-template-rows: 300px 1fr;
			place-content: start;
		}
	}
	h1 {
		font-size: 56px;
		padding: 0;
		margin: 0;
	}

	.mobile-image {
		display: none;
	}

	.grid-container {
		width: 100%;
		max-width: 1920px;
		display: grid;
		grid-template-columns: 4fr 8fr;
		gap: 64px;
		padding: 16px;
		align-items: center;
	}

	.bg-box {
		position: relative;
		overflow: visible;
		max-height: 500px;
		max-width: 500px;
		width: 100%;
		height: 100%;
		background: #e8e3df;
		background: -webkit-linear-gradient(to right, #d4d1cd, #e8e3df);
		background: linear-gradient(to right, #d4d1cd, #e8e3df);
		z-index: 1;
	}

	.image {
		position: absolute;
		max-height: 500px;
		max-width: 500px;
		width: 100%;
		height: 100%;
		left: 50px;
		bottom: 50px;
	}

	.image img {
		width: 100%;
		height: 500px;
		object-fit: cover;
	}

	.about {
		z-index: 2;
	}

	.button-container {
		width: 100%;
		display: flex;
		flex-wrap: wrap;
		gap: 24px;
		align-items: center;
		justify-content: center;
	}

	@media screen and (max-width: 960px) {
		h1 {
			text-align: center;
			font-size: 36px;
		}

		.mobile-image {
			display: block;
			width: 100%;
			background-image: url(/tamiko1.jpeg);
			background-size: cover;
			background-position-y: 33%;
		}
		.grid-container {
			grid-template-columns: 1fr;
			align-items: start;
		}

		.about {
			padding: 24px;
		}

		.bg-box {
			display: none;
		}
		.image {
			display: none;
		}

		.button-container {
		}
	}
</style>
