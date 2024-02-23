<script>
	import '../app.css';
</script>

<main>
	<slot />
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
</style>
