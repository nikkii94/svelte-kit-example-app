<script>
	import Header from '../lib/Header.svelte';
</script>

<Header />

<main>
	<slot />
</main>

<footer>Made with SvelteKit 2021</footer>

<style>
	footer {
			text-align: center;
	}
</style>