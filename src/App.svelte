<script lang="ts">
import SpeedForce from "./Calculations/SpeedForce.svelte";



	let components = [
		SpeedForce
	];

</script>

<main>
	<h1>Portal Fizyczny</h1>
	{#each components as component}
		<svelte:component this={component} />
	{/each}
</main>

<style>

</style>