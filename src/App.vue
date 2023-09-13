<script setup>
	import SectionAbout from './components/SectionAbout.vue';
	import SectionHero from './components/SectionHero.vue';
	import SectionProj from './components/SectionProj.vue';
	import SectionSocial from './components/SectionSocial.vue';
	import SectionTech from './components/SectionTech.vue';
</script>

<template>
	<img class="hero-blur" src="./assets/images/background-blur.svg" alt="" />
	<main>
		<SectionHero></SectionHero>
		<SectionTech></SectionTech>
		<SectionProj></SectionProj>
		<SectionAbout></SectionAbout>
		<SectionSocial></SectionSocial>
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
	body {
		overflow-x: hidden;
	}
</style>
