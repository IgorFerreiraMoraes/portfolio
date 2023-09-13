<script setup>
	import ButtonSecondary from './ButtonSecondary.vue';
	import Title from './Title.vue';
	import GitHub from '../assets/images/social/social-github.svg';
	import Behance from '../assets/images/social/social-behance.svg';
	import LinkedIn from '../assets/images/social/social-linkedin.svg';
</script>
<template>
	<section id="social">
		<Title size="medium">Social</Title>
		<p>Para conhecer todos meus projetos:</p>
		<ButtonSecondary
			link="https://github.com/IgorFerreiraMoraes"
			:image="GitHub"
		>
			GitHub
		</ButtonSecondary>
		<ButtonSecondary
			link="https://www.behance.net/igorfmoraes"
			:image="Behance"
		>
			Behance
		</ButtonSecondary>
		<ButtonSecondary
			link="https://www.linkedin.com/in/moraes-igor/"
			:image="LinkedIn"
		>
			LinkedIn
		</ButtonSecondary>
	</section>
</template>
<style scoped>
	p {
		font: var(--body-medium);
		margin-top: 1rem;
		text-align: center;
	}
	#social h2 {
		text-align: center;
	}
	#social div {
		margin-top: 1.5rem;
	}
</style>
