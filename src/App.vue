<script setup>
	import SectionHero from './components/SectionHero.vue';
</script>

<template>
	<img class="hero-blur" src="./assets/images/background-blur.svg" alt="" />
	<main>
		<SectionHero></SectionHero>
	</main>
</template>

<style>
	.hero-blur {
		width: 70vw;
		position: absolute;
		aspect-ratio: 1 / 1;
		top: -45vw;
		left: -20vw;
	}
</style>
