<script lang="ts">
	import Header from '$lib/header/Header.svelte';
	import '../app.css';
</script>

<Header />

<main>
	<slot />
</main>

<footer>
	<!--<a href="https://www.youtube.com/watch?v=kcC8JW_Rppo" target="_blank" rel="noopener">a Isiah Lloyd production</a>-->
	<a href="https://isiah.me" target="_blank" rel="noopener">by isiah</a><span>&nbsp;|&nbsp;</span><a href="https://github.com/isiah-lloyd/radiyo-website" target="_blank" rel="noopener">website src</a>
</footer>

<style>
	footer {
		text-align: center;
		font-size: 1em;
	}


</style>
