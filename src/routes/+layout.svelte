<script>
	import '../app.css';
	import favicon from '$lib/assets/favicon.svg';

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

<nav>
	<div class="bg-blue-500 h-8"></div>
	<a href="/">home</a>
	<a href="/missions">missions and activities</a>
</nav>

<main>
	{@render children?.()}
</main>

<footer>
	footer
</footer>
