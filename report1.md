## 封筒DBでB*-tree索引を作成する

### お題
 [サンプルスライド](pdf/EnvelopeDBMS-Btree.pdf)を参考に、
20レコードを挿入したB*-tree索引（一次索引）を作成しましょう。

### 締め切り
* 2016年5月31日 12:00 

### 提出方法
* Slack の #program チャンネルに以下の情報を投稿してください
  * 氏名
  * 学籍番号
  * ソースコードの置いてある場所
  * 説明の書いてあるファイルの場所

### 設定
* レコードは (氏名,年齢)の二つの属性を持ち, 年齢の属性で索引を作成してください。
* オーダーは d=1 とします（１ページに２レコードまで）

### 提出方法
* レポートは５名までのグループ提出OKとします。
* サンプルスライドのように挿入する過程を写真に撮り、PDFファイルで提出してください
* PDFファイルは情報科計算機室の ~chiemi/Report/dbms16/report1 においてください
* ファイル名は g学籍番号_g学籍番号_g学籍番号.pdf というようにメンバーの学籍番号をアンダースコア(_)で繋げてください。

## おまけ：btreeプログラムを書いてみる
### おまけ課題締め切り
 * 6月14日(火) 12:00
 
### ソースコードについて
* サンプルソースコード：rlsv.is.ocha.ac.jp:~chiemi/lecture/2016/dbms/btree
* 準備
 * サンプルソースコードをディレクトリごとコピーしてください
 
 ```
  % cp -r ~chiemi/lecture/2016/dbms/btree .
 ```
 
 * ~/.bash_profileに以下の１行を付け足してください

 ```
 export CLASSPATH=./bin:$CLASSPATH
 ```

 * .bash_profileを有効にしてください
 
 ```
 % source ~/.bash_profile
 ```

* コンパイル方法

```
 % javac -sourcepath src src/btree/* -d bin 
```

* 実行方法

```
 % java btree.Database
```

 * コピーしただけで何も編集してないでコンパイル・実行したら以下の１行が表示されるはずです

 ```
 % Hello! Let's start exercises.
 ```

* 課題をとくのに利用できるメソッドの情報
  * [program/bree/README.md](program/btree/README.md)
