# プログラミング言語に共通する文法と考え方

対応言語: PHP / JavaScript / TypeScript / Java / Python / C / C++ / C# / Lua / ShellScript

---

## 🧩 共通する基本文法とその解説

### 1. 変数宣言

```c
int x = 5;
```

- 多くの言語では型を指定して変数を宣言。
- JavaScript/TypeScript では `let`, `const` などを使い、型は省略可能（TypeScript は型注釈あり）。

---

### 2. 演算子

```text
+ - * / %（算術演算子）
== != > < >= <=（比較演算子）
&& || !（論理演算子）
```

- 条件式や数値計算、真偽値判定に使用。

---

### 3. 条件分岐

```c
if (condition) {
    // 処理
} else if (otherCondition) {
    // 他の処理
} else {
    // どれでもない処理
}
```

- すべての言語に存在。条件によって異なる処理を選択。

---

### 4. 繰り返し処理（ループ）

```c
for (int i = 0; i < 10; i++) {
    // 処理
}

while (condition) {
    // 処理
}
```

- `for`, `while`, `do-while` など。Python や JavaScript でも同様。

---

### 5. 関数・メソッド

```python
def greet(name):
    return "Hello " + name
```

- 一連の処理を再利用可能にする。
- 入力（引数）と出力（戻り値）を明確に定義。

---

### 6. 配列・リスト・コレクション

```java
String[] fruits = {"apple", "banana"};
```

- 複数の値をまとめて管理。イテレーションにも対応。

---

### 7. コメント文

```c
// 一行コメント
/* 複数行コメント */
# Python/Shell のコメント
```

- コードの説明や無効化に使用。実行時には無視される。

---

## 🎯 共通するプログラミングの考え方（パラダイム）

### ▶️ 手続き型（Procedural）

- 順に命令を記述して処理（例：C, ShellScript）

### 🧱 オブジェクト指向（OOP）

- クラスとオブジェクト、継承、カプセル化など（Java, C++, C#, Python）

### 🔁 関数型（Functional）

- 関数を値として扱う。状態を持たない設計が特徴（JavaScript, Python, Lua）

---

## 🔚 まとめ

- 構文は異なっても「条件分岐」「繰り返し」「関数」「変数」などの基本的な枠組みは共通。
- パラダイムの違い（OOP、手続き型、関数型）を理解すれば、異なる言語も習得しやすい。