---
layout: post
title:  "GitHub Pages でブログを始める"
date:   2015-03-29 07:31:56
tags: jekyll github pages blog
---

記念すべき最初のポストは GitHub Pages でブログを始める方法を。

GitHub ではスタティックなウェブサイトを無料で公開できる [GitHub Pages](https://pages.github.com/) というサービスがあります。  
GitHub を使っている人であればやり方は簡単で、`(username).github.io` というレポジトリを作ってそこにコンテンツを push すると `http://(username).github.io` という URL で公開されるというものです。  
※username は GitHub アカウント名

ただし、1からサイトを作るのは大変なので、スタティックページジェネレーターである [Jekyll](http://jekyllrb.com/) を使って構築してみます。  
※GitHub Pages では Jekyll をサポートしているので、毎回ページを手動生成しなくとも、レポジトリに push するだけで GitHub Pages 側で自動生成処理が走ります。

1. GitHub アカウントが無い場合は[アカウント作成](https://github.com/)から。
1. (username).github.io レポジトリを作る
1. [jekyll](http://jekyllrb.com/) をインストールする
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
