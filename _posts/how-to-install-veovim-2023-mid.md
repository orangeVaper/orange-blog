---
title: '最新のneovimのインストール方法（そのかわりappimage）'
excerpt: 'vscode neovimが最新のneovimを欲しがっていたのでメモ'
coverImage: '/assets/blog/how-to-install-veovim-2023-mid/vscode-neovim.jpg'
date: '2023-10-08T17:35:07.322Z'
author:
  name: orangeVager
  picture: '/assets/blog/authors/orangeVaper.png'
ogImage:
  url: 'how-to-install-veovim-2023-mid.jpg'
---

# vscode neovimユーザーです。

最近vscodeのneovimを最新にしたら、なんだか選択モードで文字がぴょんぴょん飛んでしまって、まるでバグのようになっていましたので、メモします。というかブログの表題の通り最新のneovimが必要ということです。

## githubを確認

2023年9月くらいから頻繁にPRがされていて、何やら選択したら対応する文字が強調するようにしている模様でした。

```
https://github.com/vscode-neovim/vscode-neovim
```

## 今回のvscode neovimには、システムのnvimの最新版が必要

Issuesなど（いろいろ）見てみるとなんとなく、nvimの最新版が必要そうでした。これはvscode側ではなく、システムにインストールしてあるnvimの最新です。

## ということで、neovimの最新はこちら

```
https://github.com/neovim/neovim/wiki/Installing-Neovim#snap
```

自分はwsl=linuxなので、

```
curl -LO https://github.com/neovim/neovim/releases/latest/download/nvim.appimage
chmod u+x nvim.appimage
./nvim.appimage
```

をインストール。しかし何？appimageって？？で、今はあまり良くわかっていません。

## vscode のsettingを変更

変更前は、

```
/user/local/bin/nvim
```

だったので、

```
"vscode-neovim.neovimExecutablePaths.linux": "~/nvim.appimage",
```
に変更。これでvscode neovimでの不具合が修正されました。