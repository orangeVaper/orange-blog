---
title: 'githubへのpush'
excerpt: 'githubへのソースのpush方法のメモです。'
coverImage: '/assets/blog/how-to-github-push/github.jpg'
date: '2023-09-23T17:35:07.322Z'
author:
  name: orangeVager
  picture: '/assets/blog/authors/orangeVaper.png'
ogImage:
  url: '/assets/blog/how-to-github-push/github.jpg'
---

# githubへのpush

githubへのpushの方法をメモしておきます。てか、そんなにやることないので記事的にどうでしょうか。と思い始めました。このブログをgithubにpushしているのですが、どうやってやったか詳細まで覚えてないので、調べながらメモしますｗ

## githubアカウントを作ってなかったら作成する

githubを使うのでgithubアカウントを作成。

## 最初だけgitにユーザー名とメールアドレスを設定

ローカルのgitにユーザー名とメールアドレスを設定しておきます。コミットの履歴情報といったメタデータとして使われる。

```
git config --global user.name "YourGitHubUsername"
git config --global user.email "youremail@example.com"
```

設定の確認

```
git config --global --get user.name
git config --global --get user.email
```

## githubにリポジトリを作成

ログイン後githubでリポジトリを作成します。リポジトリを作成時にREADMEを作成するかどうか聞かれるので、作成しないでおきます。

## リモートリポジトリのURLをコピーする

## Next.jsのブログのインストール
