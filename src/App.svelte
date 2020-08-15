<script>
	export let name;
  import Tailwind from './Tailwind.svelte'
</script>

<Tailwind />

<main>
	<h1>Hello {name}!</h1>
	<p>Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn how to build Svelte apps.</p>
  <p class="tailwind">Now with Tailwind!</p>
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

  .tailwind {
    @apply text-3xl bg-red-500;
  }

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>
