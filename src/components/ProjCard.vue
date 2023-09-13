<script setup>
	import ButtonPrimary from './ButtonPrimary.vue';
	import ButtonSecondary from './ButtonSecondary.vue';

	const props = defineProps(['image', 'repository', 'link']);

	const image_url = `url("${props.image}")`;
</script>
<template>
	<div class="proj-card">
		<div class="image"></div>
		<p>
			<slot></slot>
		</p>
		<div class="buttons">
			<ButtonSecondary :link="repository">repo</ButtonSecondary>
			<ButtonPrimary :link="link">conhecer</ButtonPrimary>
		</div>
	</div>
</template>
<style scoped>
	.proj-card {
		width: 100%;
		min-height: 26.9375rem;
		margin: auto;
		border-radius: 0.5rem;
		background: rgba(39, 49, 50, 0.75);
		backdrop-filter: blur(4px);
	}
	.image {
		width: 100%;
		min-height: 13rem;
		border-radius: 0.5rem 0.5rem 0 0;
		background-image: v-bind(image_url);
		background-size: cover;
	}
	p {
		margin: 1rem 1.5rem 1.5rem;
		font: var(--body-small);
	}
	.buttons {
		margin: 0 1.5rem;
		display: grid;
		grid-template-columns: 1fr 1fr;
		gap: 1rem;
	}

	@media (min-width: 1024px) {
		.proj-card {
			min-height: 32rem;
		}
		.image {
			min-height: 15.55rem;
		}
		.buttons {
			margin-top: 2.5rem;
		}
	}
</style>
