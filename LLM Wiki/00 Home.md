---
type: moc
status: active
domain:
  - AI
  - 日本文化
  - ホラー
---

# LLM Wiki Home

このフォルダは、`LLM` が継続的に保守するための自己完結型 wiki。

- 生の資料は `[[LLM Wiki/raw/README]]`
- 生成・更新される知識ページは `[[LLM Wiki/wiki/index]]`
- 運用ルールは `[[LLM Wiki/AGENTS]]`

既存の Vault はそのまま残し、この `LLM Wiki` 配下だけを「LLM が書く場所」として扱う。

## 使い始め方

1. 新しいソースを `[[LLM Wiki/raw/inbox/README]]` に置く  
   もしくは、既存の `clipping/` `読書メモ/` `PDF` などを「今回はソースとして使う」と LLM に明示する。
2. エージェントに `LLM Wiki/AGENTS.md` を読ませる。
3. `このソースを ingest して` と依頼する。
4. 更新結果を `[[LLM Wiki/wiki/overview]]` `[[LLM Wiki/wiki/index]]` `[[LLM Wiki/wiki/log]]` で確認する。

## 構成

- `[[LLM Wiki/AGENTS]]` : この wiki の保守ルール
- `[[LLM Wiki/raw/README]]` : raw source 層の説明
- `[[LLM Wiki/wiki/overview]]` : 現在の全体像と仮説
- `[[LLM Wiki/wiki/index]]` : コンテンツ目録
- `[[LLM Wiki/wiki/log]]` : 時系列ログ
- `[[LLM Wiki/_templates/source-summary]]` : source summary の雛形
- `[[LLM Wiki/_templates/entity-page]]` : entity page の雛形
- `[[LLM Wiki/_templates/concept-page]]` : concept page の雛形
- `[[LLM Wiki/_templates/synthesis-page]]` : synthesis page の雛形

## この Vault 向けの初期テーマ

いまの Vault から見ると、この wiki の最初の焦点は次の束になりやすい。

- `AI`
- `日本文化`
- `ホラー表現`
- `XR`
- `アニミズム / 多神教的世界観 / 幽玄 / 陰翳 / 間`

## 最初に ingest しやすい候補

- `[[Discordサーバー言葉設計_日本ホラー再構築]]`
- `[[reference]]`
- `[[ホラー表現]]`
- `[[アニミズム]]`
- `[[nullのテクスチャ]]`

## メモ

- raw source は原則 immutable。
- wiki は LLM が保守し、人間は方向づけとレビューを行う。
- よい問いへの回答は `wiki/syntheses/` に残して蓄積させる。
