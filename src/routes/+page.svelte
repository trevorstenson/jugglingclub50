<script lang="ts">
	import bostonSilhouette from '$lib/assets/boston_silhouette_transparent.png';

	const eventName = "MIT Juggling Club's 50th Anniversary";
</script>

<div class="page-container">
	<div
		class="skyline-layer"
		aria-hidden="true"
		style={`--skyline-image: url(${bostonSilhouette});`}
	></div>

	<div class="content-section">
		<header>
			<h1>{eventName}</h1>
		</header>
	</div>
</div>

<style>
	:global(:root) {
		--sky-color: linear-gradient(180deg, #f4e6d7 0%, #e5eef5 100%); /* warm beige to soft blue sky */
		--base-color: #1f2329; /* charcoal for buildings + content */
		--accent-primary: #a31f34; /* MIT red accent */
		--accent-muted: #8a8b8c; /* muted gray accent */
		--card-bg: #2a2f38;
		--card-border: #3a414c;
		--text-strong: #f6f7fb;
		--text-muted: #c8cdd6;
		--skyline-height: clamp(260px, 40vw, 460px);
	}

	.page-container {
		width: 100%;
		min-height: 100vh;
		margin: 0;
		padding: 0;
		display: flex;
		flex-direction: column;
		background-color: var(--base-color);
	}

	.skyline-layer {
		position: relative;
		width: 100%;
		height: var(--skyline-height);
		background: var(--sky-color);
	}

	.skyline-layer::after {
		content: '';
		position: absolute;
		inset: 0;
		background: var(--base-color);
		-webkit-mask-image: var(--skyline-image);
		mask-image: var(--skyline-image);
		-webkit-mask-size: cover;
		mask-size: cover;
		-webkit-mask-repeat: no-repeat;
		mask-repeat: no-repeat;
		-webkit-mask-position: center bottom;
		mask-position: center bottom;
	}

	.content-section {
		background-color: var(--base-color);
		color: var(--text-strong);
		width: 100%;
		min-height: 100vh;
		padding: 3rem 2rem;
		margin: 0;
		flex: 1;
		line-height: normal;
	}

	header {
		text-align: center;
		margin-bottom: 3rem;
	}

	h1 {
		font-size: 2.5rem;
		margin: 0;
		color: var(--text-strong);
	}

</style>
