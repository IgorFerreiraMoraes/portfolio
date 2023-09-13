<script setup>
	import ButtonPrimary from './ButtonPrimary.vue';
	import Title from './Title.vue';

	const link_whatsapp =
		'https://wa.me/5511941285976?text=Ol%C3%A1,%20Igor!%20Tenho%20interesse%20em%20seus%20servi%C3%A7os,%20vamos%20conversar%20sobre%20como%20voc%C3%AA%20pode%20me%20ajudar?';
</script>
<template>
	<section id="thanks">
		<Title size="medium">Obrigado por ler até aqui!</Title>
		<Title size="small">Bora criar algo fascinante juntos</Title>
		<ButtonPrimary :link="link_whatsapp">Entrar em contato</ButtonPrimary>
	</section>
</template>
<style scoped>
	#thanks h2,
	#thanks h3 {
		text-align: center;
	}
	#thanks h3 {
		margin-bottom: 1rem;
	}
</style>
