# MangaX — FOMUS Creative Studio LP

## プロジェクト概要
漫画制作サービス「FOMUS Creative Studio」のランディングページ。
プラットフォーム名は「MangaX」（mangax.fomusglobal.com）。

## ファイル構成
```
mangax-site/
├── index.html        # メインLP（全セクション）
├── options.html      # オプション料金一覧ページ
└── CLAUDE.md         # このファイル
```

## デザインシステム
### カラーパレット
- `--void: #04040a`        背景（最深）
- `--deep: #08081a`        背景（深）
- `--panel: #0d0d20`       カードパネル
- `--magenta: #e8006a`     メインアクセント
- `--cyan: #00d4ff`        セカンダリアクセント
- `--gold: #f5c842`        テーシャリアクセント
- `--white: #f0eef8`       テキスト

### フォント
- `Bebas Neue` — 見出し・数字（display）
- `Noto Sans JP` — 本文（body）
- `Noto Serif JP` — イタリック強調（serif）
- `Space Mono` — ラベル・キャプション（mono）

### アニメーション
- `.rv` — スクロールリビール（下から）
- `.rl` — 左から
- `.rr` — 右から
- IntersectionObserver で `.on` クラスを付与

## セクション構成（index.html）
1. **NAV** — ロゴ + ナビリンク + CTAボタン
2. **HERO** — メインビジュアル + コピー + スタッツ
3. **MARQUEE** — 流れるテキスト帯
4. **COMPARE** — 従来制作 vs FOMUS比較テーブル
5. **WHY** — 4つの数字カード（横4列シネマティック）
6. **USE CASES** — 4用途カード（シネマティック画像付き）
7. **PLATFORM** — MangaX プラットフォーム紹介
8. **PRICING** — 3プラン料金表
9. **SUBSIDY** — 補助金セクション（カウントダウン付き）
10. **PROCESS** — 5ステップ制作フロー
11. **CREATOR** — まっすー紹介
12. **FAQ** — アコーディオンFAQ（6問）
13. **COUNTDOWN** — 締切カウントダウンバナー
14. **CTA** — 最終クロージング
15. **FOOTER** — リンク + コピーライト

## 料金体系
### 個人向け（Story Starter）
- 10P: ¥98,000

### 法人向け（4/30申込特別価格）
- Business Standard: ¥148,000（通常¥198,000）
- Brand Package: ¥298,000（大企業向け）

### 補助金
- 小規模事業者持続化補助金（第19回）
- 申請締切: 2026年4月30日 17:00
- 補助率2/3、上限250万円
- 実質負担: Business Standard → 約¥49,000

## よく使うリンク
- 資料請求フォーム: `#contact`（フォームURLに差し替え予定）
- オプション: `options.html`
- MangaX: `https://mangax.fomusglobal.com`

## 今後の作業メモ
- [x] まっすーの写真を `massu.jpg` として追加 → `<img>` に差し替え済み
- [ ] 資料請求フォームURLを設定（index.html / options.html の `<!-- TODO: 資料請求フォームのURLに差し替え -->` を検索）
- [ ] Use Casesの画像を実際の漫画サンプルに差し替え（現在はbase64プレースホルダー）
- [x] OGP / meta タグの追加
- [ ] Google Analytics / GTMの追加（GA測定ID `G-XXXXXXXXXX` が必要）
- [x] SEO構造化データ（WebPage, Organization, Service, FAQPage, BreadcrumbList）
- [x] options.htmlをindex.htmlのデザインに統一
- [x] favicon.svg追加
- [x] robots.txt / sitemap.xml追加
- [x] キーワード最適化（7ターゲットキーワード）
- [ ] OG画像（`og-image.jpg` 1200×630px）を作成し、og:image / twitter:image のコメントを解除
