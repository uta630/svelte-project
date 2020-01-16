<script>
	export let title = 'no title';
</script>

<div class="c-title">
	{#if title !== ''}
		<h1>{title}!!!</h1>
	{:else}
		<h1>Empty!</h1>
	{/if}
</div>

<style>
	.c-title {
		background: #333;
		padding: 12px 24px;
		color: white;
	}
</style>