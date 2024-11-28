<script>
	import Icon from '@iconify/svelte';
	const links = [
		{
			name: 'GitHub',
			url: 'https://github.com/robpidev',
			bg: '#fff',
			fg: 'gray',
			icon: 'mdi:github'
		},
		{
			name: 'Discord',
			url: 'https://discord.gg/6kqy5H7',
			bg: 'purple',
			fg: 'white',
			icon: 'ic:outline-discord'
		},
		{
			name: 'YouTube',
			url: 'https://youtube.com/robpi',
			bg: 'red',
			fg: 'white',
			icon: 'mdi:youtube'
		},
		{
			name: 'Telegram',
			telegram: 'https://t.me/robpi',
			bg: 'skyblue',
			fg: '#000',
			icon: 'mdi:telegram'
		},
		{
			name: 'TikTok',
			url: 'https://tiktok.com/@robpidev',
			bg: 'black',
			fg: 'white',
			icon: 'ic:baseline-tiktok'
		}
	];
</script>

<ul>
	{#each links as links}
		<li>
			<a style="background: {links.bg}; color: {links.fg};" href={links.url}>
				<Icon icon={links.icon} style="font-size: 1.8rem;" />
				{links.name}
			</a>
		</li>
	{/each}
</ul>

<style>
	ul {
		display: flex;
		list-style: none;
		gap: 1rem;
		flex-wrap: wrap;
		padding: 0;
	}

	a {
		padding: 0.3rem 1rem 0.3rem 0.6rem;
		border-radius: 8px;
		text-decoration: none;
		display: flex;
		gap: 0.5rem;
		align-items: center;
	}

	li:last-child a {
		box-sizing: border-box;
		border: 1px solid white;
	}
</style>
