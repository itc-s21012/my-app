# react api

## 映画検索ができるapi
キーワードを入れると映画を探してくるアプリ

## 作成方法
- 友達と協力しながら勧めた
- いろんなサイトを検索して有効活用できそうなのを使用した
- 何回もyarn startをかけて出たエラーやnvimに出るエラーを調べて修正した

## 仕様したapi
- OMDb API: http://www.omdbapi.com/?i=tt3896198&apikey=98e52704
- キーを取得するためメールアドレスを登録したりキーをアクティブにした

## 工夫した点
コンポーネントを４つに分けた
- App.js(他の３つの親コンポーネント)
- Header.js(ヘッダーをレンダリングし、タイトルのプロップスを受け取る)
- Movie.js(各映画をレンダリング)
- Search.js(入力と検索を行うフォーム)

## その他
- feachのエラーが出てきたので、調べた結果
yarn add node-fetchとnpm install --save node-fetchをコマンドで実行したが変わりなし。
import fetch from 'node-fetch';をApp.jsの先頭に追加した結果、エラーは消えたが起動しない
- その後、import fetch from 'node-fetch';を消したら起動した（何故？）
- 参考にしたサイト
- [Node.jsでfetchを使えるようにする](https://morizyun.github.io/javascript/node-js-npm-library-node-fetch.html)
- [ReferenceError: fetch is not defined](https://stackoverflow.com/questions/48433783/referenceerror-fetch-is-not-defined)

### ソースコードはsrc->components->4つのjsファイルそれぞれ
