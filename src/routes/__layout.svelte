<script lang="ts">
	import Header from '$lib/header/Header.svelte';
	import '../app.css';
</script>

<Header />

<main>
	<slot />
</main>

<footer>
	<a href="https://getyarn.io/yarn-story/7f0308cc-7923-4eda-8b24-cc6731eb0808" target="_blank">a Isiah Lloyd production</a>
</footer>

<style>
	footer {
		text-align: center;
		font-size: x-small;
	}
	footer > a {
	}

</style>
