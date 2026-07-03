---
name: llm-wiki-ingest
description: Ingest raw sources, reading notes (読書メモ), clippings, PDFs, and Obsidian notes into this vault's LLM Wiki (LLM Wiki/raw -> LLM Wiki/wiki), and turn them into concept/entity/synthesis pages using a disciplined 一次→二次→三次 abstraction method (収集→分類→関連→抽出→検証). Use this whenever the user asks to ingest something, process raw/, learn a book or 読書メモ, update the LLM Wiki, create or update a source summary, write or upgrade a synthesis page, "抽象化して" / "三次情報にして" / "法則を抜き出して" / "統合して" / "概念化して", lint the wiki, update wiki/index.md or wiki/log.md, or otherwise maintain LLM Wiki pages. Also use it proactively whenever the user drops a link, clipping, or note and says something loose like "これ読んどいて" / "まとめといて" / "rawに入れた" if it's clearly destined for this wiki.
---

# LLM Wiki Ingest

## Scope

Use this skill only for this Obsidian vault's `LLM Wiki/`. Nothing outside `LLM Wiki/` unless the user explicitly names another vault note as a source to copy in.

The operating rules — directory meaning, page conventions, naming, and the abstraction method — live in:

- `LLM Wiki/AGENTS.md`

Always read `LLM Wiki/AGENTS.md` before doing ingest, lint, or maintenance. It is the single source of truth; do not duplicate its detail from memory, re-read it each session since it evolves.

## Core Rule

Treat `LLM Wiki/raw/` as immutable source material.

- Do not edit raw source files.
- If the user points to a normal vault note such as `読書メモ/メタスキル.md`, copy it into `LLM Wiki/raw/from-vault/読書メモ/` first.
- Then ingest the copy, not the original note.

## Standard Ingest Workflow

When the user says `ingest`, `インジェスト`, `rawに入れた`, `読書メモを学習`, or similar:

1. Read `LLM Wiki/AGENTS.md`.
2. Identify the source: if already under `LLM Wiki/raw/`, use it directly; otherwise copy it into the matching `LLM Wiki/raw/from-vault/` subfolder first.
3. Read the source (and any attached images).
4. Create or update a source summary in `LLM Wiki/wiki/sources/`.
5. Create or update related pages in `LLM Wiki/wiki/concepts/`, `LLM Wiki/wiki/entities/`, `LLM Wiki/wiki/syntheses/` — prefer updating an existing page over creating a near-duplicate.
6. Add wikilinks between related topic pages.
7. Update `LLM Wiki/wiki/index.md` and, if the big picture shifted, `LLM Wiki/wiki/overview.md`.
8. Append an entry to `LLM Wiki/wiki/log.md`.
9. Run lint / health checks on edited files.

Full step-by-step detail (directory meanings, page section conventions, naming rules) is in `AGENTS.md` — this list is just the checklist to keep in view while working.

## Why this skill exists beyond plain summarizing

A source summary and a concept page are still close to the raw material — useful, but they're organizing (二次情報), not yet distilling (三次情報). The actual value of this wiki compounds when a synthesis page reaches a law or structure that would survive even if every proper noun in it were swapped out. A synthesis that just lists "person A said X, person B said Y" is a well-organized restatement, not yet an abstraction — it's fine as a stepping stone, but don't stop there when the source material supports more.

## Abstraction Method (収集 → 分類 → 関連 → 抽出 → 検証)

This is the same method documented in full in `AGENTS.md` under "抽象化ワークフロー" — read that section for the complete version. The compressed form to keep in mind while writing pages:

1. **収集**: gather the source(s) plus whatever related sources/concepts already exist (check `wiki/index.md` first — don't re-derive what's already there).
2. **分類**: group raw elements that belong together and name the group. This naming *is* the concept/entity page title. Reuse an existing concept if it already fits; only mint a new one when nothing existing covers it.
3. **関連**: state the relationship between groups explicitly — causal (A causes B), contrastive (A and B pull opposite ways), sequential (A → B → C), or correlational — instead of listing groups side by side.
4. **抽出**: try to restate the core finding with every proper noun removed (no person names, company names, work titles, source titles). If it still holds together, that's a portable, three-tier finding. Three techniques help get there:
   - **上位概念化** (naming up): replace a specific instance with a broader term.
   - **変数モデル化** (modeling): replace proper nouns with variables and keep only the relationship (e.g. "revenue = unit price × turnover rate" shaped statements).
   - **アナロジー** (borrowing a form): map the situation onto an already-understood pattern from another domain.
   If removing the proper nouns leaves nothing — the sentence collapses or loses its meaning — the page is still at the organizing (二次) level. Say so plainly rather than forcing a law that isn't there.
5. **検証**: stress-test whatever law/structure step 4 produced, either by hunting for a counterexample elsewhere in the wiki, or by predicting what it implies for a situation not yet in the sources and checking whether that prediction is supported. Write the result into `## 含意` or `## open question`. If you find a counterexample, narrow the claim rather than hiding it — same honesty principle as elsewhere in `AGENTS.md`.

### Worked example (before / after)

Raw material: three separate sources where three different people each argue creators need to defend something against AI commoditization (one talks about reproduction-difficulty and merchandising, one about aesthetic friction/imperfection, one about domain expertise + AI).

- **二次情報 stop (organizing only)**: "深津は再現困難性とIP設計を挙げ、久保田・千葉は不完全さや摩擦を挙げ、Jensen Huangは専門性×AIを挙げた。" — accurate, but it's just three people's opinions lined up.
- **三次情報 (abstracted)**: strip the names — what's left is "commoditization pressure pushes value toward whatever an average model output can't cheaply reproduce: friction the model didn't choose to keep, context the model wasn't given, or a distribution channel the model can't occupy." That sentence survives without Fukatsu, Kubota, or Huang in it — it's a portable claim about how value relocates under commoditization, which is why it's worth a `## 含意` about where *this vault's own projects* should put their friction.
- **検証**: does any source in the wiki contradict "value moves to whatever isn't cheaply reproducible"? If a source shows commoditized output still capturing value on brand/distribution alone, that's a counterexample worth noting rather than smoothing over.

This is the bar to aim for when writing or upgrading a `wiki/syntheses/` page — not every page will fully clear it, and that's fine to say directly, but always attempt step 4 before settling for a list of who-said-what.

## Wiki Lint Workflow

When asked to lint:

1. Check IDE lint diagnostics.
2. Check broken wikilinks.
3. Check orphan pages.
4. Check pages missing from `wiki/index.md`.
5. Check raw files not represented by `wiki/sources/*` `source_path`.
6. Fix obvious issues.
7. Append the lint result to `wiki/log.md`.

Expected clean result:

```text
BROKEN 0
ORPHANS 0
MISSING_INDEX 0
NOT_INGESTED_COUNT 0
```

## User Shortcut Examples

The user can say things like:

- `これ ingest して`
- `読書メモをrawにして学習して`
- `raw全部処理して`
- `lintして`
- `未ingestを調べて`
- `このsynthesisをもっと抽象化して` / `三次情報まで持ち上げて`
- `固有名詞抜きで法則にして`
- `これと前のsourceを統合して`

Apply this skill for those requests.
