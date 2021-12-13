---
layout: post
title:  "Blender Beginner Tutorial(椅子編)に挑戦"
date:   2021-12-13 17:00:00 +0900
categories: blender tutorial chair
---

ドーナツチュートリアル動画と同じくBlender Guruが投稿しているBlender初心者向けチュートリアル動画を参考に椅子をモデリングしました。

## 椅子の脚をつくる
- [Blender Beginner Modelling Tutorial Part 1](https://www.youtube.com/watch?v=Hf2esGA7vCc)　〜　

製作するのはボーエ・モーエンセンがデザインしたソボーチェアと呼ばれる椅子です。家具メーカーのフレデリシアから販売されており，[フレデリシアの公式サイト](https://www.fredericia.com/products/by-designer-børge-mogensen/søborg-wood-base-1.aspx?PID=63&catid=6219)からソボーチェアのCADファイルを手に入れることができます。ここから得た3面図を基に椅子のモデリングをしていきましょう。動画ではサブサーフモディファイアと辺ループカットで角を滑らかに
表現する方法を紹介しています。



## 椅子の座面をつくる
- [Blender Beginner Modelling Chair Tutorial Part 4: Modifier Mayhem](https://www.youtube.com/watch?v=BgY3QMXQYLI)　〜　

滑らかにしたい辺と角度を保ちたい辺を区別するために「シャープをマーク」と自動スムーズ機能を利用します。実際にカクついた部分がないか確認するには3DレンダービューでMatCapを利用すると視覚的にわかりやすいです。

## 椅子の貫(脚同士を繋ぐパーツ)をつくる
- [Blender Beginner Modeling Chair Tutorial Part 6: Creases & Shearing](https://www.youtube.com/watch?v=KzA5fOIq8Qw)　〜　

ここでは貫と脚を繋ぐ面を鋭く保つために「辺のクリース」を使っています。サブサーフモディファイアを使用する際にどの程度エッジを丸めるかを調節することができます。辺のクリースを設定した辺は紫に着色されます。Guruはこの方法をあまり好まないようで辺ループカットによるエッジの調節を勧めています。



ここに木目のテクスチャをつけた画像がこちらです。

<img src="/images/chair_rendered12.png" alt="chair" title="chair">


ドーナツより文量は短くなりましたが実作業時間としては椅子の方がずいぶんかかりました……。次はソファ編を頑張ります。