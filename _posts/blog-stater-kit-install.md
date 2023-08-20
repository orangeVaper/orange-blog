---
title: 'Next.js blog-starter-kitのインストール'
excerpt: 'Next.js/Reactの勉強をしてるんですがやはり、なにか実際に手を動かしてモノを作っていかなければということで手をつけ始めたのがテックブログなるものでした。果たしてものになるのかどうなのかやってみます。まずはblog-starterになります。'
coverImage: '/assets/blog/blog-starter-kit-install/cover2.jpg'
date: '2022-11-26T18:18:07.322Z'
author:
  name: orangeVager
  picture: '/assets/blog/authors/orangeVaper.png'
ogImage:
  url: '/assets/blog/blog-starter-kit-install/cover2.jpg'
---

## ブログを書き始めようと思ったきっかけ

そろそろなにか作り始めないといけないと思っていまして、何がいいかと考えていたんですが、ブログくらいしか思いつかずNext.jsでブログが作りやすそうなので、設置、カスタマイズ等のメモを記していければと思いました。

このブログ記事を書き始めていつ頃公開できるか多少心配してはいるんですが、ゆっくりじっくり執筆していこうかと思います。焦らずじっくりとｗ

## なぜNext.jsブログか？

- フロントエンド学習にもってこい
- wordpressより表示が早い模様
- reactの学習
- typeScriptの学習
- ブログ執筆は.mdでその書き方の学習
- デプロイにはvercelを使いたいが、それも勉強になる
- 以前Next.js/React環境のデザイニングで参画した経験があるので、更なる勉強のために
- 将来の自分の為のメモとして

学習項目が盛りだくさんで勉強になります

## Next.jsのブログのインストール
では、まずはここからブログをダウンロードします。

[Blog-Starter-Kit](https://vercel.com/templates/next.js/blog-starter-kit)をclone。

以下のコマンドでセットアップします。

```yarn create next-app --example blog-starter blog-starter-app```

## インストール状況を確認

インストールされたディレクトリに移動

```cd blog-stater-app```

コマンド実行

```npm run dev```

これでhttp://localhost:3000でローカルを確認できます

## ブログ記事の作成

_posts/ディレクトリに予め例がありますので、複製して自分のブログを書いていきます。ちょうど今、複製して書いています！

## authorsの画像

authors画像の保存ディレクトリにあります。

**public/assets/blog/authors**

この中に画像を保存して、記事の.mdファイルの先頭にあるpicture:に設定します。


