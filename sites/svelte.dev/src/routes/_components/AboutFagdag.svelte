<script>
  import Section from "@sveltejs/site-kit/components/Section.svelte";

</script>
<Section>
	<div class="boxcontainer">
		<div class="box">
			<h2>Gå til oppgavene</h2>
			<div class="topmargin">Oppgave 1 består av en tutorial som er kopiert og modifisert fra <a href="https://svelte.dev/tutorial" class="link">den offisielle Svelte Tutorial</a></div>
			<a class="button" href="/tutorial">Oppgave 1 - Tutorial</a>

			<div class="topmargin">I oppgave 2 skal dere få teste på en real world app</div>
			<a class="button" href="https://github.com/Sonat-Consulting/fagdag-bergen-svelte-chat-demo">Oppgave 2 - repo i Github</a>

		</div>
	</div>


</Section>

<style>

	.boxcontainer {
		display: grid;
	}

	.topmargin {
		margin-top: 1rem;
	}

	.box {
		padding: 1em;
		display: flex;
		flex-direction: column;
		border-bottom: none;
		color: var(--back);
		border-radius: var(--border-r);
		background: var(--prime);
	}

	.box :global(h2) {
		padding: 0;
		margin: 0 0 0.5em 0;
		font-size: var(--h2);
		font-weight: 300;
		color: white;

	}

	.box a.link {
		color: var(--back);
		text-decoration: underline;
	}

	.button {
		position: relative;
		max-width: 15em;
		padding: 0.8rem 1.6rem;
		border-radius: 4px;
		background: var(--back);
		border: 1px solid white;
		color: var(--second);
		font-size: var(--h6);
		text-decoration: none;
	}

	.button:hover {
		background: transparent;
		color: var(--back);
	}

	.button::after {
		content: '';
		position: absolute;
		display: block;
		right: 0.5em;
		top: 0em;
		width: 1em;
		height: 100%;
		background: url(arrow-right-black.svg);
		background-size: 100% 100%;
	}

</style>

