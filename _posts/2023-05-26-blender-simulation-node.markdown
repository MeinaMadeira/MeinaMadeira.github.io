---
layout: post
title:  "Simulation Zone(シミュレーションノード)について"
date:   2023-05-26 17:45:00 +0900
categories: blender
---

現在Blenderではバージョン3.6がα版で提供されています。今回はこの3.6で新たに追加された新機能「Simulation Zone(シミュレーションノード)」に触れてみた所感を書いていこうと思います。

## Simulation Zoneは何をするのか。
Simulation Zoneとはジオメトリノードに追加される機能で、あるフレームでの計算結果が次のフレームに影響を与えられるようになります。
たとえばこちらのキューブ、


<img src="/images/example_cube.png" alt="適用例" title="適用例">


これにSimulation Zoneを使ったジオメトリノードを適用するとします。
<img src="/images/sim_io.png" alt="simulation_zone1" title="Simulation Zone1">


Simulation Zoneのインプットとアウトプットの間に位置設定ノードでx方向へ0.1mのオフセットを指定します。
<img src="/images/sim_io2.png" alt="simulation_zone2" title="Simulation Zone2">


すると1フレームごとにx方向へ0.1mずつ移動するキューブのアニメーションが生成されます。
<video src="/images/sim_movie.mp4" width="750" controls loop></video>



つまりSimulation Zoneを使えば、どんなオブジェクトにもジオメトリノードで任意の変化量を与えたアニメーションを自動生成できることになります。

## Simulation Zoneで何ができるのか
すでに多くの方がSimulation Zoneを使った作例を発表していますが、私がSimulation Zoneを知って触れてみようと思ったきっかけの動画がこちらです。

<iframe width="100%" height="315" src="https://www.youtube.com/embed/h5_uA9sOw7g" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

はじめはクロスかソフトボディのシミュレーションとジオメトリノードの組み合わせかな？と思っていたため、ジオメトリノードだけでこの複雑なアニメーションが実現されていることに度肝を抜かれました。全編英語ですが、非常に勉強になったので興味が出てきたという方にはぜひ見ていただきたいです。

## 所感
Simulation Zoneはそのアニメーションを構成するノードとそのすべてのパラメータを自分で設定できることから、理解して使うことができれば大変強力な機能だと感じました。自分の作品に生かせるよう、積極的に学習や情報収集をしたいと思います。

## 参考資料
- [Blender公式ドキュメント](https://docs.blender.org/manual/ja/3.6/modeling/geometry_nodes/simulation/simulation_zone.html)
- [Simulation Nodes String Physics (Blender 3.6)](https://www.youtube.com/embed/h5_uA9sOw7g)　


