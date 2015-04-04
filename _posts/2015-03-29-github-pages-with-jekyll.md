---
layout: post
title:  "GitHub Pages でブログを始める"
date:   2015-03-29 07:31:56
tags: jekyll github pages
---
jekyll を使って Github Pages にブログを作るメモ

1. (username).github.io レポジトリを作る
1. [jekyll](http://jekyllrb.com/) をインストール
1. セットアップ
```sh
$ jekyll new (username).github.io
$ cd (username).github.io
$ jekyll serve # http://127.0.0.1:4000/ にアクセスして動作確認。Ctrl-c で抜ける。
$ git init
$ git add .
$ git commit -m ‘create github pages’
$ git remote add origin git@github.com:(username)/(username).github.io.git
$ git fetch origin
$ git push origin master
```
1. http://(username).github.io にアクセスして動作確認（反映まで時間がかかることがある）
