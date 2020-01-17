<script>
	export let text = 'no text';
</script>

<div class="c-text">
	{#if text !== ''}
		<p>Hello, {text}!</p>
	{:else}
		<p>Empty!</p>
	{/if}
	<slot/>
</div>

<style lang="scss">
	.c-text {
		color: #333;
		font-size: 24px;
	}
</style>