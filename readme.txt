[TEST] Alfred Json Format in bash.alfredworkflowのメモ

機能：
　Alfred Json Formatを利用してAlfredに表示させる

インストール：
　1.alfredworkflowをダウンロード
　2.ファイルをダブルクリックしてワークフローに登録

使い方：
　Alfredからキーワードで起動
　testjson 
　と入力すると検索するリストを表示してくれます
　
　パラメータなしのキーワード起動で、よく使う検索一覧という感じで作ってみました
　

開発メモ：

1.JSONフォーマットを使ってみる
　本家サイトのヘルプがありました
　https://www.alfredapp.com/help/workflows/inputs/script-filter/json/
　仕様はとりあえず、最下部にワークフローの＋（追加）→ Getting Started → Script Fillterにサンプルがあるとのこと
　早速導入して、jsonformatと入力すると。。。

2.スクリプトを見てみる
　驚くほど簡単なコードでした
　cat << EOBでJSONを記述するだけのようです

3.早速、自分でコードを書いてみる
　xmlをできるだけシンプルにして書いてみました
　日本語も変数も全然平気でつかえます
　JSONの作り方をループにしたりするとエレガントかもしれません

背景：
　google suggest 	ワークフローでxmlを利用しているようでしたので、解析してみました。
　解析といっても、なんとなくphpの構文や動きを理解する程度です。
　そうしたらAlfred出力用のxmlがあることがわかったので試してみました。
　xmlで扱われている部分もあるようですが、多分過去バージョンを保証する意味で残っているようで、
　現在のAifredではJSON形式を推奨しています 
