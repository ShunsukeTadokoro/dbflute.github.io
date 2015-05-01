# DBFlute
*DB変更に強い*をテーマにした開発支援ツール  

##DBFluteとは
- リーン・スタートアップ＆インクリメンタル開発
- 設計しながら実装する開発 (納期の短い開発)

ビジネス要求の変化が激しいシステム開発が増えてきました。DB変更は日常の風景。
そんな現場でDB変更に対しアプリケーションが**できるだけスピーディーに**対応できるようにするために、
DBFlute は大きく二つの機能を備えています。

*O/Rマッパー*
: 自動生成ドリブンでDB変更の影響範囲をスピーディーに検知  
*DB管理支援ツール*
: DB環境構築自動化や履歴管理など、DB変更の運用上の悩みを解決

両方の機能を利用することで最大の効果を得られますが、開発運用支援ツールの機能だけを利用することも可能であり、
様々なアーキテクチャと組み合わせて利用することもできます。

##インストール
###1. DBFluteクライアントの作成 (+ エンジンインストール)  
EMechaを使ってDBFluteモジュールとDBFluteクライアントの準備をして下さい。  
[EMecha - DBFluteクライアントの作成](http://dbflute.seasar.org/ja/manual/function/helper/emecha/newclient/index.html)

###2.DBFluteランタイムの準備
アプリケーションのクラスパスにDBFluteランタイム(JAR)を追加して下さい。  
[セットアップ - DBFluteランタイムの準備](http://dbflute.seasar.org/ja/environment/setup/runtime.html)

###3.JDBCドライバの準備
DBFluteにJDBCドライバが同梱されていないデータベース(Oracle や DB2 など)を利用する場合は、そのデータベースのJDBCドライバを配置する必要があります。 (同梱されてるDBならこの項目はスキップ)  
[セットアップ - JDBCドライバの準備](http://dbflute.seasar.org/ja/environment/setup/jdbcdriver.html)

###4.特定環境適用プロパティ
最初の自動生成の前に考慮すべき特定の環境に適用するためのプロパティを設定して下さい。 (ほとんどのケースで不要であると想定され、特殊な環境でなければ、もしくは、よくわからなければとりあえずスキップでもOK)  
  [セットアップ - 特定環境適用プロパティ](http://dbflute.seasar.org/ja/environment/setup/firstprop.html)

###5.クラスの自動生成
それでは、自動生成をしてみましょう。  
[セットアップ - クラスの自動生成](http://dbflute.seasar.org/ja/environment/setup/generate.html)

###6.DI環境の調整
アプリケーションで利用しているDIコンテナの環境にDBFluteのクラスを認識させて下さい。  
[セットアップ - DI環境の調整](http://dbflute.seasar.org/ja/environment/setup/injection.html)

###7. その後の設定
ひとまず、アプリケーション上でDBFluteのクラスを利用することができるようになりました。 しかし、ディベロッパーに横展開するまでには、まだあともうちょい頑張りが必要です。 より良い環境で実装してもらうために、現場フィットな機能を整えましょう！  
[セットアップ - その後の設定](http://dbflute.seasar.org/ja/environment/setup/thenafter.html)

##DBFluteの使い方
###チュートリアルあります
ここはいわゆる "分厚い本のマニュアル" のようなもので、構造的に網羅された仕様書です。  
なので、機能を探すときは "テーマごとのチュートリアル" がオススメです。  

*アーキテクト向け*
: [アーキテクトのためのチュートリアル](http://dbflute.seasar.org/ja/tutorial/architect.html)  
*ディベロッパー向け*
: [ディベロッパーのためのチュートリアル](http://dbflute.seasar.org/ja/tutorial/developer.html)  
*パッと見たいとき*
: [ひとめでDBFlute](http://dbflute.seasar.org/ja/tutorial/hitomeflute.html)  
