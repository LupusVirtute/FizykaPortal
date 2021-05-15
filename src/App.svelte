<script lang="ts">
import BodyMomentum from "./Calculations/BodyMomentum.svelte";

import Friction from "./Calculations/Friction.svelte";
import Speed from "./Calculations/Speed.svelte";

import SpeedForce from "./Calculations/SpeedForce.svelte";



	let components = [
		SpeedForce,
		Friction,
		BodyMomentum,
		Speed
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