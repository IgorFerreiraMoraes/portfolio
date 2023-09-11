<script setup>
	import Title from './Title.vue';
	import TechCard from './TechCard.vue';
</script>
<template>
	<section id="tech">
		<Title size="medium">Ferramentas e Tecnologias</Title>
		<p>
			Construindo pontes para o seu objetivo: conheça os instrumentos
			utilizados!
		</p>
		<img
			class="float"
			id="ps"
			src="../assets/images/tools/floating-photoshop.svg"
			alt=""
		/>
		<TechCard>
			<template #title>A Essência</template>
			<template #content>
				<img
					src="../assets/images/tools/tool-nuxt.svg"
					alt="Nuxt logo"
				/>
				Nuxt e
				<img src="../assets/images/tools/tool-vue.svg" alt="" />
				Vue são o que uso para construir interfaces web excepcionais e
				dar vida aos sites.
			</template>
		</TechCard>
		<img
			class="float"
			id="vue"
			src="../assets/images/tools/floating-vue.svg"
			alt=""
		/>
	</section>
</template>
<style scoped>
	section {
		position: relative;
	}
	p {
		font: var(--body-small);
		letter-spacing: -0.2px;
		margin: 1rem 0;
	}
	.float {
		width: 4.25rem;
		position: absolute;
	}
	#ps {
		top: 38%;
		left: -4%;
		transform: rotate(-10.646deg);
		filter: blur(2px);
		z-index: -1;
	}
	#vue {
		top: 80%;
		right: 0;
		transform: rotate(15deg);
		filter: blur(1px) drop-shadow(-2px 4px 12px #17252633);
	}
</style>
