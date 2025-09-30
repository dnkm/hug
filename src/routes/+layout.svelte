<script>
	import '../app.css';
	import favicon from '$lib/assets/favicon.svg';

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

<div class="min-h-screen flex flex-col">
	<nav>
		<div class="h-8 bg-primary"></div>
		<div class="container mx-auto flex justify-between py-4 text-lg">
			<div>LOGO</div>
			<a href="/">home</a>
			<a href="/missions">missions and activities</a>
			<a href="/">?</a>
			<a href="/">?</a>
			<a href="/">?</a>
			<button class="btn btn-accent">Join Us!</button>
		</div>
	</nav>

	<main class="flex-1">
		{@render children?.()}
	</main>

	<footer class="bg-primary text-primary-content h-[200px]">footer</footer>
</div>
