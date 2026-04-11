---
type: wiki-entity
status: active
aliases: []
source_pages:
  - "[[LLM Wiki/wiki/sources/2026-04-11 Source - CoDesignAI]]"
updated: 2026-04-11
---

# CoDesignAI

## 要点

- `CoDesignAI` は、参加型都市デザインのための multi-user / multi-agent web platform。
- 人間の参加者に加えて、`AI facilitator` と optional な expert agents を同じ協働空間へ入れる。
- Google Street View を現実文脈として使い、会話から prompt を生成し、設計案の可視化までつなげる。

## 輪郭

- 完成した商用ツールというより、`AI が複数人の協働をどう媒介できるか` を検証する prototype。
- system architecture は participant layer / backend coordination / AI service / storage の4層で構成される。
- AI facilitator は議論の交通整理、expert agents は専門視点の補助、image generation は合意案の可視化を担う。

## この wiki で重要な理由

- `AI を答える存在から、場を進行する存在へずらす` 具体例として重要。
- `会話 -> 要約 -> 構造化 prompt -> 画像化 -> 次ラウンド` という累積ワークフローが、LLM Wiki 的な知識運用にも通じる。
- 協働設計、multi-agent、memory、共有ワークスペースといった論点を1つの実装例に束ねている。

## 関連ページ

- [[LLM Wiki/wiki/sources/2026-04-11 Source - CoDesignAI]]
- [[LLM Wiki/wiki/concepts/AIファシリテーター]]
- [[LLM Wiki/wiki/concepts/ラウンド型協働]]
- [[LLM Wiki/wiki/concepts/AI支援型協働設計]]
- [[LLM Wiki/wiki/syntheses/2026-04-11 Synthesis - AIは協働の場をどう支えるか]]

## 緊張関係 / 異説

- 参加の包摂性を高める狙いはあるが、現時点では実地の包摂性検証がまだ薄い。
- 多数の参加者を扱える可能性は示すが、スケール時の token cost や運用コストは未評価。
- multi-agent を採用しているが、agent 間の本格的な conflict mediation までは踏み込んでいない。

## open question

- urban design 以外の分野で、どの役割をそのまま移植できるか。
- facilitator と expert agents の責務分離は、どの粒度が最も有効か。
- 共有空間の設計は、テキスト中心より canvas / graph 型の方が適する場面があるか。

## 根拠

- [[LLM Wiki/wiki/sources/2026-04-11 Source - CoDesignAI]]
- [[LLM Wiki/raw/codeshgin.pdf]]
