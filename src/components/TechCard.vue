<script setup></script>
<template>
	<div class="tech-card">
		<h3><slot name="title"></slot></h3>
		<p class="content">
			<slot name="content"></slot>
		</p>
		<div class="buttons">
			<slot name="buttons"></slot>
		</div>
	</div>
</template>
<style scoped>
	.tech-card {
		background-color: var(--color-white);
		width: 81.5%;
		min-height: 16.8125rem;
		margin: auto;
		border-radius: 0.5rem;
		padding: 3rem 1.5rem;
		display: flex;
		flex-direction: column;
		justify-content: center;
	}
	h3 {
		color: var(--color-background);
		font: var(--body-large);
		letter-spacing: -0.2px;
		text-align: center;
		margin-bottom: 1rem;
	}
	.tech-card .content {
		font: var(--body-small);
		color: var(--color-dark-accent);
	}
	.buttons {
		display: flex;
		width: 100%;
		justify-content: space-evenly;
		margin-top: auto;
	}
	@media (min-width: 1024px) {
		.tech-card {
			width: 100%;
		}
	}
</style>
<style>
	.tech-card .content > img {
		width: 1.6875rem;
		vertical-align: bottom;
	}
</style>
