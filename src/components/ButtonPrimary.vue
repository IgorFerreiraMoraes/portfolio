<script setup>
	const props = defineProps(['link']);

	function open_link() {
		window.open(props.link, '_blank');
	}
</script>
<template>
	<div role="button" @click="open_link">
		<a :href="link" target="_blank">
			<slot></slot>
		</a>
	</div>
</template>
<style scoped>
	a {
		color: var(--color-background);
		font: var(--body-large);
		letter-spacing: -0.2px;
		transition: 0.2s;
	}
	div {
		background-color: var(--color-main);
		height: 3.5rem;
		border-radius: 0.5rem;
		display: flex;
		align-items: center;
		justify-content: center;
		transition: 0.2s;
	}
	div:hover {
		box-shadow: 0px 0.5rem 1.5rem -0.5rem rgba(0, 244, 255, 0.2);
		cursor: pointer;
	}
</style>
