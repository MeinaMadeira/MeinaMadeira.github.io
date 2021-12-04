---
layout: post
title:  "Blender Beginner Tutorial に挑戦 Lv.3"
date:   2021-12-04 15:00:00 +0900
categories: blender tutorial donut
---

Blenderを使ってのドーナツ製作第3回。今回はドーナツの隣に置くコーヒーを作っていきます。

[Blender Begginer Tutorial Series](https://www.youtube.com/playlist?list=PLjEaoINr3zgEq0u2MzVgAaHEBt--xLB6U)


## コーヒーカップの概形をつくる
- [Part 1, Level 3: Modelling Blender Beginner Tutorial](https://www.youtube.com/watch?v=7a0cHFs7jkw)

コーヒーカップの正面写真をお手本に使って円柱からカップを作っていきます。これは汎用的に使えそうなテクニックですね。

## コーヒカップの取手をつくる
- [Part 2, Level 3: Complete Modelling Blender Beginner Tutorial](https://www.youtube.com/watch?v=SBtDix7xGOg)

カップ側面の一部から押し出しと回転を使って取手を作っていきます。ツールバーからスピンを選べば３Dカーソルを中心として選択部分を回転させながら押し出すことも可能です。取手を接続するときは面を貼りたい頂点や辺を選択して「面を貼る」(F)すればOKです。

## コーヒーカップにガラスの質感を出す
- [Part 3, Level 3: Glass and Liquid Blender Beginner Tutorial](https://www.youtube.com/watch?v=7w-m13ykLN8)

レンダーエンジンをEeveeからCyclesに変えることで緻密な描画ができるようになるのですが、これがすごくマシンパワーを食います。
またマテリアルにはガラスの質感専用のBSDFがあるようですがそのままプリンシプルBSDFを使っていきます。粗さを細かく、透明度を最大に、屈折率はデフォルトで美しいガラスの質感が出るはずです。

中身のコーヒーはコップの内側を反転させて作ります。内側をコピーして作るために法線が反転してしまうのでこれを修正する必要があります。またカップの内側と液面が近すぎると面同士が接触するために一方のテクスチャしか反映されない場合があります。距離を離すためにコーヒーの方をほんの少しだけ縮小することでカップとコーヒー両方のテクスチャを反映することができます。

ここまで製作した画像がこちらです。


<img src="/images/coffee_and_donut_delicious.png" alt="coffee_and_donut" title="level3">
次回，最終シリーズでは仕上げにアニメーションをつけて動画としてレンダリングしていきます。

