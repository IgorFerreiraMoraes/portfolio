<script setup>
	import TechCard from './TechCard.vue';
</script>
<template>
	<TechCard>
		<template #title>A Essência</template>
		<template #content>
			<img src="../assets/images/tools/tool-nuxt.svg" alt="Nuxt logo" />
			Nuxt e
			<img src="../assets/images/tools/tool-vue.svg" alt="" />
			Vue são o que uso para construir interfaces web excepcionais e dar
			vida aos sites.
		</template>
		<template #buttons>
			<button tabindex="-1" disabled class="inactive">anterior</button>
			<button @click="$emit('change-to', 'design')">próximo</button>
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
