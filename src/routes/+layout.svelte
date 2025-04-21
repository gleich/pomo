<script lang="ts">
	import type { Snippet } from 'svelte';
	import '@gleich/ui/styles.css';
	import '../styles/global.css';
	import '../styles/fonts.css';

	const { children }: { children: Snippet } = $props();
</script>

<main>
	{@render children()}
</main>

<style>
	main {
		min-height: 100vh;
	}
</style>
