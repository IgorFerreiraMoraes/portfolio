<script setup>
	import TechCard from './TechCard.vue';
</script>
<template>
	<TechCard>
		<template #title>A Estética</template>
		<template #content>
			<img
				src="../assets/images/tools/tool-photoshop.svg"
				alt="Photoshop logo"
			/>
			Photoshop e
			<img src="../assets/images/tools/tool-figma.svg" alt="Figma Logo" />
			Figma são o que uso para fazer as composições, prototipagem e artes
			dos projetos.
		</template>
		<template #buttons>
			<button @click="$emit('change-to', 'front')">anterior</button>
			<button @click="$emit('change-to', 'cloud')">próximo</button>
		</template>
	</TechCard>
</template>
<style scoped>
	button {
		background-color: transparent;
		font: var(--body-small);
		color: var(--color-secondary);
		transition: 0.2s;
		cursor: pointer;
	}
	button:hover {
		color: var(--color-main);
	}
	button.inactive,
	button.inactive:hover {
		color: var(--color-text);
		cursor: auto;
	}
</style>
