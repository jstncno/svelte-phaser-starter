<script lang="ts">
	import { onMount } from 'svelte';

	import config from './game/config';

	let gameContainer: HTMLElement;

	onMount(() => {
		console.log(gameContainer)
		const game = new Phaser.Game(config);
	});

</script>

<main id="game-container" bind:this={gameContainer}></main>

<style>
	main {
		display: flex;
		margin: auto;
	}
</style>
