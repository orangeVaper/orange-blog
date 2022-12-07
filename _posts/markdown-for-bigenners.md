---
title: 'Markdown記法メモ'
excerpt: 'エンジニアはMarkdownを好んで使うということで、このブログでも記事に使っているMarkdown記法についてまとめてみようかと思います。以前お世話になった凄腕エンジニアもよくわからない記法や記号を使っていて、その時にMarkdown記法の存在を知ったものです。'
coverImage: '/assets/blog/blog-starter-kit-install/cover2.jpg'
date: '2022-11-30T18:18:07.322Z'
author:
  name: orangeVager
  picture: '/assets/blog/authors/orangeVaper.png'
ogImage:
  url: '/assets/blog/blog-starter-kit-install/cover2.jpg'
---

## Markdown記法とは

[Getting Started](https://www.markdownguide.org/getting-started/)こちらを参考にしています。

> Markdownはあなたが平文テキスト文書にフォーマット要素を追加するために使用することができる軽量のマークアップ言語です。2004年にジョン・グルーバーによって作成され、Markdownは現在、世界で最も人気のあるマークアップ言語の一つです。

つまりMarkdownはマークアップ言語だっていうことです。

## なぜMarkdownなのか？

Why we use markdown? とぐぐると、

> Markdownは、キーボードから指を離すことなく、あなたの文章に集中することによって、書式設定ツールバーとマウスクリックのすべての気晴らしを取り払う。上級ライターは、その場でテキストをスタイライズできるこのようなシームレスな体験が好きです。

キーボードから指を離すことなく、とありますが、今のところどうしても指をキーボードから話してしまいますｗ vimやneovimなども使い慣れたらもっといい文章環境になるかもしれませんね。

## Markdown記法の使い方

### タイトル

```
# h1タイトル
## h2タイトル
### h3タイトル
#### h4タイトル
##### h5タイトル
###### h6タイトル
```
表示は

# h1タイトル
## h2タイトル
### h3タイトル
#### h4タイトル
##### h5タイトル
###### h6タイトル

となります

よく使うのはh1からh3まででしょう。

cssで調節されていれば別ですが、デフォルトのフォントサイズがh4以下は本文より小さいです。

### 箇条書き

箇条書きは、- ハイフン、* アスタリスク、+ プラス、1. などのナンバリングがあります。

```
- フロント言語
  * html
  * css
    + sass
    + tailwindcss
  * javascript
    1. turbopack
    1. Next.js
    1. React
```
表示は
- フロント言語
  * html
  * css
    + sass
    + tailwindcss
  * javascript
    1. turbopack
    1. Next.js
    1. React

となります。ナンバリングでは、全て1. と記述することで自動でインクリメントされるので、順番に入れ替えが生じた場合は役に立ちます。

### 水平線

水平線は、- ハイフン、 * アスタリスク、_アンダースコアを3つ以上記述すると書くことができます。連続していなくても、間にスペースが入っていても水平線が表示されます。

```
---
- - -
***
*  *  *
___
_ _ _
```

表示は全て同じです

```---の場合```

---

```- - -の場合```

- - -

```***の場合```

***

``` *  *  *の場合```

*  *  *

```___の場合```

___

```_ _ _の場合 ```

_ _ _

### 引用



### 二重引用


[Blog-Starter-Kit](https://vercel.com/templates/next.js/blog-starter-kit)をclone。



## インストール状況を確認



## authorsの画像




