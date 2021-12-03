---
layout: post
title:  "Blender Beginner Tutorial に挑戦 Lv.1"
date:   2021-12-03 15:30:00 +0900
categories: blender tutorial donut
---

前回に引き続きBlenderを使ったCG制作を行ないました。友人曰く、「Blenderを学ぶものはまずドーナツを作らなければならない」とのこと。

[Blender Begginer Tutorial Series](https://www.youtube.com/playlist?list=PLjEaoINr3zgEq0u2MzVgAaHEBt--xLB6U)

こちらの動画に沿ってドーナツを作り、新たに学んだことを全４回に分けて書き留めていきます。

解説はやっぱり全編英語のため字幕をつけたり、再生速度を少し落としてじっくり見ることをおすすめします。

## ドーナツの概形をつくる
- [Part 2, Level 1: Modelling Beginner Blender Tutorial Series](https://www.youtube.com/watch?v=RaT-uG5wgUw)

なるべく現実のサイズに近づける、という発想が無かったので目から鱗でした。現実の画像やVR空間との兼ね合いを考えればそれはそうだ。

また，ここでは"Computers make things that are perfect, and in the real world they're not. That's why imperfection is the virtual perfection."という引用の元に整ったトーラスにデコボコをつけていきます。

この時に紹介されたプロポーショナル編集機能がすごい。対象を中心に指定した範囲の大きさで変形を行うことができます。細かく対象を指定しなくとも直感的にこの辺をふくらませたい／へこませたい、という操作が可能になります。


## ドーナツにアイシングをかける
- [Part 3, Level 1: Modifiers Blender Beginner Tutorial](https://www.youtube.com/watch?v=R2qjqqfkH6E)

メッシュから選択した範囲をコピー(Shift + D)、別のオブジェクトとして分離(P)することでドーナツにぴったりくっついたアイシング部分を作成します。キャラクターの服飾なんかにも使えそうですね。

面のままでは薄すぎるのでソリッド化モディファイアを追加してアイシングに厚みを作ってやります。他のモディファイアとの適用順によって変形が異なるので確認しておきましょう。


## アイシングを側面に垂らす（ペアレント・スナップ）
- [Part 4, Level 1: Modelling Blender Beginner Tutorial](https://www.youtube.com/watch?v=jmSgsaNSQ6s)

アイシング部はドーナツ部に追従して欲しいので、ドーナツを親、アイシングを子としてペアレント関係を設定します。
ドーナツにでこぼこをつけた時と同様に、プロポーショナル編集を用いてアイシングのふちを垂れさせます。移動させたくないふち以外の部分は一時的に非表示(H)にしておきます。

またドーナツ内にふちが沈んでしまわないよう、トランスフォーム時のスナップを設定(磁石マーク)しふちがドーナツの面に沿って動くようにします。移動（G）だけでなく押し出し(E)も使うとそれらしくなります。

## スカルプト
- [Part 5, Level 1: Sculpting Blender Beginner Tutorial](https://www.youtube.com/watch?v=6OTX3ZdYvEA)

スカルプトタブに移動してドーナツの側面に溝を入れたり凹ませたり膨らませたりとがらせたり丸めたりします。何せメッシュがまるで粘土のように扱えるのでできることが多すぎる。無法。メッシュのワイヤーフレームとスカルプトタブを反復横跳びして永遠に理想のドーナツを追い求めることができます。

## マテリアル
- [Part 7, Level 1: Materials Blender Beginner Tutorial](https://www.youtube.com/watch?v=5lr8QnR5WWU)

ライトやカメラ、基準になる平面を追加したら、ドーナツとアイシングそれぞれにマテリアルを追加して色をつけます。
ここまで実際に作ってレンダリングしたドーナツがこちらです。
<img src="/images/proto_donut.png" alt="proto_donut" title="level1">

次回シリーズではアイシングにトッピングを追加していきます。

