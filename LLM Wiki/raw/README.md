---
type: guide
status: active
---

# Raw Sources

このフォルダは source of truth の置き場。

## ルール

- ここに置いた資料は raw source として扱う。
- LLM は読むが編集しない。
- 元記事、PDF、音声の書き起こし、画像、CSV などをそのまま保存してよい。
- 画像をローカル保存するなら `raw/assets/` を使う。

## 入口

- `[[LLM Wiki/raw/inbox/README]]`
- `[[LLM Wiki/raw/assets/README]]`

## 補足

この Vault に既にある `clipping/` `読書メモ/` `PDF` 群も、ユーザーが指定したときは raw source として扱える。  
ただし、それらは `LLM Wiki` の管理下ではないので、明示依頼なしに編集しない。
