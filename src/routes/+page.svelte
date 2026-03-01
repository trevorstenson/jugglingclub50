<script lang="ts">
	import bjfBanner from '$lib/assets/bjf_banner.png';
	import oldLogo from '$lib/assets/old_blue.png';
	const mapsUrl =
		'https://www.google.com/maps/search/?api=1&query=142+Memorial+Drive+Cambridge+MA+02139';
</script>

<div class="page">
	<div class="banner-wrap">
		<img class="banner" src={bjfBanner} alt="Boston Juggling and Flow festival banner" />
	</div>

	<main class="content">
		<!-- HERO -->
		<header class="hero">
			<h1 class="title">Boston Juggling & Flow</h1>
			<p class="tagline">
				Come to the BJF festival to celebrate the <strong>50th</strong> anniversary of
				the MIT Juggling Club and the <strong>20th</strong> anniversary of Boston Spinjam!
			</p>
			<p class="tagline">
				Join us for a full day of open juggling, workshops, games, and free food.
				All skill levels welcome, whether you've never picked up a ball or you've been
				juggling for years. Open to everyone, not just MIT.
			</p>
			<p class="cheer">Happy Birthday to the MIT Juggling Club!</p>
			<div class="badges">
				<span class="badge badge--date">Saturday, April 4, 2026</span>
				<span class="badge badge--free">Free Admission</span>
			</div>
		</header>

		<div class="divider" aria-hidden="true">
			<span class="ball ball--1"></span>
			<span class="ball ball--2"></span>
			<span class="ball ball--3"></span>
		</div>

		<!-- DETAILS -->
		<section class="details" aria-label="Event details">
			<div class="detail detail--when">
				<h2>When</h2>
				<p>
					<strong>Saturday, April 4, 2026</strong><br />
					9:30 AM to 10:30 PM<br />
					Completely free, no cost at all.
				</p>
			</div>

			<div class="detail detail--where">
				<h2>Where</h2>
				<p>
					Massachusetts Institute of Technology<br />
					Morss Hall, Walker Building<br />
					<a href={mapsUrl} target="_blank" rel="noopener noreferrer">
						142 Memorial Drive, Cambridge, MA 02139
					</a>
				</p>
			</div>

			<div class="detail detail--what">
				<h2>What</h2>
				<p>
					A day of Juggling and Flow arts!<br />
					Including games, informal workshops, and free treats.
				</p>
			</div>
		</section>

		<!-- SCHEDULE -->
		<section class="schedule">
			<h2 class="section-title">Schedule</h2>
			<p class="schedule-note">Full schedule coming soon. Check back for updates!</p>
			<div class="timeline">
				<div class="tl-item">
					<span class="tl-time">9:30 AM</span>
					<span class="tl-desc">Doors Open</span>
				</div>
				<div class="tl-item tl-item--tbd">
					<span class="tl-time">10:00 AM</span>
					<span class="tl-desc">Workshops & Open Juggling/Flow <span class="tbd">TBD</span></span>
				</div>
				<div class="tl-item tl-item--tbd">
					<span class="tl-time">Afternoon</span>
					<span class="tl-desc">Games & Activities <span class="tbd">TBD</span></span>
				</div>
				<div class="tl-item tl-item--tbd">
					<span class="tl-time">Evening</span>
					<span class="tl-desc">Open Flow & Social <span class="tbd">TBD</span></span>
				</div>
				<div class="tl-item">
					<span class="tl-time">10:30 PM</span>
					<span class="tl-desc">Event Ends</span>
				</div>
			</div>
		</section>

		<!-- HISTORY -->
		<section class="history">
			<h2 class="section-title">A Bit of History</h2>
			<img class="old-logo" src={oldLogo} alt="Original MIT Juggling Club logo, circa 1980s" />
			<p>
				The MIT Juggling Club was founded in March 1975 by Arthur Lewbel, then an
				undergraduate, who merged his juggling group with Andy Rubel's unicycle club.
				It's been meeting weekly ever since, making it one of the longest continuously
				running public juggling clubs in the country.
			</p>
			<p>
				Over the decades the club attracted some remarkable visitors, including Claude
				Shannon, who developed the first mathematical theorem of juggling, and
				legendary high-speed photographer Doc Edgerton, who invited jugglers to his
				studio at MIT.
			</p>
			<p>
				Fifty years later, the club is still going strong. As Lewbel puts it,
				"you don't need dues. You don't need members. You just need to meet at the same
				place and time every week."
			</p>
		</section>

		<!-- NOTE -->
		<aside class="callout">
			<div class="callout-icon">
				<svg
					width="22"
					height="22"
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
			<div>
				<strong>Getting There</strong>
				<p>
					Parking is expensive and hard to find. Taking public transportation is
					recommended.
				</p>
			</div>
		</aside>

		<!-- FOOTER -->
		<footer class="footer">
			<p>MIT Juggling Club &middot; Boston Spinjam</p>
		</footer>
	</main>
</div>

<style>
	@font-face {
		font-family: 'Armstrong';
		src: url('../lib/assets/armstrong_3/Armstrong-Extrabold.otf') format('opentype');
		font-weight: 800;
		font-style: normal;
		font-display: swap;
	}

	:global(:root) {
		--onyx: #0c090d;
		--frosted-blue: #b5f0ff;
		--tomato: #f15946;
		--tuscan-sun: #f9c22e;
		--pacific-blue: #53b3cb;
		--navy: #1a3a5c;
		--surface: rgba(181, 240, 255, 0.07);
		--surface-border: rgba(181, 240, 255, 0.12);
		--text-primary: rgba(181, 240, 255, 0.92);
		--text-muted: rgba(181, 240, 255, 0.72);
		--text-strong: #b5f0ff;
	}

	/* ---- ANIMATIONS ---- */
	@keyframes fadeUp {
		from {
			opacity: 0;
			transform: translateY(16px);
		}
		to {
			opacity: 1;
			transform: translateY(0);
		}
	}

	@media (prefers-reduced-motion: reduce) {
		:global(*) {
			animation-duration: 0s !important;
			animation-delay: 0s !important;
		}
	}

	/* ---- PAGE ---- */
	.page {
		width: 100%;
		min-height: 100vh;
		background: var(--navy);
		color: var(--text-primary);
	}

	/* ---- BANNER ---- */
	.banner-wrap {
		position: relative;
		width: 100%;
		overflow: hidden;
	}

	.banner-wrap::after {
		content: '';
		position: absolute;
		bottom: -40px;
		left: 0;
		right: 0;
		height: 40px;
		background: linear-gradient(to bottom, rgba(26, 58, 92, 0.6) 0%, var(--navy) 100%);
		pointer-events: none;
		z-index: 1;
	}

	.banner {
		width: 100%;
		height: auto;
		display: block;
	}

	/* ---- CONTENT ---- */
	.content {
		max-width: 820px;
		margin: 0 auto;
		padding: 0 clamp(1.25rem, 5vw, 2.5rem) 2rem;
	}

	/* ---- HERO ---- */
	.hero {
		text-align: center;
		padding: 0.5rem 0 0.5rem;
	}

	.title {
		font-family: 'Armstrong', sans-serif;
		font-size: clamp(1.8rem, 5vw, 3rem);
		font-weight: 400;
		letter-spacing: 0.08em;
		color: var(--tuscan-sun);
		margin: 0 0 0.25rem;
		text-shadow: 0 0 60px rgba(249, 194, 46, 0.2);
		animation: fadeUp 0.6s ease-out both;
	}

	.tagline {
		font-size: clamp(1.05rem, 2.2vw, 1.15rem);
		color: var(--text-muted);
		margin: 0.4rem 0;
		line-height: 1.7;
		animation: fadeUp 0.6s ease-out 0.12s both;
	}

	.tagline strong {
		color: var(--tomato);
		font-weight: 700;
	}

	.cheer {
		color: var(--tuscan-sun);
		font-weight: 700;
		font-size: 1.15rem;
		margin: 1.25rem 0 0.25rem;
		animation: fadeUp 0.6s ease-out 0.16s both;
	}

	.badges {
		display: flex;
		justify-content: center;
		gap: 0.75rem;
		flex-wrap: wrap;
		margin-top: 1.75rem;
		animation: fadeUp 0.6s ease-out 0.2s both;
	}

	.badge {
		display: inline-block;
		padding: 0.55rem 1.3rem;
		border-radius: 100px;
		font-weight: 700;
		font-size: 0.95rem;
		letter-spacing: 0.04em;
		transition: box-shadow 200ms ease, background 200ms ease;
	}

	.badge--date {
		background: var(--tuscan-sun);
		color: var(--onyx);
	}

	.badge--free {
		background: transparent;
		border: 2px solid var(--tomato);
		color: var(--tomato);
	}

	@media (hover: hover) {
		.badge--date:hover {
			box-shadow: 0 0 24px rgba(249, 194, 46, 0.3);
		}

		.badge--free:hover {
			background: rgba(241, 89, 70, 0.1);
		}
	}

	/* ---- DIVIDER (juggling balls) ---- */
	.divider {
		display: flex;
		justify-content: center;
		gap: 0.65rem;
		padding: 2rem 0;
	}

	.ball {
		width: 10px;
		height: 10px;
		border-radius: 50%;
	}

	.ball--1 {
		background: var(--tomato);
	}

	.ball--2 {
		background: var(--tuscan-sun);
	}

	.ball--3 {
		background: var(--pacific-blue);
	}

	/* ---- DETAILS GRID ---- */
	.details {
		display: grid;
		grid-template-columns: repeat(auto-fit, minmax(min(240px, 100%), 1fr));
		gap: 1.25rem;
		margin-bottom: 3rem;
	}

	.detail {
		background: var(--surface);
		border: 1px solid var(--surface-border);
		border-radius: 10px;
		padding: 1.5rem;
		border-top: 3px solid;
		transition:
			transform 200ms ease,
			box-shadow 200ms ease;
		animation: fadeUp 0.5s ease-out both;
	}

	.detail:nth-child(1) {
		animation-delay: 0.15s;
	}

	.detail:nth-child(2) {
		animation-delay: 0.25s;
	}

	.detail:nth-child(3) {
		animation-delay: 0.35s;
	}

	.detail--when {
		border-top-color: var(--tuscan-sun);
	}

	.detail--where {
		border-top-color: var(--pacific-blue);
	}

	.detail--what {
		border-top-color: var(--tomato);
	}

	@media (hover: hover) {
		.detail:hover {
			transform: translateY(-2px);
			box-shadow: 0 8px 30px rgba(181, 240, 255, 0.06);
		}
	}

	.detail h2 {
		font-family: 'Armstrong', sans-serif;
		font-size: 1rem;
		font-weight: 400;
		text-transform: uppercase;
		letter-spacing: 0.15em;
		margin: 0 0 0.75rem;
	}

	.detail--when h2 {
		color: var(--tuscan-sun);
	}

	.detail--where h2 {
		color: var(--pacific-blue);
	}

	.detail--what h2 {
		color: var(--tomato);
	}

	.detail p {
		font-size: 1.05rem;
		color: var(--text-muted);
		line-height: 1.65;
		margin: 0;
	}

	.detail p strong {
		color: var(--text-strong);
	}

	.detail a {
		color: var(--pacific-blue);
		text-decoration: underline;
		text-underline-offset: 3px;
		text-decoration-color: rgba(83, 179, 203, 0.4);
		transition:
			color 200ms ease,
			text-decoration-color 200ms ease;
	}

	.detail a:hover {
		color: var(--frosted-blue);
		text-decoration-color: var(--frosted-blue);
	}

	/* ---- SECTION TITLE ---- */
	.section-title {
		font-family: 'Armstrong', sans-serif;
		font-size: 1.6rem;
		font-weight: 400;
		color: var(--frosted-blue);
		text-transform: uppercase;
		letter-spacing: 0.12em;
		text-align: center;
		margin: 0 0 0.75rem;
	}

	/* ---- SCHEDULE ---- */
	.schedule {
		margin-bottom: 3rem;
	}

	.schedule-note {
		text-align: center;
		color: var(--text-muted);
		font-size: 1rem;
		font-style: italic;
		margin: 0 0 1.5rem;
	}

	.timeline {
		background: var(--surface);
		border: 1px solid var(--surface-border);
		border-radius: 10px;
		overflow: hidden;
	}

	.tl-item {
		display: flex;
		align-items: center;
		padding: 0.9rem 1.5rem;
		border-bottom: 1px solid var(--surface-border);
	}

	.tl-item:last-child {
		border-bottom: none;
	}

	.tl-item--tbd {
		opacity: 0.5;
	}

	.tl-time {
		flex-shrink: 0;
		width: 110px;
		font-weight: 700;
		font-size: 0.95rem;
		color: var(--tuscan-sun);
		letter-spacing: 0.02em;
	}

	.tl-desc {
		color: var(--text-primary);
		font-size: 1.05rem;
		display: flex;
		align-items: center;
		gap: 0.5rem;
		flex-wrap: wrap;
	}

	.tl-item--tbd .tl-desc {
		color: var(--text-muted);
	}

	.tbd {
		display: inline-block;
		padding: 0.1rem 0.45rem;
		border-radius: 4px;
		background: rgba(83, 179, 203, 0.15);
		color: var(--pacific-blue);
		font-size: 0.75rem;
		font-weight: 700;
		letter-spacing: 0.08em;
		text-transform: uppercase;
	}

	@media (max-width: 480px) {
		.tl-time {
			width: 85px;
			font-size: 0.9rem;
		}

		.tl-item {
			padding: 0.8rem 1rem;
		}
	}

	/* ---- HISTORY ---- */
	.history {
		background: var(--surface);
		border: 1px solid var(--surface-border);
		border-left: 3px solid var(--tuscan-sun);
		border-radius: 0 10px 10px 0;
		padding: 1.75rem 2rem;
		margin-bottom: 3rem;
	}

	.history .section-title {
		text-align: left;
		font-size: 1.3rem;
		margin: 0 0 1rem;
		color: var(--tuscan-sun);
	}

	.old-logo {
		float: right;
		width: 180px;
		height: auto;
		margin: 0 0 1rem 1.5rem;
		border-radius: 8px;
		padding: 6px;
		background: #e8e8e8;
	}

	@media (max-width: 480px) {
		.old-logo {
			float: none;
			display: block;
			margin: 0 auto 1rem;
			width: 120px;
		}
	}

	.history p {
		color: var(--text-muted);
		line-height: 1.75;
		font-size: 1.05rem;
		margin: 0.75rem 0;
		text-align: left;
	}

	/* ---- CALLOUT ---- */
	.callout {
		display: flex;
		align-items: flex-start;
		gap: 1rem;
		padding: 1.25rem 1.5rem;
		background: var(--surface);
		border-left: 3px solid var(--pacific-blue);
		border-radius: 0 10px 10px 0;
		margin-bottom: 3rem;
	}

	.callout-icon {
		flex-shrink: 0;
		width: 22px;
		height: 22px;
		color: var(--pacific-blue);
		margin-top: 2px;
	}

	.callout strong {
		color: var(--frosted-blue);
		display: block;
		margin-bottom: 0.4rem;
		font-size: 1.05rem;
	}

	.callout p {
		color: var(--text-muted);
		margin: 0;
		line-height: 1.6;
		font-size: 1.02rem;
	}

	/* ---- FOOTER ---- */
	.footer {
		text-align: center;
		padding: 1.5rem 0 2.5rem;
		border-top: 1px solid var(--surface-border);
	}

	.footer p {
		color: var(--text-muted);
		font-size: 0.9rem;
		letter-spacing: 0.06em;
		margin: 0;
	}
</style>
