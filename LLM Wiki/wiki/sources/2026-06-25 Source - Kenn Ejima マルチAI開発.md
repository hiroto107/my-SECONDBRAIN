---
type: wiki-source
status: active
source_path: 'LLM Wiki/raw/clipping/Kenn Ejima Codex Plan workflow.md'
source_kind: 'clipping / short raw alias'
created: 2026-06-25
updated: 2026-06-25
---

# 2026-06-25 Source - Kenn Ejima マルチAI開発

## 要点

- Codex Plan mode（High）で要件＋参考.md/SKILLを渡し、プラン作成。
- 実行前にPlan modeをOFFにし、プランを docs/ に書き出す。
- Claude Codeでプランをレビュー→Codexにフィードバック→収束まで往復。
- Cursor Composer 2 Fastで実装。staged/unstagedで差分を取捨選択。

## 主張

- Codex＝頭脳・司令塔、Composer＝爆速実装、Claude＝無駄削減の掃除屋。
- Plan modeを抜けずに書き出すと失敗する——モード切替が重要。
- 実装後もレビュー→plan trim→SKILL化で学習を蓄積。

## 関連 entity

- Kenn Ejima

## 関連 concept

- [[LLM Wiki/wiki/concepts/Agentic Engineering]]
- [[LLM Wiki/wiki/concepts/バイブコーディング]]
- [[LLM Wiki/wiki/concepts/メタスキル]]

## 更新候補

- 更新 concept: Agentic Engineering、バイブコーディング

## open question

- 自分の開発ワークフローに Plan→Review→Implement→SKILL化 をどう入れるか。

## 根拠

- [[LLM Wiki/raw/clipping/Kenn Ejima Codex Plan workflow]]
