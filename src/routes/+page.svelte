<script lang="ts">
	import bostonSilhouette from '$lib/assets/boston_silhouette_transparent.png';

	// Event information - to be customized later
	const eventName = "SpinJam Juggling Event";
	const eventDate = "Coming Soon";
	const eventLocation = "TBA";
	const eventDescription = "Join us for an exciting juggling event featuring amazing performers, workshops, and community fun!";
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

		<section class="event-info">
			<div class="info-card">
				<h2>Date</h2>
				<p>{eventDate}</p>
			</div>

			<div class="info-card">
				<h2>Location</h2>
				<p>{eventLocation}</p>
			</div>
		</section>

		<section class="description">
			<p>{eventDescription}</p>
		</section>

		<section class="additional-content">
			<p>More details about the event will be announced soon. Stay tuned for updates on performers, workshops, and registration information.</p>
			<p>This is a community event celebrating the art of juggling and bringing together enthusiasts from all skill levels.</p>
		</section>
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

	.event-info {
		display: grid;
		grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
		gap: 1.5rem;
		margin-bottom: 3rem;
		max-width: 800px;
		margin-left: auto;
		margin-right: auto;
	}

	.info-card {
		padding: 1.5rem;
		border: 1px solid var(--card-border);
		border-radius: 8px;
		text-align: center;
		background-color: var(--card-bg);
	}

	.info-card h2 {
		font-size: 1.2rem;
		margin: 0 0 0.5rem 0;
		color: var(--accent-muted);
	}

	.info-card p {
		font-size: 1.1rem;
		margin: 0;
		font-weight: 500;
		color: var(--text-strong);
	}

	.description {
		text-align: center;
		font-size: 1.1rem;
		line-height: 1.6;
		color: var(--text-muted);
		max-width: 800px;
		margin: 0 auto 3rem auto;
	}

	.additional-content {
		max-width: 800px;
		margin: 0 auto;
		color: var(--text-muted);
		line-height: 1.8;
	}

	.additional-content p {
		margin-bottom: 1.5rem;
	}
</style>
