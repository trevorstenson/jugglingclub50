<script lang="ts">
	import favicon from '$lib/assets/favicon.svg';

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
	<link rel="preconnect" href="https://fonts.googleapis.com" />
	<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin="anonymous" />
	<link
		href="https://fonts.googleapis.com/css2?family=Outfit:wght@400;600;700&display=swap"
		rel="stylesheet"
	/>
	<title>BJF: Boston Juggling and Flow</title>
	<meta
		name="description"
		content="BJF: Boston Juggling and Flow — celebrating the MIT Juggling Club's 50th and Boston Spinjam's 20th anniversary. Free admission, April 4, 2026 at MIT."
	/>
</svelte:head>

<style>
	:global(body) {
		margin: 0;
		padding: 0;
		overflow-x: hidden;
		background-color: #1A3A5C;
		font-family: 'Outfit', system-ui, -apple-system, sans-serif;
		line-height: 1.6;
		-webkit-font-smoothing: antialiased;
		-moz-osx-font-smoothing: grayscale;
	}

	:global(html) {
		margin: 0;
		padding: 0;
		background-color: #1A3A5C;
	}

	:global(*) {
		box-sizing: border-box;
	}

	:global([data-sveltekit-preload-data]) {
		margin: 0;
		padding: 0;
		background-color: #1A3A5C;
	}

	:global([data-sveltekit-preload-data] > div) {
		margin: 0;
		padding: 0;
		background-color: #1A3A5C;
	}
</style>

{@render children()}
