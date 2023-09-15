<script setup>
	import TechCard from './TechCard.vue';
</script>
<template>
	<TechCard>
		<template #title>A Essência</template>
		<template #content>
			<img
				src="../assets/images/tools/tool-nuxt.svg"
				alt="Logo do Nuxt"
			/>
			Nuxt e
			<img src="../assets/images/tools/tool-vue.svg" alt="Logo do Vue" />
			Vue são o que uso para construir interfaces web excepcionais e dar
			vida aos sites.
		</template>
		<template #buttons>
			<button tabindex="-1" disabled class="inactive">anterior</button>
			<button aria-hidden="true" @click="$emit('change-to', 'design')">
				próximo
			</button>
		</template>
	</TechCard>
</template>
