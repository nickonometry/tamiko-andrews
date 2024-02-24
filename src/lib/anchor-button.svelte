<script>
	export let buttonText;
	export let link;
	export let linkTarget;
</script>

<a href={link} class="btn" target={linkTarget}>
	<svg width="277" height="62">
		<defs>
			<linearGradient id="grad1">
				<stop offset="0%" stop-color="#FF8282" />
				<stop offset="100%" stop-color="#E178ED" />
			</linearGradient>
		</defs>
		<rect x="5" y="5" rx="25" fill="none" stroke="url(#grad1)" width="266" height="50"></rect>
	</svg>
	<span>{buttonText}</span>
</a>

<style>
	.btn {
		position: relative;
		display: inline-block;
		width: 277px;
		height: 50px;
		font-size: 1em;
		font-weight: bold;
		line-height: 60px;
		text-align: center;
		text-transform: uppercase;
		background-color: transparent;
		cursor: pointer;
		text-decoration: none;
		font-size: 18px;
		letter-spacing: 0.045em;
		color: #847d75;
	}

	.btn svg {
		position: absolute;
		top: 0;
		left: 0;
	}

	.btn svg rect {
		stroke: #d4d1cd;
		stroke-width: 4;
		stroke-dasharray: 353, 0;
		stroke-dashoffset: 0;
		-webkit-transition: all 600ms ease;
		transition: all 600ms ease;
	}

	.btn span {
		background: linear-gradient(to right, #d4d1cd, #e8e3df);
		background: -moz-linear-gradient(left, #d4d1cd 50%, #e8e3df 100%);
		background: -webkit-linear-gradient(left, #d4d1cd 50%, #e8e3df 100%);
		background: linear-gradient(to right, #d4d1cd 50%, #e8e3df 100%);

		-webkit-background-clip: text;
	}

	.btn:hover svg rect {
		stroke-width: 4;
		stroke-dasharray: 196, 543;
		stroke-dashoffset: 437;
	}
</style>
