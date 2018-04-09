# JavaScript入門編2

## 目次

- if文
- botを作ってみよう

## if文

if文を用いると「もし○○ならば●●を行う」という条件分岐が可能になります。

if (true)である必要があります。

```js
if (true) {
  // ()がtrueであれば、処理を実行
}
```

![if1](https://user-images.githubusercontent.com/35711528/36883927-e54e94a0-1e20-11e8-8f42-878a15134da3.png)

trueかどうかは入門編1で使用した演算子を主に用いて判断します。

```js
var msg = "Hello Job One";

if (msg === "Hello Job One") {
  // msgが“Hello Job One”であれば、trueを返却するので処理を実行
}
```

## else文

if文を用いると「もし○○ならば●●を行う」という条件分岐が可能になります。elseを用いることで「もし○○でなければ●●を行う」という処理が可能になります。

![else1](https://user-images.githubusercontent.com/35711528/36883934-ee9d00a0-1e20-11e8-83e7-f83c185fc6e3.png)

```js
var msg = "Hello Job One";

if (msg === "Hello world") {

} else {
// msgが“Hello world”でなければ、falseを返却するので処理を実行
}
```

## else if文
else ifを用いると「もし◯◯だったら●●を行う、そうでなくもし△△であれば▲▲を行う、いずれでもなければ■■を行う」という条件分岐ができます。

![elseif1](https://user-images.githubusercontent.com/35711528/36883942-f759efbe-1e20-11e8-993e-f6540b811cdb.png)


```js
if (条件式) {
    // 条件式がtrueなら実行
} else if (条件式) {
    // if (条件式)がfalseかつ、 else if (条件式)がtrueなら実行
} else {
    // if (条件式)がfalseかつ、 else if (条件式)もfalseであれば実行
}
```

## botを作ってみよう

```html
おいくつですか
<input type="text" id="age">
<button onclick="goAnswer()">goAnswer</button>

<script>
    function goAnswer() {
        const age = document.getElementById('age').value;
        if (age >= 20) {
            alert("成人されてますね");
        } else if (age >= 12 && age < 20) {
            alert("青年ですね");
        } else {
            alert("小学生かそれより年下ですね");
        }
    }
</script>
```
