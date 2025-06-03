<script>
	let { children } = $props();
</script>

<nav>
	<ul>
		<li>
			<a class="logo" href="/">Robpi</a>
		</li>
		<li>
			<a href="/config">Configs</a>
		</li>
	</ul>
</nav>
{@render children()}

<style>
	nav {
		border-bottom: 1px solid rgba(255, 255, 255, 0.2);
		height: 48px;
		display: flex;
		align-items: center;
		padding: 0 1rem;
	}

	a {
		text-decoration: none;
		font-weight: 600;
		font-size: 1.2rem;
	}

	ul {
		margin: 0;
		padding: 0;
		list-style: none;
		display: flex;
		gap: 1rem;
		align-items: center;
	}

	.logo {
		font-size: 1.4rem;
		font-weight: 600;
	}
</style>
