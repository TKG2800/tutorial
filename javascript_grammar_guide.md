# JavaScript 文法解説

---

## 📌 基本構文

### 1. 変数宣言

```javascript
let a = 10;
const b = 20;
var c = 30;
```

- `let`: 再代入可・再宣言不可（ブロックスコープ）
- `const`: 再代入不可・再宣言不可（ブロックスコープ）
- `var`: 再代入可・再宣言可（関数スコープ）

---

### 2. データ型

```javascript
let num = 42;               // 数値
let str = "Hello";          // 文字列
let isTrue = true;          // 真偽値
let nothing = null;         // null
let undef = undefined;      // 未定義
let obj = { name: "John" }; // オブジェクト
let arr = [1, 2, 3];        // 配列
```

---

### 3. 演算子

```javascript
// 算術
+ - * / % **

// 比較
== != === !== > < >= <=

// 論理
&& || !

// 代入
= += -= *= /=

// その他
typeof, instanceof, ternary (? :)
```

---

### 4. 条件分岐

```javascript
if (x > 0) {
  console.log("positive");
} else if (x === 0) {
  console.log("zero");
} else {
  console.log("negative");
}
```

- `===` は型と値を比較、`==` は型変換後に比較

---

### 5. ループ

```javascript
for (let i = 0; i < 5; i++) {
  console.log(i);
}

while (condition) {
  // ...
}

do {
  // ...
} while (condition);
```

- `for...in`：オブジェクトのキーを列挙
- `for...of`：配列などの反復可能な要素を列挙

---

### 6. 関数

#### 通常関数

```javascript
function greet(name) {
  return "Hello, " + name;
}
```

#### 関数式

```javascript
const greet = function(name) {
  return "Hello, " + name;
};
```

#### アロー関数

```javascript
const greet = (name) => "Hello, " + name;
```

---

### 7. 配列・オブジェクト

```javascript
let fruits = ["apple", "banana"];
fruits.push("orange");

let person = {
  name: "Alice",
  age: 30
};
console.log(person.name);
```

---

### 8. クラス

```javascript
class Animal {
  constructor(name) {
    this.name = name;
  }
  speak() {
    console.log(`${this.name} makes a sound.`);
  }
}
```

---

### 9. モジュール

```javascript
// export.js
export const pi = 3.14;

// import.js
import { pi } from './export.js';
```

---

### 10. 非同期処理

```javascript
async function fetchData() {
  const res = await fetch("https://api.example.com");
  const data = await res.json();
  return data;
}
```

- `Promise`、`async/await` による非同期処理が主流

---

## ✅ まとめ

JavaScript は柔軟性が高く、初心者にも扱いやすい言語ですが、
`var` や `==` など注意すべき落とし穴も存在します。

常に `let` / `const` を使い、`===` を用いた厳密比較を推奨します。
