---
layout: post
title:  "Github Pages でブログを作成した時にハマったところ"
date:   2021-08-05 16:58:00 +0900
categories: jekyll github
---

## 経緯
転職活動を本格化させるにあたって，制作物やこれまでの開発過程をまとめたページを作ろうと思い立つ。  
どんな形にするか考えていたところ知人に「Github Pagesで作るのが簡単だよ！」と勧められたのでひとまず触ることにしました。

## 作成手順

詳しい作成手順はここでは触れません。大方は[Github docs](https://docs.github.com/ja/pages/setting-up-a-github-pages-site-with-jekyll/creating-a-github-pages-site-with-jekyll)をご参照ください。 

## ハマったところ
- webrickがない  
   Github docsに従ってサイトを構築していくと，webrickがないことをbundlerに怒られます。ので，Gemfileに以下を追記。  
   `gem "webrick", "~> 1.7"`

- minima以外のjekyll themeが適用できない    
     `jekyll new` してサイト作成した際のデフォルトのサイトテーマはminimaになっています。
    これを別のサイトテーマに変更しようとすると，他のテーマはブログ形式のレイアウトを持たないためにページレイアウトが崩れてしまいます。ブログ形式を採用する場合はテーマギャラリーなどからブログ対応可能なテーマを探す必要がありそうです。
    
