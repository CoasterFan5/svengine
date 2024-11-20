<script>
	import Navbar from '$lib/components/Navbar.svelte';
	import '@fontsource/monaspace-neon';
	let { children } = $props();
</script>

<Navbar />
{@render children()}

<style lang="scss">
	:global(body) {
		--text: #252422;
		--background: #ffffff;
		--primary: #ffa100;
		--secondary: #413e3a;
		--accent: #ccc5b8;
		margin: 0;

		color: var(--text);
		font-family: 'Monaspace Neon', monospace;
	}

	:global(*) {
		box-sizing: border-box;
		color: var(--text);
	}

	:global(*::selection) {
		background: var(--primary);
	}
</style>
