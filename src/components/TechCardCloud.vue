<script setup>
	import TechCard from './TechCard.vue';
</script>
<template>
	<TechCard>
		<template #title>A Estrutura</template>
		<template #content>
			<img
				width="1.6875rem"
				src="../assets/images/tools/tool-firebase.svg"
				alt="Logo do Firebase"
			/>
			Firebase e
			<img
				width="1.6875rem"
				src="../assets/images/tools/tool-vercel.svg"
				alt="Logo da Vercel"
			/>
			Vercel são plataformas que fornecem serviços como hospedagem e
			autenticação.
		</template>
		<template #buttons>
			<button @click="$emit('change-to', 'design')">anterior</button>
			<button aria-hidden="true" tabindex="-1" disabled class="inactive">
				próximo
			</button>
		</template>
	</TechCard>
</template>
