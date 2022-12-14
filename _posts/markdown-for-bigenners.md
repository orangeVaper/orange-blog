---
title: 'Markdown記法メモ'
excerpt: 'エンジニアはMarkdownを好んで使うということで、このブログでも記事に使っているMarkdown記法についてまとめてみようかと思います。以前お世話になった凄腕エンジニアもよくわからない記法や記号を使っていて、その時にMarkdown記法の存在を知ったものです。'
coverImage: '/assets/blog/markdown-for-bigenners/coffee.jpg'
date: '2022-12-12T23:36:07.322Z'
author:
  name: orangeVager
  picture: '/assets/blog/authors/orangeVaper.png'
ogImage:
  url: '/assets/blog/markdown-for-bigenners/coffee.jpg'
---

## Markdown記法とは

[Getting Started](https://www.markdownguide.org/getting-started/)を参考にしました

> Markdownはあなたが平文テキスト文書にフォーマット要素を追加するために使用することができる軽量のマークアップ言語です。2004年にジョン・グルーバーによって作成され、Markdownは現在、世界で最も人気のあるマークアップ言語の一つです。

つまりMarkdownはマークアップ言語だっていうことです。

## なぜMarkdownなのか？

> Markdownは、キーボードから指を離すことなく、あなたの文章に集中することによって、書式設定ツールバーとマウスクリックのすべての気晴らしを取り払う。上級ライターは、その場でテキストをスタイライズできるこのようなシームレスな体験が好きです。

ってことです

キーボードから指を離すことなく、とありますが、今のところどうしても指をキーボードから離してしまいますｗ vimやneovimなども使い慣れたらもっといい文章環境になるかもしれませんね

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

引用は、> を行頭に書きます。ネストも可能です

blockquotesで囲まれますが、そのblockquotesの中で段落を設けたい場合には、空白行の先頭に>を書きます

段落扱いなので、brのような改行ではなく、pの扱いですので、段落感のマージンが付きます

```
> 今日は寝る前にコーヒーを飲んでしまったんだ
>
> だから眠れなくなっちゃったよ
>
>> 本当は紅茶を飲むつもりだったんだ
>>
>> 明日は紅茶を飲むぞ
>>
>>> 明日紅茶で眠れたらいいね
```
> 今日は寝る前にコーヒーを飲んでしまったんだ
>
> だから眠れなくなっちゃったよ
>
>> 本当は紅茶を飲むつもりだったんだ
>>
>> 明日は紅茶を飲むぞ
>>
>>> 明日紅茶で眠れたらいいね

### 画像

画像表示もできます！

`![OrangeVaper](/assets/blog/authors/orangeVaper.png)`

![OrangeVaper](/assets/blog/authors/orangeVaper.png)

------
Main Imageは [Unsplash](https://unsplash.com/ja?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText)の[thirdy perasol](https://unsplash.com/@thirdyp_?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText)が撮影した写真
