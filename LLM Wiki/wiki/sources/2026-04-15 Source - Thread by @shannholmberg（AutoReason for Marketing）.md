---
type: wiki-source
status: active
source_path: "LLM Wiki/raw/clipping/Thread by @shannholmberg.md"
source_kind: social_thread
created: 2026-04-15
updated: 2026-04-15
---

# 2026-04-15 Source - Thread by @shannholmberg（AutoReason for Marketing）

## 要点

- テーマは「主観的なマーケティング判断に AutoReason を使う方法」。
- 従来の self-refine（同一系統の改善指示）で起こりがちな「自己肯定ループ」を避けるため、役割を分離した複数 agent 反復を採用する。
- 基本ループは `A初稿 -> Critic批評 -> B再著述 -> AB合成 -> 盲検Judge(Borda)` で、勝者を新しい A として次ラウンドへ送る。
- 停止条件は「A が2ラウンド連続で置換されないこと」。
- 価値は「make this better」型の単発改善ではなく、意図的に不一致を作ることにあると主張。
- 実運用では knowledge layer（過去キャンペーン指標、勝ち/負けコピー、顧客文脈、競合文脈、ブランド声）を入れることで、一般論ではなく自社データに anchored な改善が可能になる。
- ループ結果を知識ベースへ戻すことで、反復ごとに根拠が増える学習系になる。

## 主張

- 主観的タスク（ポジショニング、LPコピー、メール件名）にも、批評・再構成・盲検評価の構造を入れれば品質が安定しやすい。
- 役割隔離（critic と author の情報遮断、judge の盲検）により、単一会話で起きる同調バイアスを抑えられる。
- 定量指標が薄い領域でも、業務データを知識層に組み込むことで「議論の質」を高められる。

## 関連 entity

- [[LLM Wiki/wiki/entities/shannholmberg]]
- [[LLM Wiki/wiki/entities/Naval Ravikant]]

## 関連 concept

- [[LLM Wiki/wiki/concepts/AutoReason]]
- [[LLM Wiki/wiki/concepts/AI支援型協働設計]]
- [[LLM Wiki/wiki/concepts/ラウンド型協働]]
- [[LLM Wiki/wiki/concepts/バイブコーディング]]

## 更新候補

- 更新すべき entity page: `shannholmberg` を新設
- 更新すべき concept page: `AI支援型協働設計` に反証設計の観点を追記
- 新規で必要な synthesis: `マーケ文脈でのAutoReason運用ノート`

## open question

- 盲検 judge panel の信頼性をどこまで担保できるか（judge 多様性、評価基準固定、再現性）。
- 停止条件「2ラウンド連続勝利」はタスク難易度依存で、最適な閾値設計は別途検証が必要。
- 収益指標に接続したとき、短期最適化とブランド長期性のトレードオフをどう扱うか。

## 根拠

- [[LLM Wiki/raw/clipping/Thread by @shannholmberg]]
- [[LLM Wiki/raw/clipping/Thread by @SHL0MS]]
