---
layout: post
title:  "Blender Beginner Tutorial に挑戦 Lv.2"
date:   2021-12-03 21:20:00 +0900
categories: blender tutorial donut
---

Blenderを使ってのドーナツ製作第２回。今回はアイシングの上にかけるトッピングを作り、ドーナツのディテールを詰めていきます。

[Blender Begginer Tutorial Series](https://www.youtube.com/playlist?list=PLjEaoINr3zgEq0u2MzVgAaHEBt--xLB6U)

## トッピングを散らす
- [Part 1, Level 2: Particles Blender Beginner Tutorial](https://www.youtube.com/watch?v=jNmnPXY9UQA)

アイシングの上に散らしたい形のオブジェクトを別途作成し、パーティクルシステムで適用します。数や大きさ、散らばりのランダム性なとはパーティクルシステムタブから調節できますし、アイシングにウェイトペイントで密度の偏りを作ればトッピングを多く乗せたい部分と少なくしたい部分を作ることもできます。

## トッピングに色を指定する。
- [Part 2, Level 2: Random Materials Blender Beginner Tutorial](https://www.youtube.com/watch?v=aZ5ungDgFNc)

トッピングに色をつけるにあたってマテリアルを設定します。ここでシェーダータブに移動しオブジェクト情報ノードを追加。ランダムからBSDFノードへ接続するとパーティクルにはランダムにモノトーンカラーが設定されます。更にこのノード間にカラーランプノードを追加してようやく好きな色を指定することができます。どこに何のノードがあってどれとどれが接続できるかなどは情報が膨大すぎるので今後も勉強ですね。

パーティクルにはオブジェクトの他にオブジェクト群をまとめたコレクションを指定することができます。よって星でもハートでも好きな形のオブジェクトをコレクション内に作ればトッピングは自由自在ということです。

## ドーナツに焼き色をつける(テクスチャペイント)
- [Part 2, Level 3: Texture Painting Blender Beginner Tutorial](https://www.youtube.com/watch?v=nht2RoYBUfA)

テクスチャペイントについて。この辺は以前のフクロウでもやりましたね。加えてこの回ではテクスチャマスクを使ってドロー時にさまざまな模様を描き出すことができます。

↓こんな感じ


<img src="/images/Texture_mask.png" alt="texture_mask" title="level2">


## ドーナツの質感にこだわる
- [Part 4, Level 2: Procedural Displacement Blender Beginner Tutorial](https://www.youtube.com/watch?v=Rh5gAQLtOls)

テクスチャペイントが済んだら更に質感を本物に近づけていきます。シェーダータブに移動してノイズテクスチャノード，テクスチャ座標ノード，ディスプレイスメントノードを追加。それぞれを接続してノイズテクスチャの数値を調節することでドーナツ表面のような質感を表現することができます。やはりノードの組み合わせが膨大なので先達の資料をたくさん参照するのが良さそうです。

こうして描画したのがこちらのドーナツです。

<img src="/images/fried_donut.png" alt="fried_donut" title="level2">


だいぶドーナツらしく美味しそうな見た目になってすごく嬉しいですね。
次回シリーズではドーナツの隣に置くコーヒーとそのグラスカップを作ります。

