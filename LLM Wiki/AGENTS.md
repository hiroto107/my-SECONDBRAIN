# LLM Wiki Agent Schema

このファイルは `LLM Wiki/` 配下を保守するエージェント向けの運用仕様。

## 役割

あなたの役割は、raw source から知識を抽出し、`LLM Wiki/wiki/` を継続的に育てること。

- 人間は source の選定、論点の指定、レビューを担当する。
- LLM は要約、リンク付け、差分反映、横断整理、ログ更新を担当する。

## 作業範囲

- 通常の編集対象は `LLM Wiki/` 配下のみ。
- `LLM Wiki/raw/` は source layer なので読んでよいが編集しない。
- Vault 内の既存ノート (`clipping/` `読書メモ/` など) は、ユーザーが明示したときだけ source として読む。
- `LLM Wiki/` 外の既存ノートは、明示指示がない限り更新しない。

## ディレクトリの意味

- `LLM Wiki/raw/inbox/` : 新しく追加された raw source
- `LLM Wiki/raw/assets/` : source に付随する画像など
- `LLM Wiki/wiki/sources/` : source ごとの summary
- `LLM Wiki/wiki/entities/` : 人物、作品、組織、場所、媒体などの page
- `LLM Wiki/wiki/concepts/` : 概念、テーマ、モチーフ、論点の page
- `LLM Wiki/wiki/syntheses/` : 比較、分析、問いへの回答、仮説整理
- `LLM Wiki/wiki/index.md` : コンテンツ目録
- `LLM Wiki/wiki/log.md` : 時系列ログ
- `LLM Wiki/wiki/overview.md` : 現時点の全体像
- `LLM Wiki/_templates/` : 雛形

## 基本原則

1. raw source は immutable とみなす。
2. 同じことを複数ページに重複して書きすぎない。既存 page を更新できるなら更新を優先する。
3. 新しい情報が既存の記述と衝突する場合は、上書きで隠さず「何がどう食い違うか」を明示する。
4. 推測は事実と分けて書く。
5. 曖昧な点や不足情報は、そのまま `open question` として残してよい。
6. 重要な回答や比較は chat に閉じ込めず `wiki/syntheses/` に保存する。

## ページ規約

- 可能なら YAML frontmatter を付ける。
- Obsidian の wikilink を使う。
- section 名は日本語でよい。
- 断定的な主張には、根拠 source を末尾の `## 根拠` に並べる。
- source summary には `## 要点` `## 主張` `## 関連 entity` `## 関連 concept` `## 更新候補` を含める。
- entity / concept page には `## 要点` `## 定義または輪郭` `## この wiki で重要な理由` `## 関連ページ` `## 根拠` を基本として使う。

## 命名

- source summary : `YYYY-MM-DD Source - タイトル`
- entity page : 自然な固有名詞
- concept page : 自然な概念名
- synthesis page : `YYYY-MM-DD Synthesis - テーマ`

日本語タイトルでよい。ASCII slug には統一しなくてよい。

## Ingest Workflow

新しい source を ingest するときは、原則として次を行う。

1. source を読む。必要なら画像も別途確認する。
2. ユーザーと重点を短くすり合わせる。
3. `wiki/sources/` に source summary を作る。
4. 既存の entity / concept / synthesis page への影響を洗い出す。
5. 必要な page を更新または新規作成する。
6. `wiki/overview.md` に大局的な変化があれば反映する。
7. `wiki/index.md` を更新する。
8. `wiki/log.md` に append-only で記録する。

source 1件で 1ページしか触らないのは例外であり、必要なら複数ページを同時更新してよい。

## Query Workflow

質問に答えるときは、原則として次を行う。

1. まず `wiki/index.md` と `wiki/overview.md` を読む。
2. 関連 page を特定して読む。
3. 回答では、どの page と source に依拠したかを明確にする。
4. 再利用価値がある答えなら `wiki/syntheses/` に保存する提案を行うか、ユーザーが望めば保存する。

## Lint Workflow

lint / health-check を頼まれたら、次を確認する。

- 相互に矛盾する記述
- 新しい source で古くなった主張
- 孤立している page
- 頻出するのに page がない概念や entity
- つながっていない cross-reference
- 追加調査で埋まりそうな data gap

必要なら `wiki/syntheses/` に `Lint` note を作ってもよい。

## index.md の更新ルール

- page を作ったら同じセッション中に必ず `index.md` を更新する。
- 各項目は `リンク + 1行説明` を基本にする。
- section は `overview / sources / entities / concepts / syntheses` を維持する。

## log.md の更新ルール

- `log.md` は append-only。
- 各 entry は次の形式を基本にする。

`## [YYYY-MM-DD] operation | title`

- 箇条書きで、何を読んだか、何を更新したか、未解決は何かを残す。

## 禁止事項

- raw source の改変
- 出典不明の断定
- 既存 page を読まずに似た page を量産すること
- ユーザーの明示なしに `LLM Wiki/` 外のノートを書き換えること

## 最初に読むべきファイル

この schema を読んだら、通常は次を先に確認する。

1. `LLM Wiki/00 Home.md`
2. `LLM Wiki/wiki/overview.md`
3. `LLM Wiki/wiki/index.md`
4. `LLM Wiki/wiki/log.md`
