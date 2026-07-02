---
type: wiki-source
status: active
source_path: "LLM Wiki/raw/clipping/Thread by @SHL0MS.md"
source_kind: "x thread (markdown clipping)"
created: 2026-04-20
updated: 2026-04-20
---

# 2026-04-20 Source - Thread by @SHL0MS（AutoReason）

## 要点

- `AutoReason` は、主観的タスクでの iterative self-refinement が劣化しやすいという問題に対する reasoning method として提示されている。
- 単純な critique-and-revise は、存在しない欠点を hallucinate し、scope を拡張し、変更不要な場面でも改変し続ける傾向があると主張される。
- AutoReason では incumbent と challenger の競争、AB synthesis、judge による比較を通じて、`本当に安定した output` に到達することを重視している。
- 収束は `モデルが言うことを失うから` ではなく、`出力が genuinely stable になったから` 起きるべきだとされる。
- 安価なモデルでも baseline より高い評価を出せる可能性が示され、prompt の工夫より protocol 設計が重要だという含意を持つ。

## 主張

- subjective domain では、自己批評を重ねるほど品質が上がるとは限らない。
- refinement loop には、批評と判断を分離し、比較と置換を明示する protocol が必要である。
- 改善は単線的な revise ではなく、複数候補の競争と synthesis によって進める方が安定しやすい。

## 関連 entity

- 特になし

## 関連 concept

- [[LLM Wiki/wiki/concepts/AutoReason]]
- [[LLM Wiki/wiki/concepts/AI支援型協働設計]]

## 更新候補

- 更新すべき entity page: 特になし
- 更新すべき concept page: `AutoReason` `AI支援型協働設計`
- 新規で必要な synthesis: 特になし

## open question

- subjective task ごとの convergence 判定は、どこまで一般化できるか。
- human judge を含まない場合でも同等の安定性を維持できるか。
- creative writing や worldbuilding での効用は marketing task と同程度か。

## 根拠

- [[LLM Wiki/raw/clipping/Thread by @SHL0MS]]
