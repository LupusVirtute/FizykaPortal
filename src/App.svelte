<script lang="ts">
import Friction from "./Calculations/Friction.svelte";

import SpeedForce from "./Calculations/SpeedForce.svelte";



	let components = [
		SpeedForce,
		Friction
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