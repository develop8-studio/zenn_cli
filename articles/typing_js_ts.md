---
title: "JavaScriptとTypeScriptの違い"
emoji: "🍡"
type: "tech"
topics: [javascript, typescript]
published: true
---

##  TypeScriptとは
TypeScript（略称: TS）は、Microsoftによって開発されたJavaScriptの拡張として開発されたプログラミング言語です。

##  JavaScriptとTypeScriptの違い
JavaScriptとTypeScriptは、型付けに関する重要な違いがあります。

###  静的な型付け
JavaScriptでは、変数や関数の型は実行時に決まります。つまり、コードを実行する際に変数に代入される値の型によって、その変数の型が動的に決定されます。例えば、以下のようなJavaScriptコードを考えてみましょう。

```js
let x = 10; // xは数値型
console.log(typeof x); // 結果: "number"

x = "Hello"; // xは文字列型
console.log(typeof x); // 結果: "string"
```
上記の例では、変数`x`は最初に数値型として宣言されましたが、後で文字列型の値が代入されました。JavaScriptは値の型に応じて自動的に変数の型を切り替えます。

一方、TypeScriptでは、開発者がコードを書くときに変数や関数に型を指定する必要があります。これにより、コンパイル時に型エラーが検出され、実行前に問題が発見されます。例えば、次のTypeScriptコードを考えてみましょう。
```ts
let x: number = 10; // xは数値型
console.log(typeof x); // エラー: TypeScriptはtypeof演算子をサポートしていません
```
TypeScriptでは、変数`x`に型注釈としてnumberが付けられています。このように、変数が宣言されるときに型が明示されるため、コンパイラが型エラーを検出します。JavaScriptとは異なり、TypeScriptでは型が実行時ではなく、開発者がコードを書く時点で確定されます。

## まとめ
#### JavaScriptは「型が動的」でTypeScriptは「型が静的」
JavaScriptでは、変数の型は実行時に解決されますが、TypeScriptではコードを書く段階で型を明示的に指定します。

[例]
JavaScript: ドアの鍵が何でも開ける（何でも代入できる）。
TypeScript: ドアの鍵は車の鍵なのか、家の鍵なのか、最初に決めておく必要がある。