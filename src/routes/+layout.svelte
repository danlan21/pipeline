<script lang="ts">
	import Header from './Header.svelte';
	import './layout.css';

	let { children } = $props();
</script>

<div>
	<Header />

	<main>
		{@render children()}
	</main>
</div>
