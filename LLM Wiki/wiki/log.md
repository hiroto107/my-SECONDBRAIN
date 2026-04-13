---
type: log
status: active
---

# log

append-only の時系列ログ。

## [2026-04-11] setup | LLM Wiki scaffold

- `LLM Wiki/` を新規作成。
- `raw/` `wiki/` `_templates/` の基本構成を用意。
- `AGENTS.md` を追加し、ingest / query / lint の運用ルールを定義。
- `overview.md` `index.md` を追加。
- 既存 Vault の主題である `AI` `日本文化` `ホラー` `XR` を初期焦点として設定。
- まだ raw source の ingest は実行していない。

## [2026-04-11] import | from-vault unorganized notes

- `MOC/未整理インボックス.md` を基準に、既存 Vault の未整理候補を確認。
- 既存リンクを壊さないため、物理移動ではなく `LLM Wiki/raw/from-vault/` へ複製。
- `読書メモ` `単発メモ` `思想` `日本文化` `アイデア` から合計 21 件を raw source copy として追加。
- すでに `LLM Wiki/raw/clipping/` に存在していた clipping 系は重複取り込みしなかった。
- `読書メモ/ゆるすといっく` `読書メモ/越境3.0` `偶然思いついたアイデア/ディズニーのような壮大なBGMを科学したい` は元ファイル未検出のため未取り込み。

## [2026-04-11] ingest | CoDesignAI

- `[[LLM Wiki/raw/codeshgin.pdf]]` を source として読解。
- `[[LLM Wiki/wiki/sources/2026-04-11 Source - CoDesignAI]]` を作成。
- 関連 page として `[[LLM Wiki/wiki/entities/CoDesignAI]]` `[[LLM Wiki/wiki/concepts/AIファシリテーター]]` `[[LLM Wiki/wiki/concepts/ラウンド型協働]]` `[[LLM Wiki/wiki/concepts/AI支援型協働設計]]` を追加。
- 抽出知見を保存するため `[[LLM Wiki/wiki/syntheses/2026-04-11 Synthesis - AIは協働の場をどう支えるか]]` を追加。
- `overview.md` と `index.md` を更新し、この source から立ち上がった論点を反映。
- `[[LLM Wiki/raw/怨霊.pdf]]` は文字抽出が崩れており、今回の ingest 対象からは外した。必要なら OCR かテキスト化が必要。

## [2026-04-11] ingest | 御霊信仰の諸相

- `[[LLM Wiki/raw/怨霊.pdf]]` の OCR テキスト層を PDFKit 経由で確認し、本文読解が可能であることを確認。
- source summary として `[[LLM Wiki/wiki/sources/2026-04-11 Source - 御霊信仰の諸相]]` を作成。
- 関連 page として `[[LLM Wiki/wiki/entities/菅原道真]]` `[[LLM Wiki/wiki/concepts/御霊信仰]]` `[[LLM Wiki/wiki/concepts/怨霊]]` を追加。
- 抽出知見を保存するため `[[LLM Wiki/wiki/syntheses/2026-04-11 Synthesis - 怨霊はどのように御霊へ変わるか]]` を追加。
- `overview.md` と `index.md` を更新し、日本文化 / ホラー / 鎮魂の軸を強化。

## [2026-04-11] ingest | アニミズムと日本コンテンツへの影響

- `[[LLM Wiki/raw/animism_report.pdf]]` を source として読解。
- source summary として `[[LLM Wiki/wiki/sources/2026-04-11 Source - アニミズムと日本コンテンツへの影響]]` を作成。
- 関連 page として `[[LLM Wiki/wiki/concepts/アニミズム]]` `[[LLM Wiki/wiki/concepts/テクノアニミズム]]` を追加。
- 抽出知見を保存するため `[[LLM Wiki/wiki/syntheses/2026-04-11 Synthesis - アニミズムは日本コンテンツに何をもたらすか]]` を追加。
- 既存 page との接続として `[[LLM Wiki/wiki/concepts/御霊信仰]]` `[[LLM Wiki/wiki/concepts/怨霊]]` `[[LLM Wiki/wiki/concepts/AI支援型協働設計]]` に関連リンクを追加。
- `overview.md` と `index.md` を更新し、日本文化 / コンテンツ / AI の橋渡しとしてアニミズム軸を反映。
