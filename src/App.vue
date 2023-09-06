<script setup>
	import ButtonPrimary from './components/ButtonPrimary.vue';
	import ButtonSecondary from './components/ButtonSecondary.vue';
	import Title from './components/Title.vue';
</script>

<template>
	<main>
		<Title size="large">Igor Moraes</Title>
		<Title size="medium">Front-end & Designer</Title>
		<Title size="small">Bora criar algo fascinante juntos</Title>
		<br />
		<ButtonPrimary link="https://github.com/"> Conheça </ButtonPrimary>
		<br />
		<ButtonSecondary
			link="https://github.com/"
			image="./src/assets/images/social/social-instagram.svg"
			>Instagram</ButtonSecondary
		>
	</main>
</template>

<style scoped></style>
