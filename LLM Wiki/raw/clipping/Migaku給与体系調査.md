---
title: "Migaku給与体系調査"
source: "https://chatgpt.com/c/6a3a2b3f-f128-83e8-baf9-4fb7f0c43255"
author:
published:
created: 2026-06-23
description: "ChatGPT conversation with 6 messages"
tags:
  - "clippings"
---
**ChatGPT said**

Migakuを起点に、公開求人・採用ページで「日本在住/日本法人あり」「USDまたは米国/グローバル水準の報酬」「リモート採用」の証拠が取れる会社を中心に洗います。給与体系は非公開な会社も多いので、確度を分けて整理します。

2026年6月23日時点の公開情報ベースだと、 **Migakuにかなり近い会社は少数** です。理由は、日本法人の正社員給与は実務上JPY払いになりやすく、公開求人でも「USD基準・米国水準」と明言する会社が少ないためです。日本の賃金支払いには労基法24条の「通貨・直接・全額・毎月1回以上・一定期日」の原則があり、リモート雇用実務でも日本の正社員給与はJPYで払うのが一般的です。 [^1]  
なので、ここでは **「USDで表示/米国・グローバル基準で設計」** と **「実際にUSDで振込」** を分けて見ています。

## 結論：Migakuに近い候補

| 会社 | 日本拠点/法人 | 報酬の公開情報 | Migaku類似度 |
| --- | --- | --- | --- |
| **Migaku** | 東京HQあり | iOS求人で **67k〜135k USD / 1,000万〜2,000万円** 、世界リモート可。別求人でも$60k〜$100k、Product Designerで$70k〜$90kの履歴あり。 [^2] | 基準点 |
| **Alpaca** | **AlpacaJapan株式会社** あり。日本で第一種金融商品取引業者登録もあり。 [^3] | Japan向けSenior SEで **1,400万〜2,100万円** 、別媒体でJapan/Remoteポジションが **$106k〜$114k推定** 。公式求人にもUSD建ての在宅手当・月次手当あり。 [^4] | **A：最有力** |
| **GitLab** | **GitLab GK** の東京住所・日本向け福利厚生ページあり。全社リモート。 [^5] | 報酬設計はSan Franciscoベンチマークを起点にロケーション係数などで調整する方式を公開。東京の投稿給与データは職種により約1,500万〜3,100万円級の例あり。 [^6] | **A-/B+：米国基準だが地域調整あり** |
| **Applied Intuition** | 米国発スタートアップ。東京拠点・日本市場進出情報あり。 [^7] | JapanDev掲載で日本ポジション **1,100万〜1,500万円** 、一部SWEで **800万〜1,300万円** 。米国側求人では$100k〜$200k級の例あり。 [^8] | **B：US企業の日本高給枠** |
| **Stripe** | 東京オフィスあり。 [^9] | JapanDevで **900万〜2,000万円** レンジ。OpenSalaryでは日本Stripeの投稿中央値が約3,780万円だが、投稿データなので参考値。 [^9] | **B：外資US水準、ただしUSD払いとは限らない** |
| **Noeon Research** | 東京HQのAIスタートアップ | Japan在住者向けでML Engineer **1,800万〜2,100万円** 、Backend/Frontend **1,400万〜1,700万円** 。英語環境・日本語不要の求人。 [^10] | **B/C：給与帯は近いがUS/ドル基準ではない** |
| **Automattic** | 日本法人は未確認 | 「勤務地に関係なくグローバルレンジと内部公平性を重視」と説明。一方で可能な限り現地通貨払い。 [^11] | **C：報酬思想は近いが日本支社条件に弱い** |
| **DataAnnotation** | 日本法人は未確認 | 日本向けリモート案件で、PayPal経由USD払いの記載あり。ただし基本は業務委託/タスク型。 [^12] | **C：USD払い寄りだが正社員/支社条件に弱い** |

## 実際に狙うなら優先順位

**最優先で見るべきは Alpaca と GitLab** です。Alpacaは「日本法人/日本登録あり」「Japan向け高レンジ求人」「USD表記の周辺手当」が揃っていて、Migakuに最も近いです。GitLabは「日本法人＋全社リモート＋San Franciscoベンチマーク起点の報酬設計」が明確ですが、完全な米国同額ではなく地域調整型です。

**次点は Applied Intuition と Stripe** です。どちらも米国企業の日本拠点で、給与レンジは日本市場の上位です。ただし、公開情報上は「USD建てで給与を払う」とまでは確認できず、JPY給与＋株式/RSUで米国テック水準に近づくタイプと見るのが安全です。

**Migaku型の見分け方** は、求人に次の表現があるかです。

- `USD salary range` / `$100k+`
- `Remote - Japan` / `Remote - APAC`
- `Japan residents only` かつ `No Japanese required`
- `US benchmark` / `global compensation`
- `stock options` / `equity`
- `Tokyo Office (Remote)` / `Japan entity`

面接やリクルーターには、次をそのまま聞くのがよいです。

> Base salaryはUSD建てですか、それともJPY建てですか？JPY建ての場合、USDレンジにペッグされていますか？Employer of Recordは日本法人ですか、海外法人との契約ですか？社会保険込みの正社員雇用ですか、業務委託ですか？Equity/RSUは米国本社と同じバンドですか？

日本の一般的なソフトウェアエンジニア給与中央値は、TokyoDevで約569万円、Levels.fyiの日本SWE中央値で約862万円なので、 **Migakuの1,000万〜2,000万円、Alpacaの1,400万〜2,100万円、Noeonの1,800万〜2,100万円は明確に上位帯** です。 [^13]

継続的に探すなら、JapanDev / TokyoDev / Web3.career / Greenhouse / Ashbyで「Japan + Remote + USD + 14M JPY+」条件を週次監視すると見つかりやすいです。

---

**You said**

Migakuはなんでそんな高いの？？

---

**ChatGPT said**

Migakuの給与が高い理由は、単に「気前がいい」よりも、会社の市場・採用競争・少人数体制が噛み合っている可能性が高いです。公開求人とプロダクト情報を確認して、推測と確認済み情報を分けて説明します。

一言でいうと、 **Migakuは「日本企業の給与」ではなく、グローバルSaaSスタートアップの採用競争で値付けしているから** だと思います。

特に大きい理由はこのあたりです。

### 1\. 日本国内採用ではなく、世界中から採っている

MigakuのiOS求人は「Remote OK - Worldwide」「Apply from Anywhere」で、日本語不要・英語Fluent・Senior以上という条件です。給与も **67k〜135k USD、1,000万〜2,000万円** とUSD併記されています。つまり、日本の相場に合わせるより、 **欧州・アジア・米国寄りのリモート人材市場で戦っている** 。 [^14]

日本で見ると高いですが、米国のSenior iOS Developer相場で見ると、$135kはむしろ普通〜やや控えめです。ZipRecruiterでは2026年6月時点の米国Senior iOS Developer平均が約$137k、IndeedでもiOS Developer平均が約$137kです。 [^15]

### 2\. 求めている人材がかなり狭い

MigakuのiOS求人は、単なるSwift実装者ではなく、Kotlin Multiplatform APIとの統合、App Storeリリース、ユーザー対応、ピクセルパーフェクトなUI、流体的なアニメーション、Apple Pay、OCR、リモート国際チーム対応、さらに「外国語学習への深い関心」まで求めています。 [^14]

これはかなりニッチです。  
**iOSが強い + 英語で働ける + KMP/OCR/課金まわりが分かる + 語学学習プロダクトに本気で興味がある** みたいな人は、そもそも候補者数が少ない。少ない人材を取りに行くなら、給与を上げるしかありません。

### 3\. 少人数なので、1人の影響が大きい

JapanDev上ではMigakuは東京拠点・11〜50人規模とされています。iOS求人にも「あなたの仕事が会社の成功に大きく直接影響する」と書かれています。 [^14]

大企業の1人エンジニアは何百分の1ですが、Migaku規模だと **モバイル担当1人の出来が、売上・継続率・アプリ評価に直結** します。だから、年収1,000万〜2,000万円を払っても、良い人を採るほうが安いという判断になりやすいです。

### 4\. かなり成長フェーズっぽい

LinkedInに載っていたBusiness Operations Manager求人では、Migaku自身が「過去1年で売上が10倍になり、今後12か月でも同じことを目指す」と説明しています。これは監査済み財務ではなく求人文ベースですが、少なくとも会社側は **高成長フェーズとして採用している** ことが分かります。 [^16]

高成長スタートアップでは、「安く採ってゆっくり育てる」より、 **高くても即戦力を入れて開発速度を買う** ほうが合理的です。

### 5\. プロダクトが“英会話教室”ではなく、SaaS/AI/コンテンツ統合ツール

MigakuはNetflix、YouTube、Webコンテンツを学習教材化するブラウザ拡張・モバイルアプリ・フラッシュカード・AI解説を持つプラットフォームです。複数言語対応、Chrome拡張、iOS/Android、SRS、字幕解析、辞書、AI説明などが絡みます。 [^17]

つまり労働集約型の語学学校ではなく、 **ソフトウェアの限界費用が低いサブスク事業** です。ユーザーが増えても先生を同じ割合で増やす必要がないので、エンジニアに厚く投資しやすい構造です。

### 6\. 会社の思想として「速く出す」ことを重視している

採用ページでは、Migakuは「Product Market Fitに到達するまでは、成長のために技術的負債も戦略的に許容する」「速く出荷することがスタートアップの主目的」と説明しています。 [^17]

これはかなりハードな環境のサインでもあります。高給なのは、単に福利厚生が良いというより、 **スピード・自走・曖昧さ・負荷への対価** も入っていると思います。

## なので、実態はこう

Migakuの給与が高い理由は、

**日本相場ではなくグローバル相場で採っている**  
＋  
**少人数・高成長・即戦力採用**  
＋  
**ニッチな技術/プロダクト適性を求めている**  
＋  
**普通の日本企業よりハードなスタートアップ期待値がある**

という組み合わせです。

ただし注意点として、求人上の **$135k / 2,000万円** はレンジ上限で、全員がそこになるわけではありません。求人にも「希望給与を書いて」とあり、ストックオプションも「outstanding candidates」と条件付きです。 [^14]

肌感でいうと、Migakuの給与は「日本の会社なのに異常に高い」というより、 **日本に拠点があるグローバル・リモートSaaSが、米国より少し安めの価格で優秀な人を取りに来ている** と見るのが一番近いです。

---

**You said**

グローバル基準で、AI人材とかAI使える人とかで、深くサーベイして

---

**ChatGPT said**

Called tool

<iframe title="internal://deep-research" src="https://connector_openai_deep_research.web-sandbox.oaiusercontent.com/?app=chatgpt&amp;darkModeType=increased&amp;locale=en-US&amp;deviceType=desktop" allow="camera *; clipboard-read *; clipboard-write *; fullscreen *; local-network-access *; microphone *; midi *; web-share *" allowfullscreen=""></iframe>

[^1]: [japaneselawtranslation.go.jp](https://www.japaneselawtranslation.go.jp/en/laws/view/3567/en?utm_source=chatgpt.com)

[^2]: [japan-dev.com](https://japan-dev.com/jobs/migaku/migaku-experienced-remote-ios-developer-fqq8ky?utm_source=chatgpt.com)

[^3]: [alpaca.markets](https://alpaca.markets/jp/about)

[^4]: [tokyodev.com](https://www.tokyodev.com/companies/alpaca/jobs/senior-software-engineer?utm_source=chatgpt.com)

[^5]: [about.gitlab.com](https://about.gitlab.com/company/visiting/?utm_source=chatgpt.com)

[^6]: [about.gitlab.com](https://about.gitlab.com/blog/gitlabs-global-compensation-calculator-the-next-iteration/?utm_source=chatgpt.com)

[^7]: [wellfound.com](https://wellfound.com/jobs/3604966-embedded-software-engineer-vehicle-os?utm_source=chatgpt.com)

[^8]: [japan-dev.com](https://japan-dev.com/companies/applied-intuition?utm_source=chatgpt.com)

[^9]: [japan-dev.com](https://japan-dev.com/companies/tags/usa-offices?utm_source=chatgpt.com)

[^10]: [tokyodev.com](https://www.tokyodev.com/companies/noeon-research/jobs/senior-ml-engineer-llmops?utm_source=chatgpt.com)

[^11]: [automattic.com](https://automattic.com/compensation/?utm_source=chatgpt.com)

[^12]: [jp.indeed.com](https://jp.indeed.com/q-%E3%83%AA%E3%83%A2%E3%83%BC%E3%83%88%E3%83%AF%E3%83%BC%E3%82%AF-%E6%97%A5%E6%9C%AC%E8%AA%9E-%E3%83%89%E3%83%AB-%E6%B1%82%E4%BA%BA.html?utm_source=chatgpt.com)

[^13]: [tokyodev.com](https://www.tokyodev.com/articles/software-developer-salaries-in-japan?utm_source=chatgpt.com)

[^14]: [japan-dev.com](https://japan-dev.com/jobs/migaku/migaku-experienced-remote-ios-developer-fqq8ky)

[^15]: [ziprecruiter.com](https://www.ziprecruiter.com/Salaries/Senior-Ios-Developer-Salary?utm_source=chatgpt.com)

[^16]: [jp.linkedin.com](https://jp.linkedin.com/jobs/view/business-operations-manager-at-migaku-4334057219)

[^17]: [migaku.com](https://migaku.com/careers)