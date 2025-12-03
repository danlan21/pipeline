<script lang="ts">
	import { columns } from "./data";
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Pipeline task management platform" />
</svelte:head>

<section>
	<div class="column-container">
		{#each columns as column (column)}
			<div class="column">
				<h1>{column}</h1>
			</div>
		{/each}
	</div>
</section>

<style>
	.column {
		margin: 0.5em;
		padding: 1em;
		border: 1px solid green;
		border-radius: 4px;

		flex-basis: 0;
		flex-grow: 1;
	}
	.column-container {
		margin: 0.5em;
		padding: 1em;
		border: 2px solid black;
		border-radius: 8px;
		height: 100vh;
		display: flex;
		flex-direction: row;
	}
</style>
