<script lang="ts">
	import bostonSilhouette from '$lib/assets/boston_silhouette_transparent.png';

	const mapsUrl =
		'https://www.google.com/maps/search/?api=1&query=142+Memorial+Drive+Cambridge+MA+02139';
</script>

<div class="page-container">
	<div class="sky-spacer" aria-hidden="true"></div>
	<div
		class="skyline-layer"
		aria-hidden="true"
		style={`--skyline-image: url(${bostonSilhouette});`}
	></div>

	<div class="content-section">
		<!-- HERO -->
		<header class="hero">
			<h1 class="event-name">BJF</h1>
			<p class="event-subtitle">Boston Juggling and Flow</p>
			<p class="event-tagline">Come to the BJF celebration festival!</p>
			<p class="event-tagline">
				The MIT Juggling Club will be <strong>50 years old</strong>, and<br />
				The Boston Spinjam will be <strong>20 years old</strong>!
			</p>
			<div class="hero-badges">
				<span class="badge">Saturday, April 4, 2026</span>
				<span class="badge">Free Admission</span>
			</div>
		</header>

		<hr class="accent-rule" />

		<!-- INFO CARDS -->
		<section class="info-grid" aria-label="Event details">
			<div class="info-card">
				<div class="info-card-icon">
					<svg
						width="28"
						height="28"
						viewBox="0 0 24 24"
						fill="none"
						stroke="currentColor"
						stroke-width="2"
						stroke-linecap="round"
						stroke-linejoin="round"
					>
						<circle cx="12" cy="12" r="10" />
						<polyline points="12 6 12 12 16 14" />
					</svg>
				</div>
				<h2 class="info-card-label">When</h2>
				<p class="info-card-text">
					<strong>Saturday, April 4, 2026</strong><br />
					9:30 AM to 10:30 PM<br />
					No cost — completely free admission.
				</p>
			</div>

			<div class="info-card">
				<div class="info-card-icon">
					<svg
						width="28"
						height="28"
						viewBox="0 0 24 24"
						fill="none"
						stroke="currentColor"
						stroke-width="2"
						stroke-linecap="round"
						stroke-linejoin="round"
					>
						<path d="M21 10c0 7-9 13-9 13s-9-6-9-13a9 9 0 0 1 18 0z" />
						<circle cx="12" cy="10" r="3" />
					</svg>
				</div>
				<h2 class="info-card-label">Where</h2>
				<p class="info-card-text">
					Massachusetts Institute of Technology<br />
					Morss Hall, Walker Building<br />
					<a href={mapsUrl} target="_blank" rel="noopener noreferrer" class="address-link">
						142 Memorial Drive, Cambridge, MA 02139
					</a>
				</p>
			</div>

			<div class="info-card">
				<div class="info-card-icon">
					<svg
						width="28"
						height="28"
						viewBox="0 0 24 24"
						fill="none"
						stroke="currentColor"
						stroke-width="2"
						stroke-linecap="round"
						stroke-linejoin="round"
					>
						<path
							d="M12 2l2.4 7.4H22l-6.2 4.5 2.4 7.4L12 16.8l-6.2 4.5 2.4-7.4L2 9.4h7.6z"
						/>
					</svg>
				</div>
				<h2 class="info-card-label">What</h2>
				<p class="info-card-text">
					A day of Juggling and Flow arts!<br />
					Including games, informal workshops, and free treats.
				</p>
			</div>
		</section>

		<!-- SCHEDULE -->
		<section class="schedule-section">
			<h2 class="section-heading">Schedule</h2>
			<p class="schedule-tbd-note">Full schedule coming soon — check back for updates!</p>
			<div class="schedule-timeline">
				<div class="schedule-item">
					<span class="schedule-time">9:30 AM</span>
					<span class="schedule-desc">Doors Open</span>
				</div>
				<div class="schedule-item tbd">
					<span class="schedule-time">10:00 AM</span>
					<span class="schedule-desc">Workshops & Open Juggling <span class="tbd-badge">TBD</span></span>
				</div>
				<div class="schedule-item tbd">
					<span class="schedule-time">Afternoon</span>
					<span class="schedule-desc">Games & Activities <span class="tbd-badge">TBD</span></span>
				</div>
				<div class="schedule-item tbd">
					<span class="schedule-time">Evening</span>
					<span class="schedule-desc">Open Flow & Social <span class="tbd-badge">TBD</span></span>
				</div>
				<div class="schedule-item">
					<span class="schedule-time">10:30 PM</span>
					<span class="schedule-desc">Event Ends</span>
				</div>
			</div>
		</section>

		<!-- STORY -->
		<section class="story-section">
			<h2 class="section-heading">Why</h2>
			<p>
				The MIT Juggling Club was started <strong class="accent-number">50</strong> years ago
				by Arthur Lewbel in 1976. It's now the oldest juggling club in continuous operation in
				the entire world!
			</p>
			<p>
				Plus, the Boston Spinjam is <strong class="accent-number">20</strong> years old!
			</p>
			<p class="celebration">Happy Birthday to Boston Juggling and Flow!</p>
		</section>

		<!-- NOTE -->
		<aside class="note-callout">
			<div class="note-icon">
				<svg
					width="24"
					height="24"
					viewBox="0 0 24 24"
					fill="none"
					stroke="currentColor"
					stroke-width="2"
					stroke-linecap="round"
					stroke-linejoin="round"
				>
					<circle cx="12" cy="12" r="10" />
					<line x1="12" y1="16" x2="12" y2="12" />
					<line x1="12" y1="8" x2="12.01" y2="8" />
				</svg>
			</div>
			<div class="note-text">
				<strong>Getting There</strong>
				<p>
					Parking is expensive and hard to find. Taking public transportation is
					recommended.
				</p>
			</div>
		</aside>

		<!-- FOOTER -->
		<footer class="site-footer">
			<hr class="accent-rule" />
			<p>MIT Juggling Club &middot; Boston Spinjam</p>
		</footer>
	</div>
</div>

<style>
	:global(:root) {
		--sky-color: linear-gradient(180deg, #f4e6d7 0%, #e5eef5 100%);
		--base-color: #1f2329;
		--accent-primary: #a31f34;
		--accent-muted: #8a8b8c;
		--card-bg: #2a2f38;
		--card-border: #3a414c;
		--text-strong: #f6f7fb;
		--text-muted: #c8cdd6;
		--skyline-height: clamp(260px, 40vw, 550px);
	}

	/* ---- PAGE CONTAINER ---- */
	.page-container {
		width: 100%;
		min-height: 100vh;
		margin: 0;
		padding: 0;
		display: flex;
		flex-direction: column;
		background-color: var(--base-color);
	}

	/* ---- SKY SPACER ---- */
	.sky-spacer {
		width: 100%;
		height: clamp(0px, 8vw, 120px);
		background-color: #f4e6d7;
	}

	@media (max-width: 768px) {
		.sky-spacer {
			display: none;
		}
	}

	/* ---- SKYLINE ---- */
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
		-webkit-mask-size: 100% auto;
		mask-size: 100% auto;
		-webkit-mask-repeat: no-repeat;
		mask-repeat: no-repeat;
		-webkit-mask-position: center bottom;
		mask-position: center bottom;
	}

	/* ---- CONTENT SECTION ---- */
	.content-section {
		background-color: var(--base-color);
		color: var(--text-strong);
		width: 100%;
		padding: 1.5rem clamp(1rem, 4vw, 2rem) 2rem;
		margin: 0;
		flex: 1;
	}

	/* ---- HERO ---- */
	.hero {
		text-align: center;
		padding: 0.5rem 0 2rem;
		max-width: min(900px, 90vw);
		margin: 0 auto;
	}

	.event-name {
		font-size: clamp(2.5rem, 6vw, 4rem);
		font-weight: 800;
		letter-spacing: 0.15em;
		text-transform: uppercase;
		color: var(--text-strong);
		margin: 0 0 0.25rem;
	}

	.event-subtitle {
		font-size: clamp(1rem, 2.5vw, 1.4rem);
		font-weight: 400;
		letter-spacing: 0.15em;
		text-transform: uppercase;
		color: var(--text-muted);
		margin: 0 0 1.25rem;
	}

	.event-tagline {
		font-size: clamp(0.95rem, 2vw, 1.1rem);
		color: var(--text-muted);
		margin: 0.4rem 0;
		line-height: 1.6;
	}

	.event-tagline strong {
		color: var(--text-strong);
	}

	.hero-badges {
		display: flex;
		justify-content: center;
		gap: 1rem;
		flex-wrap: wrap;
		margin-top: 1.5rem;
	}

	.badge {
		display: inline-block;
		padding: 0.5rem 1.25rem;
		border-radius: 100px;
		background: rgba(163, 31, 52, 0.15);
		color: var(--accent-primary);
		font-weight: 600;
		font-size: 0.9rem;
		letter-spacing: 0.03em;
	}

	/* ---- ACCENT RULE ---- */
	.accent-rule {
		border: none;
		width: 60px;
		height: 2px;
		background: var(--accent-primary);
		margin: 2rem auto;
	}

	/* ---- INFO CARDS ---- */
	.info-grid {
		display: grid;
		grid-template-columns: repeat(auto-fit, minmax(min(260px, 100%), 1fr));
		gap: 1.5rem;
		max-width: min(900px, 90vw);
		margin: 0 auto 3rem;
	}

	.info-card {
		background: var(--card-bg);
		border: 1px solid var(--card-border);
		border-top: 3px solid var(--accent-primary);
		border-radius: 8px;
		padding: 1.5rem;
		transition:
			transform 200ms ease,
			box-shadow 200ms ease;
	}

	@media (hover: hover) {
		.info-card:hover {
			transform: translateY(-2px);
			box-shadow: 0 4px 20px rgba(0, 0, 0, 0.3);
		}
	}

	.info-card-icon {
		width: 28px;
		height: 28px;
		margin-bottom: 0.75rem;
		color: var(--accent-primary);
	}

	.info-card-label {
		font-size: 0.85rem;
		font-weight: 700;
		text-transform: uppercase;
		letter-spacing: 0.1em;
		color: var(--accent-primary);
		margin: 0 0 0.75rem;
	}

	.info-card-text {
		font-size: 1rem;
		color: var(--text-muted);
		line-height: 1.6;
		margin: 0;
	}

	.info-card-text strong {
		color: var(--text-strong);
	}

	.address-link {
		color: var(--text-muted);
		text-decoration: underline;
		text-underline-offset: 3px;
		text-decoration-color: var(--card-border);
		transition:
			color 200ms ease,
			text-decoration-color 200ms ease;
	}

	.address-link:hover {
		color: var(--accent-primary);
		text-decoration-color: var(--accent-primary);
	}

	/* ---- SCHEDULE SECTION ---- */
	.schedule-section {
		max-width: min(700px, 85vw);
		margin: 0 auto 3rem;
		text-align: center;
	}

	.schedule-tbd-note {
		color: var(--accent-muted);
		font-size: 0.95rem;
		font-style: italic;
		margin: 0 0 1.5rem;
	}

	.schedule-timeline {
		background: var(--card-bg);
		border: 1px solid var(--card-border);
		border-radius: 8px;
		overflow: hidden;
	}

	.schedule-item {
		display: flex;
		align-items: center;
		flex-wrap: wrap;
		padding: 1rem 1.5rem;
		border-bottom: 1px solid var(--card-border);
		text-align: left;
		gap: 0.25rem 0;
	}

	.schedule-item:last-child {
		border-bottom: none;
	}

	.schedule-item.tbd {
		opacity: 0.6;
	}

	.schedule-time {
		flex-shrink: 0;
		min-width: 90px;
		width: 110px;
		font-weight: 600;
		font-size: 0.9rem;
		color: var(--accent-primary);
		letter-spacing: 0.02em;
	}

	@media (max-width: 400px) {
		.schedule-item {
			padding: 0.85rem 1rem;
		}

		.schedule-time {
			width: auto;
			min-width: 80px;
		}
	}

	.schedule-desc {
		color: var(--text-muted);
		font-size: 1rem;
		display: flex;
		align-items: center;
		gap: 0.6rem;
		flex-wrap: wrap;
	}

	.schedule-item:not(.tbd) .schedule-desc {
		color: var(--text-strong);
	}

	.tbd-badge {
		display: inline-block;
		padding: 0.15rem 0.5rem;
		border-radius: 4px;
		background: rgba(138, 139, 140, 0.2);
		color: var(--accent-muted);
		font-size: 0.7rem;
		font-weight: 700;
		letter-spacing: 0.08em;
		text-transform: uppercase;
	}

	/* ---- STORY SECTION ---- */
	.story-section {
		max-width: min(700px, 85vw);
		margin: 0 auto 3rem;
		text-align: center;
	}

	.section-heading {
		font-size: 1.5rem;
		font-weight: 700;
		color: var(--text-strong);
		text-transform: uppercase;
		letter-spacing: 0.1em;
		margin: 0 0 1rem;
	}

	.story-section p {
		color: var(--text-muted);
		line-height: 1.7;
		font-size: 1.05rem;
		margin: 0.75rem 0;
	}

	.accent-number {
		color: var(--accent-primary);
		font-weight: 700;
		font-size: 1.15em;
	}

	.celebration {
		color: var(--text-strong) !important;
		font-weight: 600;
		font-size: 1.1rem !important;
		margin-top: 1.25rem !important;
	}

	/* ---- NOTE CALLOUT ---- */
	.note-callout {
		display: flex;
		align-items: flex-start;
		gap: 1rem;
		max-width: min(700px, 85vw);
		margin: 0 auto 3rem;
		padding: 1.25rem 1.5rem;
		background: var(--card-bg);
		border-left: 3px solid var(--accent-primary);
		border-radius: 0 8px 8px 0;
	}

	.note-callout strong {
		color: var(--text-strong);
		display: block;
		margin-bottom: 0.5rem;
	}

	.note-callout p {
		color: var(--text-muted);
		margin: 0;
		line-height: 1.6;
	}

	.note-icon {
		flex-shrink: 0;
		width: 24px;
		height: 24px;
		color: var(--accent-primary);
		margin-top: 2px;
	}

	/* ---- FOOTER ---- */
	.site-footer {
		text-align: center;
		padding: 1rem 0 2rem;
	}

	.site-footer p {
		color: var(--accent-muted);
		font-size: 0.85rem;
		letter-spacing: 0.05em;
		margin: 0;
	}
</style>
