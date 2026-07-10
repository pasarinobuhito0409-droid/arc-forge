# ARC FORGE v2.1 デルタ仕様（マスター: C:\Users\今林拓也\forge-standard\FORGE_V2.md）

対象: `C:\Users\今林拓也\arc-forge\`。現状v2.0（フル装備級＋🔬金属の目あり）。
**追加＝PASSPORT・現場の目・新機能5・XP。既存演出/本文/ドリル/金属の目/マップは変更禁止。**
注意: 進捗キーは `arc-forge-v2`（他アプリと違う）。

## D1 📷現場の目 PHOTOS（写真配置済み）

```js
const PHOTOS = {
 l1:{img:"assets/photo/a1.jpg",title:"本物のTIG溶接",
  cap:"タングステン電極の先の青白い光がアーク＝電気のプラズマ。火花（スパッタ）が出ないのがTIGの証拠。",
  points:[{x:50,y:45,t:"アーク＝約2万℃のプラズマ"}],
  credit:"写真: Mak04（Public domain／Wikimedia Commons）", vq:"TIG溶接 アーク"},
 l2:{img:"assets/photo/a2.jpg",title:"パイプの溶接ビード",
  cap:"うろこ模様は運棒のリズムの指紋。等間隔＝一定速度の証拠。ビードを見れば腕がわかる。",
  points:[{x:50,y:50,t:"うろこ＝速度の指紋"}],
  credit:"写真: Newfoundlandguy（CC BY-SA 4.0／Wikimedia Commons）", vq:"溶接ビード うろこ きれい"},
 l4:{img:"assets/photo/a3.jpg",title:"接合ロボット",
  cap:"摩擦攪拌点接合ロボ（火を使わず摩擦熱で接合する溶接の仲間）。接合はロボット化の最前線——設計指示がロボの動きになる。",
  points:[{x:50,y:40,t:"ツール先端の摩擦熱で接合"}],
  credit:"写真: Balasubramaniam et al.（CC BY 4.0／Wikimedia Commons）", vq:"溶接ロボット 自動化"},
 l6:{img:"assets/photo/a4.jpg",title:"実作業の火花",
  cap:"アーク溶接のスパッタ（飛び散る溶滴）。保護具の理由が一目でわかる。設計者が継手と姿勢を工夫するとスパッタも減る。",
  points:[{x:50,y:45,t:"スパッタ＝飛び散る溶滴"}],
  credit:"写真: Juan F. Jimenez（Public domain／Wikimedia Commons）", vq:"アーク溶接 スパッタ 対策"}
};
```
（既存レッスンIDに合わせて最適割当に変更可＝報告書に記載）

## D2 ガチャ超レア演出（溶接オリジナル）

金のアークがロゴを一周してビードを描き、テンパーカラー（金→紫→青）が走る（2秒）。称号「アークの神」。

## D3 その他

- PASSPORT移植（自キー`arc-forge-v2`）。既存RQ登録をv2ペイロード化。
- サビマップ: 既存マップ（溶接街道）ノードに適用。ドリルtag（kigo/kyaku/hizumi/tsugite/kekkan/anzen）→レッスン対応表を作成し報告書に記載。
- 新キー: `arc-forge-fresh-v1`。既存キー変更禁止。
