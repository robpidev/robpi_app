<script>
	import Icon from '@iconify/svelte';

	function copy() {
		navigator.clipboard.writeText('https://github.com/robpidev/wezterm_windows.git');
	}
</script>

<main>
	<h1>Configuraciones</h1>
	<section class="section">
		<h2>
			Terminal:
			<a target="_blank" href="https://wezfurlong.org/wezterm/index.html"> Wezterm </a>
		</h2>
		<img src="img/wez.png" alt="Wezterm config" />
		<hr />
		<p>
			Clona el respositorio
			<a target="_blank" href="https://github.com/robpidev/wezterm_windows.git"> Wezterm config </a>
			<button on:click={copy}><Icon icon="bx:copy" /></button>

			En la carpeta <code>~/.config</code> o si usas windows
			<code>C:\Users\[nombre de usuario]\.config</code>, si no tienes la carpeta creala.
		</p>

		<h3>Herramientas Adicionales</h3>
		Es el que la configuración de la linea de comandos, puedes instalarlo y configurarlo desde aquí
		<a target="_blank" href="https://starship.rs/guide/">Guia de instalación de starship</a>
	</section>

	<section class="section">
		<h2>Editor de código: Neovim</h2>
	</section>
</main>

<style>
	h2 {
		margin: 1rem 0;
	}

	img {
		width: 100%;
		border-radius: 8px;
	}

	button {
		background: initial;
		border: none;
		color: white;
		font-size: 1.1rem;
	}

	code {
		display: inline-block;
		background: rgba(255, 255, 255, 0.15);
		border-radius: 4px;
		padding: 2px 5px;
	}

	h1 {
		max-width: 1000px;
		width: 100%;
	}
</style>
