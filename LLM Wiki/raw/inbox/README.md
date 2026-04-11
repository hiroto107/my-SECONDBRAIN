---
type: guide
status: active
---

# Inbox

新しく ingest する前の raw source を置く場所。

## 想定フロー

1. Web Clipper や PDF などをここへ入れる
2. LLM に source を指定して ingest を依頼する
3. LLM が `wiki/` 側へ summary と cross-reference を作る
4. raw source 自体はそのまま残す

## メモ

- 1 source ごとに 1 file か 1 folder にまとまっていると扱いやすい。
- 長いタイトルでも問題ない。
- 画像が多い source は `raw/assets/` と組み合わせてよい。
