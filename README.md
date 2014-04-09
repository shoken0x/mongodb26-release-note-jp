# MongoDB 2.6 リリースノート

MongoDB 2.6がリリースされました。新機能として、アグリゲーションフレームワークの改善、統合的テキスト検索、クエリーエンジンの改善、新しい書き込みオペレーション、セキュリティ修正が含まれています。

また、オンプレミスサーバーのバックアップに加え、モニタリングも可能になったMMS 1.4もリリースされました。詳細はMMS 1.4のドキュメントとMMS 1.4のリリースノートを参照してください。

_訳注: リリースノート原文_
_(http://docs.mongodb.org/master/release-notes/2.6/)_


## 大きな変更点


### アグリゲーションフレームワークの改善

アグリゲーションパイプラインは、カーソルを返すことによって任意のサイズの結果セットを返すことができるようになり、また必要に応じてコレクションにアウトプットを書き込みできるようになりました。さらに変数をサポートし、データフィルタリングと結果セットを処理する新しいオペレーションを追加しました。

- [db.collection.aggregate()](http://docs.mongodb.org/master/reference/method/db.collection.aggregate/#db.collection.aggregate)はカーソルを返すようになりました。カーソルを返すことによって、アグリゲーションパイプラインは、任意のサイズの結果セットを返すことができます。

- アグリゲーションのための新しいexplainオプションは、mongodがパイプラインを処理する方法についての情報を提供します。

- アグリゲーションはより効率的な外部ディスクベースのソートプロセスを使用できるようになりました。

- 新しいパイプラインステージとして、以下が追加されました。
 - [<code>$out</code>](http://docs.mongodb.org/master/reference/operator/aggregation/out/#pipe._S_out)ステージはコレクションへ書き込むためのステージです。
 - [<code>$redact</code>](http://docs.mongodb.org/master/reference/operator/aggregation/redact/#pipe._S_redact)ステージはフィールドレベルでのフィルタリングを提供します。

- 新しい修飾子（modified operators）として以下が追加されました。
 - [setオペレータ](http://docs.mongodb.org/master/reference/operator/aggregation-set/)
 - [<code>$let</code>](http://docs.mongodb.org/master/reference/operator/aggregation/let/#exp._S_let)と[<code>$map</code>](http://docs.mongodb.org/master/reference/operator/aggregation/map/#exp._S_map)によってアグリゲーションパイプラインで変数の宣言と操作が可能になりました。
 - [<code>$literal</code>](http://docs.mongodb.org/master/reference/operator/aggregation/literal/#exp._S_literal)と[<code>$size</code>](http://docs.mongodb.org/master/reference/operator/aggregation/size/#exp._S_size)オペレータ
 - これまで[<code>$cond</code>](http://docs.mongodb.org/master/reference/operator/aggregation/cond/#exp._S_cond)の引数は配列のみでしたが、Objectも取れるようになりました。

### Text Search Integration


### Insert and Update Improvements


### New Write Operation Protocol


### MSI Package for MongoDB Available for Windows



## Security Improvements


## Query Engine Improvements


## Improvements


### Geospatial Enhancements


### Index Build Enhancements


### Enhanced Sharding and Replication Administration


## Operational Changes


### Storage


### Networking


### Tool Improvements


## MongoDB Enterprise Features


### MongoDB Enterprise for Windows


### Auditing


### LDAP Support for Authentication


### Expanded SNMP Support


## Additional Information


### Changes Affecting Compatibility


### Upgrade Process


### Download


### Other Resources












