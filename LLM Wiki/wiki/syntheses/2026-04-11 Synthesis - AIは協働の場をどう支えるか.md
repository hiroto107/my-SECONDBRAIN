---
type: wiki-synthesis
status: active
question: "AIは複数人の協働の場でどのような役割を担えるか"
source_pages:
  - "[[LLM Wiki/wiki/sources/2026-04-11 Source - CoDesignAI]]"
updated: 2026-04-11
---

# 2026-04-11 Synthesis - AIは協働の場をどう支えるか

## 問い

- AI は、複数人が何かを一緒につくる場で、具体的にどの役割を担えるのか。

## 短い答え

- CoDesignAI が示しているのは、AI は `答えを出す係` だけでなく、`議論を進行する係` `会話を構造化する係` `専門視点を差し込む係` `会話を次の artifact へ変換する係` として機能しうる、ということ。

## 重要ポイント

- `facilitator` として、複数人の発話を要約し共通 ground を探す。
- `expert agent` として、専門視点を on demand で差し込む。
- `prompt parser` として、曖昧な議論を実行可能な指示へ圧縮する。
- `memory keeper` として、ラウンドをまたいだ文脈を保持する。
- `artifact bridge` として、会話を画像や次の作業単位へ接続する。

## 比較 / 構造化

- 個人向け chatbot:
  主に 1対1 の応答最適化。
- AIファシリテーター:
  複数人の関係性と進行を扱う。
- AI支援型協働設計:
  会話、記憶、外部ツール、生成物を1つの workflow にまとめる。
- ラウンド型協働:
  その workflow を公平性と整合性が出るように制御する手法。

## 含意

- AI の価値は `うまい答え` だけではなく、`人間同士の協働をどれだけ前に進められるか` にもある。
- LLM Wiki でも、AI を source summary writer としてだけでなく、index 管理、論点抽出、次の問い提案、矛盾検知を担う facilitator とみなせる。
- ただし、合意形成の効率化は少数意見の圧縮や power imbalance の不可視化を伴いうる。

## 次に読むページ

- [[LLM Wiki/wiki/entities/CoDesignAI]]
- [[LLM Wiki/wiki/concepts/AIファシリテーター]]
- [[LLM Wiki/wiki/concepts/ラウンド型協働]]
- [[LLM Wiki/wiki/concepts/AI支援型協働設計]]

## open question

- facilitator が見落とした対立を、別 agent が補足する設計は可能か。
- 会話から画像以外の artifact へ接続する場合、どの中間形式が最も有効か。
- 知識 wiki と共同制作 workspace はどこまで統合できるか。

## 根拠

- [[LLM Wiki/wiki/sources/2026-04-11 Source - CoDesignAI]]
- [[LLM Wiki/raw/codeshgin.pdf]]
