# AI開発ポートフォリオ — Bold Industrial Impact

生成AIを使って制作したWebサイト・業務システム・ゲームの実績をまとめた、石原 健のポートフォリオサイトです。

公開URL: https://istyleken18-collab.github.io/portfolio-bold/

## 構成

| パス | 内容 |
|---|---|
| `index.html` | サイト本体。ビルド不要の静的HTML1ファイル |
| `images/hero.webp` | ヒーロー画像。GPT Image 2 で生成（2048×1152） |
| `images/bg.webp` | 背景テクスチャ。GPT Image 2 で生成（2048×2048） |
| `images/*.jpg` | 各実績のスクリーンショット |

外部のCDN・フォント・スクリプトを読み込まないため、`index.html` をブラウザで開くだけで動作します。

## デザイン

"Bold Industrial Impact" — 黒地 `#0a0a0a` に蛍光イエローグリーン `#d0ff00`。極太ゴシックを字間マイナスで組み、角丸を使わず、影はぼかし0のオフセットのみ。アニメーションは 0.1秒・`steps(2, end)` で段階的に切り替えます。

色とサイズは `index.html` 冒頭の CSS 変数（`:root`）にまとめてあります。

## 実績の追加・編集

`index.html` 内の `WORKS` 配列に1件ずつ定義しています。

```js
{ name:"作品名", cat:"カテゴリ",
  img:"images/xxx.jpg",   // 画像が無い場合は null
  desc:"一言説明",
  problem:"課題",
  made:"つくったもの",
  ai:"使ったAI", time:"制作時間",
  status:"進行中" }        // 省略可
```

`cat` に書いた値がそのまま絞り込みタグになります。画像は 4:3（推奨 1200×900px）で用意するとグリッドが揃います。

## 注意書き

掲載している店舗・ジムはすべて制作練習のための架空の店舗です。実在の団体・施設とは関係がありません。
