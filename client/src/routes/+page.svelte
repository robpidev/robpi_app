<script>
	import Links from './Links.svelte';
</script>

<main>
	<section class="desctiption">
		<div>
			<img src="favicon.png" alt="robpi" />
		</div>
		<div class="info">
			<span>Aprende sobre programación y mates.</span>
			<Links />
		</div>
	</section>

	<section class="section">
		<h2>Linux</h2>
		<p>Como usar el susbsitema de linux para windows y configuración</p>
		<iframe
			width="100%"
			height="400px"
			src="https://www.youtube.com/embed/t4XZLxAkOGU"
			title="Windows Subsitem for LInux | Como usar linux sin salir de windows | WSL"
			frameborder="0"
			allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
			referrerpolicy="strict-origin-when-cross-origin"
			allowfullscreen
		></iframe>
	</section>
</main>

<style>
	.desctiption {
		padding: 1rem;
		align-items: center;
		display: flex;
		max-width: 1200px;
		gap: 1rem;
		flex-wrap: wrap;
		justify-content: center;
	}

	.info {
		display: flex;
		flex-direction: column;
		align-items: center;
	}

	.desctiption span {
		/*color: var(--secondary);*/
		font-size: 2rem;
		font-weight: 600;
		font-family: 'consolas';
		justify-content: center;
	}

	h2 {
		margin: 0;
	}

	iframe {
		border-radius: 12px;
	}

	.card {
		border: 1px solid var(--secondary);
		border-radius: 8px;
	}
</style>
