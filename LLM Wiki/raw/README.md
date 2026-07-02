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

## ディレクトリ

| フォルダ | 用途 |
|---|---|
| `inbox/` | 新規投入の入口。ingest 後は `clipping/` か `from-vault/` へ移す |
| `clipping/` | 外部由来の資料（Web Clipper、YouTube、X、PDF など） |
| `from-vault/` | Vault 内既存ノートのコピー（読書メモ、アイデア、思想など） |
| `assets/` | 画像・添付 |

外部資料はすべて `clipping/` に置く。`raw/` 直下にはファイルを置かない。

## 入口

- `[[LLM Wiki/raw/inbox/README]]`
- `[[LLM Wiki/raw/assets/README]]`

## 補足

Vault 内の `Clippings/` は Clipper の置き場としてそのまま使う。ingest 時に `clipping/` へコピーする。  
`読書メモ/` など Vault 内ノートは ingest 時に `from-vault/` へコピーする。  
Vault 内の元ノートは、明示依頼なしに編集しない。
