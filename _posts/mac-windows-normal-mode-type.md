---
title: 'Mac/windows wsl2環境のvscode neovimでノーマルモードに戻った時自動で英数モードにするメモ'
excerpt: 'Macはim-select Windowsはwsl2/Ubuntu環境ですが、両方の設定方法のメモを残しておきます。Windowsのほうが比較的早く設定できたけど、Macはちょっと手こずりました。'
coverImage: '/assets/blog/blog-starter-kit-install/cover2.jpg'
date: '2022-12-08T18:18:07.322Z'
author:
  name: orangeVaper
  picture: '/assets/blog/authors/orangeVaper.png'
ogImage:
  url: '/assets/blog/blog-starter-kit-install/cover2.jpg'
---

## Windows/wsl2 vscode neovimで、ノーマルモードに戻ったときに自動で英数モードになる設定

[windowsでwsl2でvscode-neovimを早めにしたい](https://qiita.com/sijiaoh/items/4add320d684b7978a29f)と、

[WSL2+VS Code Neovim+ノーマルモードIME自動OFF](https://qiita.com/sasaki_hir/items/6d2cf64e4cd585e7b877)で書いてあるとおり

zenhanのインストール

環境はwindows/wsl2

```
curl -fLO https://github.com/iuchim/zenhan/releases/download/v0.0.1/zenhan.zip
unzip zenhan.zip
chmod u+x zenhan/bin64/zenhan.exe
sudo mv zenhan/bin64/zenhan.exe /usr/local/bin/zenhan
```
.config/nvim/init.vimに下記を記述

```
if executable('zenhan')
  autocmd InsertLeave * :call system('zenhan 0')
  autocmd CmdlineLeave * :call system('zenhan 0')
endif
```

vscodeのsettings.json(user)の設定



```
"vscode-neovim.neovimExecutablePaths.linux": "/usr/local/bin/nvim",
"vscode-neovim.useWSL": true,
"vscode-neovim.neovimInitVimPaths.linux": "~/.config/nvim/init.vim",
```
vscodeのリロード





