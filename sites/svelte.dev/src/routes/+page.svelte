<script>
	import { Blurb } from '@sveltejs/site-kit';
	import Supporters from './_components/Supporters/index.svelte';
	import Hero from './_components/Hero.svelte';
	import Image from './_components/Image.svelte';
	import Demo from './_components/Demo.svelte';
	import WhosUsingSvelte from './_components/WhosUsingSvelte/index.svelte';
	import Balls from './svelte-balls.png?w=640;1280;2560;3840&format=avif;webp;png&picture';
  import AboutFagdag from './_components/AboutFagdag.svelte';
</script>

<svelte:head>
	<title>Svelte • Cybernetically enhanced web apps</title>

	<meta name="twitter:title" content="Svelte" />
	<meta name="twitter:description" content="Cybernetically enhanced web apps" />
	<meta name="Description" content="Cybernetically enhanced web apps" />
</svelte:head>

<h1 class="visually-hidden">Svelte</h1>

<Hero />

<div class="blurb-shifter">
	<AboutFagdag />
</div>

<Image src={Balls} alt="The Svelte logo in a ball pit" />

<footer>
	<!-- <a href="/tutorial">Tutorial</a>
	<a href="/docs">Docs</a>
	<a href="/examples">Examples</a>
	<a href="/blog">Blog</a>
	<a href="/faq">FAQ</a>
	<a href="https://opencollective.com/svelte">Open Collective</a> -->
	Have a nice day!
</footer>

<style>
	section {
		position: relative;
		margin: 10rem auto;
		padding: 0 var(--side-nav);
		max-width: 120rem;
	}

	.blurb-shifter {
		margin-top: calc(-10rem + var(--side-nav));
	}

	footer {
		display: flex;
		flex-wrap: wrap;
		justify-content: center;
		padding: 4rem;
	}

	footer a {
		color: var(--text);
		padding: 0.5rem 1rem;
		display: block;
	}

	@media (min-width: 900px) {
		.blurb-shifter {
			margin-top: -12em;
		}
	}
</style>
