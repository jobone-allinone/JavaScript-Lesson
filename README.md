# JavaScript入門編

## 目次

- JavaScriptとは
- 基本的な使い方
- 変数について
- データ型について
- 演算子について

## JavaScriptとは

- WEBブラウザに実装されているプログラミング言語
- HTML・CSSの要素を操作して、WEBサイトに動きをつけたい時に使用

## 基本的な使い方

- HTMLファイルに直接記入する
- JSファイルを作成し、外部ファイルとして読み込む

## HTMLファイルに記述する

```html
<!-- scriptタグ内にJavaScriptコードを記述する -->
<script>
    alert("Hello Job One");
</script>
```

## JSファイルを作成し外部ファイルとして読み込む

```html
<!-- HTMLファイル -->
<script>
    <script src="js/sample1.js"></script>
</script>
```

```js
//sample1.js
/* 外部ファイルとして読み込む使い方が主流です。 */
alert("Hello Job One");
```

## 変数について①

- データを入れる箱のようなもの。
- 変数を使うことで何度も同じコードを書かなくて済む
![values](https://user-images.githubusercontent.com/35711528/36879211-00effebc-1e06-11e8-8056-47f1fb12e066.png)

msgという箱に「 Hello Job One 」という文字列が入っているイメージです。

## 変数について②

```js
var msg = "Hello Job One";
alert(msg);

var world =  "world";
alert(world);
// 変数を新しく作る時、かならず「var」を付ける必要があります。作った後は「var」を付ける必要はありません。
/* ただしES2015以降の仕様では「let」または「const」を使うことが多いです*/
```

## データ型について

- 数値(""又は'' で囲われていない数値)
- 文字列("" 又は'' で囲った文字列)
- 真偽値( true / false)
- null
- オブジェクト
　ー配列
　ー関数
等があります。

少しづつ覚えていきましょう。

## 演算子について①

- ＝

代入演算子。
変数に値を代入する時に使います。

```js
var msg = "Hello Job One";
```

## 演算子について②

- ＋

加算演算子

文字列結合、数値の加算等に使います。

```js
var msg = "Hello " + "Job One";
var num = 1 + 1;
```

## 演算子について③

- ==
- ===

比較演算子
被演算子が等しい場合に trueを返します。等しくない場合、falseを返します。
「===」の場合は型まで比較します。

```js
var num = 1;
alert(num == 1); // 「true」とアラートがでます。
alert(num === "1"); // 「false」とアラートがでます。
```

```js
var msg = "Hello";
alert(msg == "world"); // 「false」とアラートがでます。
```
