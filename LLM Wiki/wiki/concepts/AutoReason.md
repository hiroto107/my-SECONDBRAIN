---
type: wiki-concept
status: active
aliases:
  - autoreason
updated: 2026-04-15
source_pages:
  - "[[LLM Wiki/wiki/sources/2026-04-15 Source - Thread by @shannholmberg（AutoReason for Marketing）]]"
---

# AutoReason

## 要点

- AutoReason は、主観的タスクに対しても改善の再現性を上げるための multi-agent 反復方式。
- 中核は「批評」「再著述」「合成」「盲検評価」を役割分離し、同調バイアスを減らす設計。
- 勝者を incumbent として次ラウンドへ送り、置換が止まるまで反復する。

## 定義または輪郭

- 「1つの agent に改善を頼む」方式ではなく、対立構造と評価構造を明示的に入れた改善プロトコル。
- 典型フロー: `A -> critic -> B -> synthesis AB -> blind judges(Borda) -> winner as new A`。

## この wiki で重要な理由

- `AI支援型協働設計` の実務応用版として、運用可能な役割設計を提供する。
- `ラウンド型協働` を、議論収束だけでなく品質競争の仕組みへ拡張できる。
- マーケ・コピーのような主観領域でも、知識層（実績データ）を接続することで改善議論を実証寄りにできる。

## 関連ページ

- [[LLM Wiki/wiki/sources/2026-04-15 Source - Thread by @shannholmberg（AutoReason for Marketing）]]
- [[LLM Wiki/wiki/concepts/AI支援型協働設計]]
- [[LLM Wiki/wiki/concepts/ラウンド型協働]]
- [[LLM Wiki/wiki/entities/shannholmberg]]
- [[LLM Wiki/wiki/syntheses/2026-04-15 Synthesis - AutoReasonをマーケ実務に落とすときの設計要点]]

## 緊張関係 / 異説

- 盲検評価が機能しても、judge そのものが同質なら評価多様性が不足する。
- 反復回数を増やすほど品質が上がるとは限らず、過適合的な文体収束が起こりうる。
- 指標接続を強めるほど短期 KPI 偏重になり、ブランド長期価値と衝突する可能性がある。

## open question

- 停止条件（連続勝利回数）を、タスク難易度や媒体別にどう最適化すべきか。
- 複数 agent の役割定義をどこまで固定し、どこから学習的に更新すべきか。

## 根拠

- [[LLM Wiki/wiki/sources/2026-04-15 Source - Thread by @shannholmberg（AutoReason for Marketing）]]
- [[LLM Wiki/raw/clipping/Thread by @SHL0MS]]
