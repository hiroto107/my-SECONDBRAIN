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

- `[[LLM Wiki/raw/clipping/codeshgin.pdf]]` を source として読解。
- `[[LLM Wiki/wiki/sources/2026-04-11 Source - CoDesignAI]]` を作成。
- 関連 page として `[[LLM Wiki/wiki/entities/CoDesignAI]]` `[[LLM Wiki/wiki/concepts/AIファシリテーター]]` `[[LLM Wiki/wiki/concepts/ラウンド型協働]]` `[[LLM Wiki/wiki/concepts/AI支援型協働設計]]` を追加。
- 抽出知見を保存するため `[[LLM Wiki/wiki/syntheses/2026-04-11 Synthesis - AIは協働の場をどう支えるか]]` を追加。
- `overview.md` と `index.md` を更新し、この source から立ち上がった論点を反映。
- `[[LLM Wiki/raw/clipping/怨霊.pdf]]` は文字抽出が崩れており、今回の ingest 対象からは外した。必要なら OCR かテキスト化が必要。

## [2026-04-11] ingest | 御霊信仰の諸相

- `[[LLM Wiki/raw/clipping/怨霊.pdf]]` の OCR テキスト層を PDFKit 経由で確認し、本文読解が可能であることを確認。
- source summary として `[[LLM Wiki/wiki/sources/2026-04-11 Source - 御霊信仰の諸相]]` を作成。
- 関連 page として `[[LLM Wiki/wiki/entities/菅原道真]]` `[[LLM Wiki/wiki/concepts/御霊信仰]]` `[[LLM Wiki/wiki/concepts/怨霊]]` を追加。
- 抽出知見を保存するため `[[LLM Wiki/wiki/syntheses/2026-04-11 Synthesis - 怨霊はどのように御霊へ変わるか]]` を追加。
- `overview.md` と `index.md` を更新し、日本文化 / ホラー / 鎮魂の軸を強化。

## [2026-04-11] ingest | アニミズムと日本コンテンツへの影響

- `[[LLM Wiki/raw/clipping/animism_report.pdf]]` を source として読解。
- source summary として `[[LLM Wiki/wiki/sources/2026-04-11 Source - アニミズムと日本コンテンツへの影響]]` を作成。
- 関連 page として `[[LLM Wiki/wiki/concepts/アニミズム]]` `[[LLM Wiki/wiki/concepts/テクノアニミズム]]` を追加。
- 抽出知見を保存するため `[[LLM Wiki/wiki/syntheses/2026-04-11 Synthesis - アニミズムは日本コンテンツに何をもたらすか]]` を追加。
- 既存 page との接続として `[[LLM Wiki/wiki/concepts/御霊信仰]]` `[[LLM Wiki/wiki/concepts/怨霊]]` `[[LLM Wiki/wiki/concepts/AI支援型協働設計]]` に関連リンクを追加。
- `overview.md` と `index.md` を更新し、日本文化 / コンテンツ / AI の橋渡しとしてアニミズム軸を反映。

## [2026-04-19] ingest | INFOPRO 2025 落合陽一講演

- `[[LLM Wiki/raw/clipping/INFOPRO 2025 特別講演レポート：落合陽一さん「計算機自然における情報の生成論 ― 生成AI時代の審美眼と環境構築の実践」 ｜一般社団法人 情報科学技術協会（INFOSTA）]]` を source として読解。
- source summary として `[[LLM Wiki/wiki/sources/2026-04-19 Source - INFOPRO 2025 落合陽一講演]]` を作成。
- 関連 page として `[[LLM Wiki/wiki/entities/落合陽一]]` `[[LLM Wiki/wiki/concepts/デジタルネイチャー]]` を追加。
- 抽出知見を保存するため `[[LLM Wiki/wiki/syntheses/2026-04-19 Synthesis - 生成AI時代に重要なのは書く力より読む力か]]` を追加。
- `[[LLM Wiki/wiki/concepts/アニミズム]]` `[[LLM Wiki/wiki/concepts/テクノアニミズム]]` に返しリンクを追加し、既存の存在論軸へ接続。
- `overview.md` と `index.md` を更新し、`デジタルネイチャー` `読む力 / 選ぶ力` `情報環境設計` を新たな焦点として反映。

## [2026-04-15] ingest | AI時代の生き方レポート

- `[[LLM Wiki/raw/clipping/AI時代の生き方レポート]]` を source として読解。
- source summary として `[[LLM Wiki/wiki/sources/2026-04-15 Source - AI時代の生き方レポート]]` を作成。
- 関連 page として `[[LLM Wiki/wiki/concepts/AI時代の自己]]` を追加。
- 抽出知見を保存するため `[[LLM Wiki/wiki/syntheses/2026-04-15 Synthesis - AI時代にどう生きるべきか]]` を追加。
- `overview.md` と `index.md` を更新し、AI時代の自己、身体性、一次情報、物語化の軸を全体像へ反映。
- 今回は個人の生き方整理に近い source のため、entity は新設せず、concept / synthesis 中心で ingest した。

## [2026-04-15] ingest | Naval Podcast AIと仕事の未来（raw 心のためのオートバイ）

- `[[LLM Wiki/raw/clipping/心のためのオートバイ]]` を source として読解。本文タイトルは「AIと仕事の未来について」で、Naval Ravikant と Nivi の対話録。
- source summary として `[[LLM Wiki/wiki/sources/2026-04-15 Source - Naval Podcast AIと仕事の未来（raw 心のためのオートバイ）]]` を作成。
- 関連 page として `[[LLM Wiki/wiki/entities/Naval Ravikant]]` `[[LLM Wiki/wiki/concepts/バイブコーディング]]` を追加。
- 抽出知見を保存するため `[[LLM Wiki/wiki/syntheses/2026-04-15 Synthesis - NavalのAI観と仕事観の要点]]` を追加。
- 既存 page への接続として `[[LLM Wiki/wiki/concepts/AI時代の自己]]` に source / synthesis を追記。
- `index.md` と `overview.md` を更新し、仕事観・主体性・学習法の論点を全体像へ反映。

## [2026-04-15] ingest | Thread by @shannholmberg（AutoReason for Marketing）

- `[[LLM Wiki/raw/clipping/Thread by @shannholmberg]]` を `raw` source として取り込み（元 `/俺のメモ/raw` から移動）。
- 旧 `raw` フォルダ（`/Users/momisantakuto/Library/Mobile Documents/iCloud~md~obsidian/Documents/俺のメモ/raw`）は空を確認して削除。
- source summary として `[[LLM Wiki/wiki/sources/2026-04-15 Source - Thread by @shannholmberg（AutoReason for Marketing）]]` を作成。
- 関連 page として `[[LLM Wiki/wiki/entities/shannholmberg]]` `[[LLM Wiki/wiki/concepts/AutoReason]]` を追加。
- 抽出知見を保存するため `[[LLM Wiki/wiki/syntheses/2026-04-15 Synthesis - AutoReasonをマーケ実務に落とすときの設計要点]]` を追加。
- 既存 page への接続として `[[LLM Wiki/wiki/concepts/AI支援型協働設計]]` を更新。
- `index.md` と `overview.md` を更新し、主観タスク向け反証設計（批評分離・盲検評価・知識層接続）の論点を反映。

## [2026-04-20] ingest | non-held markdown backlog

- これまで `保留` 以外として整理されていた raw markdown 群をまとめて ingest した。
- source summary として、以下を追加:
  - `[[LLM Wiki/wiki/sources/2026-04-20 Source - Thread by @SHL0MS（AutoReason）]]`
  - `[[LLM Wiki/wiki/sources/2026-04-20 Source - 日本の特性を活かしたホラーコンテンツ制作]]`
  - `[[LLM Wiki/wiki/sources/2026-04-20 Source - ホラーとデジタルネイチャー]]`
  - `[[LLM Wiki/wiki/sources/2026-04-20 Source - 日本文化と東洋的価値観のコンテンツ制作応用]]`
  - `[[LLM Wiki/wiki/sources/2026-04-20 Source - アートを学ぶ：多神教的な落合陽一と一神教的なチームラボ]]`
  - `[[LLM Wiki/wiki/sources/2026-04-20 Source - AI時代（from-vault）]]`
  - `[[LLM Wiki/wiki/sources/2026-04-20 Source - 表現したいもの]]`
  - `[[LLM Wiki/wiki/sources/2026-04-20 Source - やりたいこと]]`
  - `[[LLM Wiki/wiki/sources/2026-04-20 Source - 日本文化の包括的調査レポート]]`
  - `[[LLM Wiki/wiki/sources/2026-04-20 Source - 日本文化は宇宙社会を築く最大の天然資源か]]`
  - `[[LLM Wiki/wiki/sources/2026-04-20 Source - 超AI時代の生存戦略]]`
  - `[[LLM Wiki/wiki/sources/2026-04-20 Source - 人生の経営戦略]]`
  - `[[LLM Wiki/wiki/sources/2026-04-20 Source - デザイナー]]`
  - `[[LLM Wiki/wiki/sources/2026-04-20 Source - 好きを言語化する技術]]`
  - `[[LLM Wiki/wiki/sources/2026-04-20 Source - 創造とは]]`
  - `[[LLM Wiki/wiki/sources/2026-04-20 Source - AIと現代アート]]`
  - `[[LLM Wiki/wiki/sources/2026-04-20 Source - 作品アイデア]]`
  - `[[LLM Wiki/wiki/sources/2026-04-20 Source - シンギュラリティ後のAI]]`
- 関連 page として `[[LLM Wiki/wiki/concepts/Jホラー]]` `[[LLM Wiki/wiki/concepts/気配]]` `[[LLM Wiki/wiki/concepts/身体性]]` `[[LLM Wiki/wiki/concepts/多神教的世界観]]` `[[LLM Wiki/wiki/concepts/一神教的世界観]]` `[[LLM Wiki/wiki/entities/チームラボ]]` を追加。
- 抽出知見を保存するため `[[LLM Wiki/wiki/syntheses/2026-04-20 Synthesis - Jホラーの強みは何か]]` `[[LLM Wiki/wiki/syntheses/2026-04-20 Synthesis - 日本文化の感性はAI時代の制作にどう効くか]]` `[[LLM Wiki/wiki/syntheses/2026-04-20 Synthesis - AI時代に制作と仕事の重心はどう変わるか]]` を追加。
- `index.md` と `overview.md` を更新し、`Jホラー` `気配` `身体性` `多神教的 / 一神教的世界観` `文化の資源性` `仕事重心の再配置` を新たな全体論点として反映。

## [2026-05-28] ingest | remaining raw batch

- 正規化後に未 ingest だった raw source 27件を一括 ingest。
- `wiki/sources/` に 27件の source summary を追加。
- 空ファイル `2026-01-31.md` と `中東.md` は空 source として記録。
- 関連概念として `Agentic Engineering` `AI時代の創造性` `0次情報` `セレンディピティ` `メタバース` `現実科学` `運と成功` `意味経済` `作品価値` `歌詞制作` `物語設計` `自己運用` などを追加。
- 関連 entity として `Andrej Karpathy` `佐藤航陽` `つんく♂` を追加。
- 横断 synthesis として `AI時代の創造性と仕事の重心` `日本文化を天然資源として読む` `人生と創作の自己運用メモ束` を追加。
- `index.md` と `overview.md` を更新。

## [2026-05-30] lint | wiki health check

- `LLM Wiki/wiki/` の IDE lint を確認し、エラーなし。
- Obsidian wikilink のリンク切れ、孤立ページ、`index.md` 掲載漏れを確認。
- 初回チェックでリンク切れ 3 件を検出。
- `落合陽一` を concept ではなく `[[LLM Wiki/wiki/entities/落合陽一]]` に修正。
- `overview.md` の古い `clipping/日本の特性を活かしたホラーコンテンツ制作` リンクを、対応する source summary へ修正。
- 再チェック結果: `BROKEN 0` `ORPHANS 0` `MISSING_INDEX 0`。

## [2026-05-30] ingest | メタスキル

- `読書メモ/メタスキル.md` を `LLM Wiki/raw/from-vault/読書メモ/メタスキル.md` にコピーし、raw source として扱うようにした。
- `[[LLM Wiki/wiki/sources/2026-05-30 Source - メタスキル]]` を作成。
- 新規 concept として `[[LLM Wiki/wiki/concepts/メタスキル]]` を作成。
- 横断 synthesis として `[[LLM Wiki/wiki/syntheses/2026-05-30 Synthesis - メタスキルはAI時代の生存戦略になるか]]` を作成。
- 関連 concept `[[LLM Wiki/wiki/concepts/AI時代のキャリア戦略]]` `[[LLM Wiki/wiki/concepts/自己運用]]` `[[LLM Wiki/wiki/concepts/0次情報]]` `[[LLM Wiki/wiki/concepts/物語設計]]` を更新。
- `index.md` と `overview.md` を更新。
- open question: 自分の作業・知能・存在をどの単位でモジュール化すると、AI時代の価値循環につながるか。

## [2026-06-01] ingest | リミナルスペースはなぜ怖いのか

- `Clippings/【夢ナビ 民俗学講義】リミナルスペースはなぜ怖いのか――ロアと世界観の民俗学.md` を `LLM Wiki/raw/clipping/` にコピーし、raw source として扱うようにした。
- `[[LLM Wiki/wiki/sources/2026-06-01 Source - リミナルスペースはなぜ怖いのか]]` を作成。
- 新規 concept として `[[LLM Wiki/wiki/concepts/リミナルスペース]]` `[[LLM Wiki/wiki/concepts/ロア]]` `[[LLM Wiki/wiki/concepts/日常侵食]]` を作成。
- 横断 synthesis として `[[LLM Wiki/wiki/syntheses/2026-06-01 Synthesis - リミナルスペースはJホラーの怖さをどう作るか]]` を作成。
- 関連 concept `[[LLM Wiki/wiki/concepts/Jホラー]]` `[[LLM Wiki/wiki/concepts/気配]]` `[[LLM Wiki/wiki/concepts/物語設計]]` `[[LLM Wiki/wiki/concepts/アニミズム]]` を更新。
- `index.md` と `overview.md` を更新。
- open question: 個人の恐怖体験が共同体のロアになる過程を、AI / XR / ゲーム作品内でどう体験化できるか。

## [2026-06-01] maintenance | raw を clipping/ に統合

- `raw/` 直下に散在していた PDF 3件、X スレ 2件、`心のためのオートバイ.md` を `[[LLM Wiki/raw/clipping]]` へ移動。
- `from-vault/Clippings/` にあった民俗学講義も `clipping/` へ移動し、空ディレクトリを削除。
- 影響のあった `wiki/sources/` `wiki/concepts/` `wiki/syntheses/` `wiki/entities/` `log.md` の `source_path` と wikilink を一括更新（23ファイル）。
- `[[LLM Wiki/raw/README]]` と `[[LLM Wiki/raw/from-vault/README]]` に新ルールを反映。
- 再チェック結果: `BROKEN 0`、`raw/` 直下の stray files 0、`clipping/` 35件。

## [2026-06-18] ingest | JSAI2026 ビル格と不動産価値の再設計

- ユーザー指定の `jsai_A00560_20260327_131602_A(1).pdf`（参加費・発表費領収書）を `[[LLM Wiki/raw/clipping/jsai_A00560_20260327_131602_A.pdf]]` にコピー。
- 同テーマの `[[LLM Wiki/raw/clipping/人工知能学会とビル格プロジェクト.pdf]]`（学会参加レポート）と `[[LLM Wiki/raw/clipping/人工知能学会スライドv1_JSAI2026_ビル格.pptx]]`（発表スライド）も raw に追加し、内容 ingest の主 source とした。
- `[[LLM Wiki/wiki/sources/2026-06-18 Source - JSAI2026 ビル格と不動産価値の再設計]]` を作成。
- 新規 entity: `[[LLM Wiki/wiki/entities/冷泉荘]]` `[[LLM Wiki/wiki/entities/吉原勝己]]` `[[LLM Wiki/wiki/entities/人工知能学会]]`
- 新規 concept: `[[LLM Wiki/wiki/concepts/ビル格]]`
- 横断 synthesis: `[[LLM Wiki/wiki/syntheses/2026-06-18 Synthesis - ビル格はLLM研究か不動産価値の再設計か]]`
- 関連 concept `[[LLM Wiki/wiki/concepts/0次情報]]` `[[LLM Wiki/wiki/concepts/Agentic Engineering]]` `[[LLM Wiki/wiki/concepts/意味経済]]` を更新。
- `index.md` と `overview.md` を更新。
- open question: ビル格 AI の事業検証指標（入居・集客・メディア・他オーナー相談）をどう観察・記録するか。

## [2026-06-23] ingest | AI人材報酬と日本在住キャリア戦略

- `[[LLM Wiki/raw/clipping/AI人材・AI活用プロフェッショナルのグローバル報酬と採用調査レポート]]` を source として反映。
- source summary として `[[LLM Wiki/wiki/sources/2026-06-23 Source - AI人材報酬と日本在住キャリア戦略]]` を作成。
- 関連 concept `[[LLM Wiki/wiki/concepts/AI時代のキャリア戦略]]` を更新し、報酬市場、USDベンチマーク、地域調整、エクイティ交渉をキャリア戦略の論点として追加。
- `index.md` を更新。
- open question: 日本在住で、AIキャリアのグローバル報酬と自分の創作・事業オーナーシップをどう配分するか。

## [2026-06-24] ingest | 深津貴之 AIと戦うな上司になれ

- `Clippings/【あなたの努力は“24時間働くAI”に代替される】深津貴之「AIと戦うな“上司”になれ」...` を `[[LLM Wiki/raw/clipping/深津貴之 AIと戦うな上司になれ]]` にコピーし、raw source として扱うようにした。
- source summary として `[[LLM Wiki/wiki/sources/2026-06-24 Source - 深津貴之 AIと戦うな上司になれ]]` を作成。
- 新規 entity として `[[LLM Wiki/wiki/entities/深津貴之]]` `[[LLM Wiki/wiki/entities/Demis Hassabis]]` `[[LLM Wiki/wiki/entities/TBS CROSS DIG with Bloomberg]]` を作成。
- 横断 synthesis として `[[LLM Wiki/wiki/syntheses/2026-06-24 Synthesis - AIの上司になるとは何か]]` を作成。
- 関連 concept `[[LLM Wiki/wiki/concepts/メタスキル]]` `[[LLM Wiki/wiki/concepts/AI時代のキャリア戦略]]` `[[LLM Wiki/wiki/concepts/AI時代の自己]]` `[[LLM Wiki/wiki/concepts/自己運用]]` `[[LLM Wiki/wiki/concepts/0次情報]]` `[[LLM Wiki/wiki/concepts/意味経済]]` `[[LLM Wiki/wiki/concepts/Agentic Engineering]]` を更新。
- `overview.md` と `index.md` を更新。
- open question: 自分の制作・事業において、AIに注入すべき欲望、ポリシー、初期条件、0次情報は何か。

## [2026-06-25] ingest | Clippings 未処理19件一括

- `Clippings/` に残っていた19件を `[[LLM Wiki/raw/clipping/]]` にコピーし、source summary 19件を作成。
- 新規 entity: `[[LLM Wiki/wiki/entities/原研哉]]` `[[LLM Wiki/wiki/entities/千葉雅也]]` `[[LLM Wiki/wiki/entities/中島聡]]` `[[LLM Wiki/wiki/entities/久保田晃弘]]` `[[LLM Wiki/wiki/entities/西野亮廣]]` `[[LLM Wiki/wiki/entities/Jensen Huang]]` `[[LLM Wiki/wiki/entities/外山滋比古]]`
- 横断 synthesis: `[[LLM Wiki/wiki/syntheses/2026-06-25 Synthesis - AI時代のクリエイター防御と産業再配置]]`
- 関連 entity `[[LLM Wiki/wiki/entities/深津貴之]]` `[[LLM Wiki/wiki/entities/佐藤航陽]]`、concept `[[LLM Wiki/wiki/concepts/作品価値]]` を更新。
- `index.md` を更新。
- ingest 対象: Sequoia AGI Keynote、久保田AI特論、原研哉×深津、千葉雅也、中島聡、コムドット×西野、佐藤航陽宇宙会議、深津受託化＋X3本、AI映画呼称、LLM Wiki Explained、Jensen Huang、Kenn Ejima、Migaku給与、佐藤YouTube後編、思考の整理学、キャッシュフロークワドラント。
- open question: ホラーIPを「入口＋再現困難性＋0次情報」で防御線として設計するとき、最初の1本は何を接続するか。

## [2026-06-25] lint | post-batch ingest health check

- `Clippings/` 未 ingest 19件 → 0件（全件 `raw/clipping/` + `wiki/sources/` 反映済み）。
- ファイル名に `"` を含む source は短い raw 別名（`深津X …` `Jensen Huang AI採用基準.md` `Kenn Ejima Codex Plan workflow.md`）を追加し `source_path` を修正。
- `Creativity in the Age of AI…` の YAML 引用符も修正。
- 再チェック: `NOT_INGESTED_COUNT 0`（JSAI 領収書 PDF・pptx は主 source の補助ファイルとして除外）、`MISSING_INDEX 0`。

## [2026-06-25] ingest | AI時代の創造性関連再整理

- `Creativity in the Age of AI` 系の d.school 連作と関連演習を読み直し、`[[LLM Wiki/wiki/sources/2026-05-28 Source - AIをEasy Buttonにしない]]` `[[LLM Wiki/wiki/sources/2026-05-28 Source - AIでデザインスキルはより重要になる]]` `[[LLM Wiki/wiki/sources/2026-05-28 Source - AIとともに進化する創造性]]` `[[LLM Wiki/wiki/sources/2026-05-28 Source - Articles of Serendipity]]` を詳細化。
- 近接 source として `[[LLM Wiki/wiki/sources/2026-05-28 Source - AI時代のクリエイティブワークフロー]]` `[[LLM Wiki/wiki/sources/2026-05-28 Source - AI時代に生き残る5つのこと]]` も更新し、創造性・仕事・キャリアの接続を補強。
- 新規 entity として `[[LLM Wiki/wiki/entities/Stanford d.school]]` を作成。
- 中心 concept `[[LLM Wiki/wiki/concepts/AI時代の創造性]]` を更新し、easy button 批判、摩擦、好奇心、実験、AIとのループ、自動化の配分、媒体文法、身体性、0次情報の論点を統合。
- 関連 concept `[[LLM Wiki/wiki/concepts/好奇心]]` `[[LLM Wiki/wiki/concepts/セレンディピティ]]` を更新。
- 横断 synthesis `[[LLM Wiki/wiki/syntheses/2026-05-28 Synthesis - AI時代の創造性と仕事の重心]]` を更新し、生成から意図・有用な差異・選択・関係性・身体性へ重心が移る構造として整理。
- `overview.md` と `index.md` を更新。
- health check: IDE lints 0件、wiki wikilink `BROKEN 0`。
- open question: 自分の制作工程で、AIに任せる部分と、あえて摩擦・身体性・0次情報を残す部分をどう切り分けるか。

## [2026-06-29] ingest | 多摩美AI特論 逆行する美学 未処理clipping

- `Clippings/AI特論 第1回「逆行する美学」...〈前半〉... 1.md` と `Clippings/AI特論 第1回「逆行する美学」...〈後半〉...md` を `[[LLM Wiki/raw/clipping/]]` にコピーし、raw source として扱うようにした。
- source summary として `[[LLM Wiki/wiki/sources/2026-06-29 Source - 逆行する美学 前半解説 久保田晃弘]]` `[[LLM Wiki/wiki/sources/2026-06-29 Source - 逆行する美学 後半 久保田晃弘]]` を作成。
- 新規 concept として `[[LLM Wiki/wiki/concepts/人工物の美学]]` を作成。
- 関連 entity `[[LLM Wiki/wiki/entities/久保田晃弘]]`、concept `[[LLM Wiki/wiki/concepts/AI時代の創造性]]` `[[LLM Wiki/wiki/concepts/作品価値]]` `[[LLM Wiki/wiki/concepts/身体性]]` `[[LLM Wiki/wiki/concepts/テクノアニミズム]]` `[[LLM Wiki/wiki/concepts/意味経済]]` を更新。
- 横断 synthesis `[[LLM Wiki/wiki/syntheses/2026-05-28 Synthesis - AI時代の創造性と仕事の重心]]`、`overview.md`、`index.md` を更新。
- open question: AI生成物の生成過程、使用モデル、編集履歴、倫理的背景を、作品の価値や怖さの一部としてどう扱うか。

## [2026-07-01] ingest | 思考の整理学要約 再ingest

- 既存 raw `[[LLM Wiki/raw/clipping/「思考の整理学」の長い長い要約｜sinsin_m]]` を読み直し、source summary `[[LLM Wiki/wiki/sources/2026-06-25 Source - 思考の整理学要約]]` を詳細化。
- 新規 concept として `[[LLM Wiki/wiki/concepts/知的発酵]]` `[[LLM Wiki/wiki/concepts/忘却]]` を作成。
- 横断 synthesis `[[LLM Wiki/wiki/syntheses/2026-07-01 Synthesis - 思考の整理は創造性をどう作るか]]` を作成し、入力を寝かせ、忘れ、混ぜ、身体に通し、編集する創造構造として整理。
- 関連 entity `[[LLM Wiki/wiki/entities/外山滋比古]]`、concept `[[LLM Wiki/wiki/concepts/セレンディピティ]]` `[[LLM Wiki/wiki/concepts/メタスキル]]` `[[LLM Wiki/wiki/concepts/自己運用]]` `[[LLM Wiki/wiki/concepts/身体性]]` `[[LLM Wiki/wiki/concepts/AI時代の創造性]]` を更新。
- `index.md` と `overview.md` を更新。
- open question: AIに即答させる領域と、人間側が忘却・身体・時間差を使う領域をどう切り分けるか。

## [2026-07-01] ingest | 情報のメタ化

- `LLM Wiki/raw/inbox/情報のメタ化.md` を raw source として追加（Claude との対話メモ、一次→二次→三次情報の抽象化論）。
- source summary として `[[LLM Wiki/wiki/sources/2026-07-01 Source - 情報のメタ化]]` を作成。
- 新規 concept `[[LLM Wiki/wiki/concepts/抽象化の梯子]]` を作成（メタ化・一次二次三次情報の横断ノード）。
- 横断 synthesis `[[LLM Wiki/wiki/syntheses/2026-07-01 Synthesis - 抽象化はいつ価値になるのか]]` を作成。抽出（固有名詞なしの法則: 価値 ≒ 素材の入手困難度 × 処理の昇華度）と検証（`0次情報` で反例→法則を narrowing→`AI時代のクリエイター防御と産業再配置` で予測チェック）まで実施。
- 関連 concept `[[LLM Wiki/wiki/concepts/0次情報]]` `[[LLM Wiki/wiki/concepts/メタスキル]]`、entity `[[LLM Wiki/wiki/entities/外山滋比古]]` に相互リンクを追加。
- `index.md` に source / concept / synthesis を追記。
- open question: 「一次情報」と「0次情報」の階層統合、既存 synthesis の三次情報到達率の点検。

## [2026-07-01] ingest | メタスキル 再ingest

- 既存 raw `[[LLM Wiki/raw/from-vault/読書メモ/メタスキル]]` を読み直し、source summary `[[LLM Wiki/wiki/sources/2026-05-30 Source - メタスキル]]` を詳細化。
- 新規 concept として `[[LLM Wiki/wiki/concepts/自分のモジュール化]]` `[[LLM Wiki/wiki/concepts/デジタル・アルチザン]]` を作成。
- 横断 synthesis `[[LLM Wiki/wiki/syntheses/2026-05-30 Synthesis - メタスキルはAI時代の生存戦略になるか]]` を更新し、`構造把握 × ゲーム変更 × モジュール化 × 非対称情報 × ナラティブ × 資本循環` の価値循環として再抽象化。
- 関連 concept `[[LLM Wiki/wiki/concepts/メタスキル]]` `[[LLM Wiki/wiki/concepts/AI時代のキャリア戦略]]` `[[LLM Wiki/wiki/concepts/自己運用]]` `[[LLM Wiki/wiki/concepts/0次情報]]` `[[LLM Wiki/wiki/concepts/物語設計]]` `[[LLM Wiki/wiki/concepts/意味経済]]` `[[LLM Wiki/wiki/concepts/Agentic Engineering]]` `[[LLM Wiki/wiki/concepts/AI時代の自己]]` を更新。
- `index.md` と `overview.md` を更新。
- open question: 自分の作業・知能・存在をどの粒度でモジュール化し、どの偏愛を少人数の意味として残すか。

## [2026-07-02] ingest | 深津貴之 clipping 未処理3件

- `Clippings/もっとも大事なこと （noteのはじめかた）...`、`Clippings/本文のポイント （noteのはじめかた）...`、`Clippings/経営者にデザインや技術の大切さをわかってもらうには？...` を `[[LLM Wiki/raw/clipping]]` に短い raw 名でコピー。
- source summary として `[[LLM Wiki/wiki/sources/2026-07-02 Source - noteのはじめかた もっとも大事なこと]]` `[[LLM Wiki/wiki/sources/2026-07-02 Source - noteのはじめかた 本文のポイント]]` `[[LLM Wiki/wiki/sources/2026-07-02 Source - 経営者にデザインや技術をわかってもらうには]]` を作成。
- 新規 concept として `[[LLM Wiki/wiki/concepts/継続的発表]]` `[[LLM Wiki/wiki/concepts/環境選択]]` を作成。
- 横断 synthesis `[[LLM Wiki/wiki/syntheses/2026-07-02 Synthesis - 続ける創作と通じる環境を選ぶ]]` を作成し、`継続可能性 = 低い発表摩擦 × 内発的興味 × 読者に通じる構造 × 価値観が合う環境` として抽出・検証。
- 関連 entity `[[LLM Wiki/wiki/entities/深津貴之]]`、concept `[[LLM Wiki/wiki/concepts/言語化]]` `[[LLM Wiki/wiki/concepts/物語設計]]` `[[LLM Wiki/wiki/concepts/自己運用]]` `[[LLM Wiki/wiki/concepts/AI時代の創造性]]` `[[LLM Wiki/wiki/concepts/AI時代のキャリア戦略]]` `[[LLM Wiki/wiki/concepts/メタスキル]]` `[[LLM Wiki/wiki/concepts/Agentic Engineering]]` を更新。
- `index.md` と `overview.md` を更新。
- open question: ホラー世界観づくりを、完成大作ではなく継続発表できる最小単位へどう分割するか。
