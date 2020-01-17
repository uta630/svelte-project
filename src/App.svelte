<script>
	import Heading from './Components/Heading.svelte';
	import Text from './Components/Text.svelte';
	export let name;
</script>

<main>
	<Heading title='Svelte' />

	<Text text={name} />
	<Text text=''/>

	<Text>
		<p>Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn how to build Svelte apps.</p>
	</Text>
</main>

<style lang="scss">
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	a {
		color: #ff3e00;
		text-transform: uppercase;
		font-weight: 100;
	}

	p {
		padding-top: 8px;
		border-top: 1px solid black;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>