---
layout: post
title:  "Github Pages でブログ"
date:   2015-03-29 07:31:56
categories: jekyll github pages
---
jekyll を使って Github Pages にブログを作るメモ

```
(username).github.io レポジトリを作る
jekyll をインストール
http://jekyllrb.com/
$ jekyll new (username).github.io
$ cd (username).github.io
$ jekyll serve
確認。Ctrl-c で抜ける。
$ git init
$ git add .
$ git commit -m ‘first commit’
$ git remote add origin git@github.com:(username)/(username).github.io.git
$ git fetch origin
$ git push origin master
http://(username).github.io にアクセスして反映を確認（時間がかかることがある）
```
