<script>
	export let text = 'no text';
</script>

<div class="c-text">
	{#if text !== ''}
		<h1>Hello, {text}!</h1>
	{:else}
		<h1>Empty!</h1>
	{/if}
	<slot/>
</div>

<style>
	.c-text {
		color: #333;
		font-size: 14px;
	}
</style>