<script>
	import Image from './Image.svelte';
	import Machine from './grieggarden.png?w=640;1280;2560;3840&format=avif;webp;png&picture';
</script>

<div class="hero">
	<h1>Sonat fagdag</h1>
	<strong>28. oktober 2022<br/>Svelte & Svelte kit</strong>
	<Image
		src={Machine}
		alt="The Svelte compiler packaging up your component code"
		--max-height="65vh"
	/>
	<!-- <img alt="Svelte logotype" class="logotype" src={SvelteLogotype} /> -->
</div>

<style>
	.hero {
		position: relative;
		background: radial-gradient(circle at 40% 30%, rgb(235, 243, 249), rgb(214, 222, 228));
	}

	h1 {
		font-size: 6rem;
		font-weight: 600;
	}

	strong {
		position: absolute;
		font-size: min(4vw, var(--h3));
		max-width: 10em;
		text-transform: uppercase;
		font-weight: 700;
		color: var(--back);
		letter-spacing: 0.05em;
		left: max(var(--side-nav), 10%);
		top: 25%;
		text-shadow: 0 0 10px black;
	}

	@media (min-width: 580px) {
		strong {
			max-width: 12em;
			top: 30%;
		}
	}

	@media (min-width: 800px) {
		h1 {
			position: absolute;
			display: block;

			bottom: 58%;
			left: 10%;
		}

		strong {
			max-width: 16em;
			top: 45%;
		}

		h1,
		strong {
			left: calc(var(--side-nav) + 4rem);
			color:var(--back);
			text-shadow: 0 0 1rem black;
			/* left: calc(50% - 56rem + var(--side-nav)); */
		}
	}

	@media (min-width: 1200px) {
		strong,
		h1 {
			left: calc(50% - 56rem + var(--side-nav));
			text-shadow: 0 0 10px black;
		}
	}
</style>
