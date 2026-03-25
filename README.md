# Grid Lanes Demo

`display: grid-lanes` を使ったレイアウトデモです。通常の CSS Grid と `grid-lanes` を切り替えながら、可変サイズのタイルがどのように並ぶかを確認できます。

このリポジトリは、ICS MEDIA の記事
[CSSグリッド入門 - 図解でわかりやすく解説](https://ics.media/entry/15649/)
で説明するデモです。

## Overview

- `index.html`: 画像付きカードを並べたインタラクティブなデモ
- `simple-sample.html`: 最小構成のサンプル
- `images/`: デモで使用する画像アセット

ビルドツールや依存パッケージはありません。静的ファイルだけで動きます。

## Run

ビルドは不要です。ブラウザでそのまま開けます。

- `index.html` をブラウザで開くとメインのデモを確認できます。
- `simple-sample.html` をブラウザで開くと最小構成のサンプルを確認できます。

## Demo Controls

`index.html` では以下を切り替えられます。

- `Mode`: `Grid` と `Grid Lanes` の比較
- `Template`: 列幅パターンの切り替え
- `Flow Tolerance`: 詰め方と見た目の順序のバランス調整

カードは JavaScript で生成され、30 個のタイルに 12 枚の画像を繰り返し割り当てています。

## Notes

- `grid-lanes` は W3C の `CSS Grid Layout Module Level 3` で定義されている機能です。
- 2026年1月21日公開の最新版は Working Draft です。
- 非対応環境では `index.html` と `simple-sample.html` の両方で通常の `grid` 表示にフォールバックします。
- `index.html` では View Transitions API を使って切り替えアニメーションを行っています。

## License

MIT License. 詳細は [LICENSE](./LICENSE) を参照してください。
