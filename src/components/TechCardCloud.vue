<script setup>
	import TechCard from './TechCard.vue';
</script>
<template>
	<TechCard>
		<template #title>A Estrutura</template>
		<template #content>
			<img
				src="../assets/images/tools/tool-firebase.svg"
				alt="Photoshop logo"
			/>
			Firebase e
			<img
				src="../assets/images/tools/tool-vercel.svg"
				alt="Figma Logo"
			/>
			Vercel são plataformas que fornecem serviços como hospedagem e
			autenticação.
		</template>
		<template #buttons>
			<button @click="$emit('change-to', 'design')">anterior</button>
			<button tabindex="-1" disabled class="inactive">próximo</button>
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
