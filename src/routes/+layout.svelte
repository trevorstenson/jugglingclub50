<script lang="ts">
	import favicon from '$lib/assets/favicon.svg';

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
	<title>SpinJam Juggling Event</title>
	<meta name="description" content="Join us for an exciting juggling event featuring amazing performers, workshops, and community fun!" />
</svelte:head>

<style>
	:global(body) {
		margin: 0;
		padding: 0;
		overflow-x: hidden;
		background-color: var(--theme-color, #000);
	}

	:global(html) {
		margin: 0;
		padding: 0;
		background-color: var(--theme-color, #000);
	}

	:global([data-sveltekit-preload-data]) {
		margin: 0;
		padding: 0;
		background-color: var(--theme-color, #000);
	}

	:global([data-sveltekit-preload-data] > div) {
		margin: 0;
		padding: 0;
		background-color: var(--theme-color, #000);
	}
</style>

{@render children()}
