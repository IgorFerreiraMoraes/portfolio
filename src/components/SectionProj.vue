<script setup>
	import Title from './Title.vue';
	import ProjCard from './ProjCard.vue';
	import Cocktail from '../assets/images/projects/cocktail-app.avif';
	import Solarium from '../assets/images/projects/solarium.avif';
</script>
<template>
	<section id="projects">
		<Title size="medium">Projetos em Destaque</Title>
		<div class="projects-area">
			<div class="projects-cards">
				<ProjCard
					:image="Cocktail"
					repository="https://github.com/IgorFerreiraMoraes/cocktail-app"
					link="https://www.instagram.com/reel/CpzqLDBAK0U/"
				>
					App de pedidos de coquetéis com Vue usando componentes, uma
					API externa e armazenamento de dados
				</ProjCard>
				<ProjCard
					:image="Solarium"
					repository="https://github.com/IgorFerreiraMoraes/Solarium"
					link="https://www.behance.net/gallery/162023573/Solarium"
				>
					Criei a identidade visual da Solarium, incluindo logo, site
					responsivo e estratégia de marca
				</ProjCard>
			</div>
		</div>
	</section>
</template>
<style scoped>
	.projects-area {
		margin-top: 1rem;
		min-height: 558px;
		position: relative;
	}
	.projects-area::before {
		content: '';
		position: absolute;
		top: 0;
		left: 50%;
		transform: translateX(-50%);
		width: 100vw; /* Make it 100% of the viewport width */
		height: 100%; /* Make it 100% of the .section height */
		background: url('../assets/images/projects/projects-background.avif');
		background-size: 100%;
		z-index: -1;
	}
	.projects-cards {
		padding-top: 4rem;
		display: grid;
		grid-template-columns: repeat(2, max(87.39%, 18rem));
		column-gap: 2rem;
		overflow-x: scroll;
	}

	@media (min-width: 1024px) {
		.projects-area {
			min-height: 762px;
		}
		.projects-area::before {
			background-position: 0 -8rem;
		}
		.projects-cards {
			padding-top: 3rem;
			display: grid;
			grid-template-columns: repeat(2, 1fr);
			column-gap: 5.5rem;
			overflow-x: scroll;
		}
	}
</style>
