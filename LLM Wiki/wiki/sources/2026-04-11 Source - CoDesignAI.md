---
type: wiki-source
status: active
source_path: "LLM Wiki/raw/codeshgin.pdf"
source_kind: "research paper (pdf)"
created: 2026-04-11
updated: 2026-04-11
---

# 2026-04-11 Source - CoDesignAI

## 要点

- `CoDesignAI` は、複数ユーザーと複数 AI agent を同じ場に入れて参加型都市デザインを支援する proof-of-concept の web platform。
- 中核は `AI facilitator` で、議論を要約し、共有意図を抽出し、画像生成用の prompt へ変換する。
- 協働は `round-based` に設計されており、全員の発話が揃ってから AI が synthesize する。
- Google Street View を現実空間の土台にし、Gemini 2.5 Flash / Flash Image を使って設計案を画像として反映する。
- 論文の価値は完成品の提示よりも、`AI が協働の場をどう構造化するか` を具体的なシステム設計として示した点にある。

## 主張

- LLM は個人への応答だけでなく、複数人の協働を媒介する `facilitator` として機能しうる。
- 議論を `ラウンド` と `共有状態` で管理すると、公平性、トレーサビリティ、一貫性を上げやすい。
- AI を discussion layer と image generation layer のあいだに置くことで、会話を設計案へ変換しやすくなる。
- ただし現段階では、包摂性、スケーラビリティ、コスト、真の同期協働、利害対立の調停は未解決のまま残っている。

## 関連 entity

- [[LLM Wiki/wiki/entities/CoDesignAI]]

## 関連 concept

- [[LLM Wiki/wiki/concepts/AIファシリテーター]]
- [[LLM Wiki/wiki/concepts/ラウンド型協働]]
- [[LLM Wiki/wiki/concepts/AI支援型協働設計]]

## 更新候補

- 更新すべき entity page: `CoDesignAI`
- 更新すべき concept page: `AIファシリテーター` `ラウンド型協働` `AI支援型協働設計`
- 新規で必要な synthesis: `AIは協働の場をどう支えるか`

## open question

- この設計は都市デザイン以外の創作、研究、コミュニティ運営にどこまで転用できるか。
- facilitator が合意形成を担うとき、少数意見や対立をどのように保存すべきか。
- round-based 協働は公平性を上げる一方で、速度や spontaneity をどれだけ犠牲にするか。

## 根拠

- [[LLM Wiki/raw/codeshgin.pdf]]
