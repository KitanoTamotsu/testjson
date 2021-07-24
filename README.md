## 　　Lesson6.　Alfredの出力フォーマットを試してみる 
#### 開発メモ
ワークフロー
<br><img width="600" src="https://user-images.githubusercontent.com/40127279/126855770-e0e7f392-8559-4e29-be92-1673beb72369.png">

### 1.Alfred Json Format
　ワークフローの追加『+』から、Getting StartedのScript Filterを選択しましょう
<br>　jsonformatとxmlformatの2つのScript Fillterが準備されています
<br>　ワークフローに登録してjsonformatもしくはxmlformatと入力してみましょう
<br>　これがAlfred Json Formatです
<br>　[ドキュメントもどうぞ](https://www.alfredapp.com/help/workflows/inputs/script-filter/json/)
### 2.Jsonの書き方を理解する
　jsonformatのScript Fillterを見てみましょう
<br>　シェルスクリプトでの利用は簡単そうですね
```
 Cat << EOB
 〜
 EOB
```
<br>　上記のようなコードでJsonを囲めばOKです
<br>　なおXMLタイプは非推奨です。なので使いません
<br>　多分過去バージョンの互換性保証のために残しているのではないかな
<br>　
<br>　ちなみ一言で言うと、XMLはタグ付きデータの集合で、
<br>　JSONはキーとバリューの集合です
<br>　XMLはHTML的な表現で
<br>　JSONは名前のとおりJavaScriptの表現となります
<br>　余談でした
### 3.パクる
　スクリプト学習の常套手段です。早速パクりましょう
<br>　最低限必要そうなキーはtitle, subtitle, argですかね
<br>　正しい仕様はalfredのヘルプを見てください
<br>　
<br>　早速ゴリゴリ書いてみましょう
<br>　いくつかのキーワードを表示させて、それを選択すると
<br>　デフォルトブラウザで検索するという動きです
<br>　コードをみながら実行してみてくださいな
<br>　各itemをループ処理で書くとエレガントかもしれませんね
<br>　
<br>　RunScript
<br>　<img width="600"  src="https://user-images.githubusercontent.com/40127279/126855793-99705aad-3352-4b9a-8b06-ae6e57c6af81.png">

#### 取扱説明
### 機能:
　Alfred Json Formatをシェルスクリプトで動かしてみる
<br>　※本家Alfredのサンプルの簡易版です
### インストール:
　1.[alfredworkflow](https://github.com/KitanoTamotsu/testjson/releases/download/1.0/TEST.Alfred.Json.Format.in.Bash.script.alfredworkflow.zip)をダウンロード 
<br>　2.ファイルをダブルクリックしてワークフローに登録
### 使い方:
　Alfredからキーワード起動『tj』
<br>
<br>
[トップページに戻る](https://kitanotamotsu.github.io/)

