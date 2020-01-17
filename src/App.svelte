<script>
	import Heading from './components/Heading.svelte';
	import Text from './components/Text.svelte';
	export let name;
</script>

<main>
	<Heading title='Svelte' />

	<Text text={name} />
	<Text text=''/>

	<Text>
		<p>Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn how to build Svelte apps.</p>
	</Text>

	<p class="c-main__text">Using scss and BEM.</p>
	<div class="c-main__quote">
		<p>VSCodeでlang="scss"を記述するとエラーになるので設定を変更する。</p>
		<p>まずプロジェクトディレクトリの直下に「svelte.config.js」を作成して設定を記述。</p>
		<p>VSCodeで「Svelte> Language-server：Runtime」にnodeのパスを記述して再起動。</p>
		<p>※nodeのパスはターミナルで[which node]を実行してnodeのパスを確認できる。</p>
		<p>参考URL：<a href="https://medium.com/@sean_27490/svelte-sapper-with-sass-271fff662da9" target="_blank">SassteとSvelte / Sapper！</a></p>
	</div>
</main>

<style lang="scss">
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;

		a {
			color: #ff3e00;
			text-transform: uppercase;
			font-weight: 100;
		}
	}

	.c-main {
		&__text {
			background: aquamarine;
		}

		&__quote {
			padding: 8px 12px;
			border-left: 4px solid #ccc;

			p {
				margin: 6px 0;
				text-align: left;
				font-size: 14px;
			}
		}
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>