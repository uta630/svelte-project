## svelte project
VSCodeでlang="scss"を記述するとエラーになるので設定を変更する。  
まずプロジェクトディレクトリの直下に「svelte.config.js」を作成して設定を記述。  
VSCodeで「Svelte> Language-server：Runtime」にnodeのパスを記述して再起動。  
※nodeのパスはターミナルで[which node]を実行してnodeのパスを確認できる。  
参考URL：https://medium.com/@sean_27490/svelte-sapper-with-sass-271fff662da9