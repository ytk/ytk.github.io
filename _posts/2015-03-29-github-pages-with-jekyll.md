---
layout: post
title:  "Jekyll を使って GitHub Pages でブログを始める"
date:   2015-03-29 07:31:56
tags: jekyll github pages blog
---

記念すべき最初のポストは GitHub Pages でブログを始める方法を。

### GitHub Pages って？
GitHub ではスタティックなウェブサイトを無料で公開できる [GitHub Pages](https://pages.github.com/) というサービスがあります。  
GitHub を使っている人であればやり方は簡単で、`(username).github.io` というレポジトリを作ってそこにコンテンツを push すると `http://(username).github.io` という URL で公開されるというものです。  
※username は GitHub アカウント名

ただし、1からサイトを作るのは大変なので、スタティックページジェネレーターである [Jekyll](http://jekyllrb.com/) を使って構築してみます。  
※GitHub Pages では Jekyll をサポートしているので、毎回ページを手動生成しなくとも、レポジトリに push するだけで GitHub Pages 側で自動生成処理が走ります。

### Jekyll を使って GitHub Pages でブログを始める手順
1. GitHub アカウントが無い場合は[アカウント作成](https://github.com/)を済ませる。
1. (username).github.io レポジトリを作る
1. [jekyll](http://jekyllrb.com/) をインストールする
1. セットアップ

{% gist ytk/b303f3e382335978f1a9 %}

http://(username).github.io にアクセスして動作確認できれば完了です。  
※反映まで時間がかかることがあるので、しばらく待ちましょう。

ブログタイトル等の変更は `_config.yml` を修正することで反映できます。
