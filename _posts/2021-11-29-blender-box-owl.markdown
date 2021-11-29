---
layout: post
title:  "Blender公式チュートリアルを見て学習した内容覚え書き"
date:   2021-11-29 13:50:00 +0900
categories: blender
---

あつまれどうぶつの森、及びハッピーホームパラダイス熱が高まりすぎてついに[Blender](https://www.blender.org/)を使った3DCG制作の勉強を始めました。手始めにBlender公式が出している初心者向けチュートリアル動画(全４回)に沿ってフクロウのマスコットを作ったのでざっくり手順を書き留めていきます。

解説は全編英語のため字幕をつけたり、再生速度を少し落としてじっくり見ることをおすすめします。また、動画中で使っている機能の詳細な解説動画が紹介されているため適宜ご参照ください。

## 概形をつくる
- [Default Cube Owl Tutorial 1/4 Blocking](https://www.youtube.com/watch?v=4xLdisAvjx8&t=3s)
メッシュの追加(Shift + A)、視点移動(トラックパッド)、オブジェクトの移動(G)・回転(R)・拡縮(S)を使ってフクロウの概形を作っていきます。またミラーモディファイアーで対称形を作りやすくする、サブディビジョンモディファイアーで表面を滑らかにしていきます。

## 細部をつくる
- [Default Cube Owl Tutorial 2/4 Modeling](https://www.youtube.com/watch?v=LbQ6_D-wLQs&t=1s)
辺ループカット(Ctrl + R)、押し出し(E)、ベベル(Ctrl + B)を駆使して各パーツの詳細を作りこんでいきます。

## シェーディング
- [Default Cube Owl Tutorial 3/4 Shading](https://www.youtube.com/watch?v=eX3skhOOmco&t=37s)
シェーディングタブで色や陰影をつけます。マテリアルタブでベースカラーを設定したり、粗さや反射率の数値をいじって表面の質感を調整していきます。画像マテリアルをブランクで設定しておくと、UV展開後にテクスチャペイントタブでオブジェクトに直接を色を塗ることができます。UV展開はオブジェクトへ適切にシームをつけることで展開図がめちゃくちゃにならずに済みます。。。

## レンダリング
- [Default Cube Owl Tutorial 4/4 Rendering](https://www.youtube.com/watch?v=z-gTThdpho4)
カメラやライトの設定をいじってレンダリングしていきます。ライトは距離や光源の強さ・大きさ、色などを変えることができます。カメラ視点に移動するにはテンキー0、現在の視点にカメラを移動するにはcommand + option + 0でできます。

こうして実際に制作したフクロウの完成図がこちらです。
<img src="/images/box_owl.png" alt="box_owl" title="完成図">

今後も継続的にBlenderでやったことをまとめていく予定です。プロポーショナル編集やスカルプトなどが便利すぎてびっくりしたことなどが書け、書けるといいな……。