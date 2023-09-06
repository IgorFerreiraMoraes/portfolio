<script setup>
	const props = defineProps(['size']);

	const sizes = {
		large: 'h1',
		medium: 'h2',
		small: 'h3',
	};
</script>

<template>
	<component :is="sizes[size]">
		<slot></slot>
	</component>
</template>

<style scoped>
	h1 {
		color: var(--color-white);
		font: var(--title-large);
		letter-spacing: -0.8px;
	}
	h2 {
		color: var(--color-white);
		font: var(--title-medium);
		letter-spacing: -0.24px;
	}
	h3 {
		font: var(--title-small);
	}
</style>
