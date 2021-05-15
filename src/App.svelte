<script lang="ts">
import BodyMomentum from "./Calculations/BodyMomentum.svelte";

import Friction from "./Calculations/Friction.svelte";
import PotentialWeight from "./Calculations/PotentialWeight.svelte";
import Speed from "./Calculations/Speed.svelte";

import SpeedForce from "./Calculations/SpeedForce.svelte";



	let components = [
		SpeedForce,
		Friction,
		BodyMomentum,
		Speed,
		PotentialWeight
	];

</script>

<main>
	<div class='content'>
		
		<h1>Portal Fizyczny</h1>
		{#each components as component}
		<div class='component'>
			<svelte:component this={component} />
		</div>
		{/each}
		<div class='empty'></div>
	</div>
</main>

<style global>
	.content {
		display:flex;
		flex-direction: column;
		flex-wrap: wrap;
		align-items: center;
	}
	.empty {
		padding-bottom: 4vh;
	}
	.component {
		margin-bottom:10px;
		border-radius: 20px;
		border: 1px solid #339;
		background: #335;
		width:50%;
		padding:10px;
	}
	:global(body){
		background: #334;
		color: white;
		text-align:center;
		font-size:1vw;
	}
	:global(span){
		color:#80f;
		font-weight: 700;
		font-size: 1.3vw;
	}
	:global(h2){
		color: #60a;
		text-shadow: 
		1px 1px 1px #111,
		-1px -1px 1px #111,
		1px -1px 1px #111
		;
	}
	:global(h3){
		color: #60f;
		text-shadow: 
		1px 1px 1px #111,
		-1px -1px 1px #111,
		1px -1px 1px #111
		;
	}
	:global(input) {
		margin-bottom:10px;
		font-weight: 900;
		background: #223;
		color: #ddd;
		border-radius:10px;
		-moz-appearance: textfield;
		appearance: textfield;
		border:0;

	}
	:global(input:focus){
		outline:none;
	}
</style>