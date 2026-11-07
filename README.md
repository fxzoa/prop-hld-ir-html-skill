# prop-hld-ir-html-skill

`prop-hld-ir-html` スキルを別 PC やチーム環境に `npx skills add` で 1 コマンド導入するための配布用 Git リポジトリです。

---

## 概要

IT実務における重要文書：
* **提案書（Proposal）**
* **基本・方式設計書（High-Level Design: HLD）**
* **障害・調査報告書（Incident Report: IR）**

これらの文書の読み手は、基本的に**「迅速に判断・意思決定したい」**人です。  
本スキルは、過剰な装飾（グラデーション・絵文字・アイコンカード）を排し、**紙と墨を基調とした高視認性タイポグラフィ、余白設計、本章の結論ボックス、対比グリッド、レスポンシブ表組み、印刷最適化CSS** によって読み手の判断速度を最大化するドキュメントを構築する専門スキルです。

* **Zero External Dependencies**: 外部CDN、外部スクリプト、Webフォントに依存しないオフライン稼働保証。
* **Decision-Making Focus**: 絵文字・不要グラデーションを全廃し、構造・図表・比較表で判断材料を提供。
* **Type A Native Visual Standard**: インラインSVG/CSSによるモノクロ基調＋朱色（`#b5371f`）1色ハイライト、厳密な凡例（Legend）付き。
* **Responsive & Print-Ready**: モバイルでのテーブル縦積みリフロー（`data-label`）および印刷改ページ崩れ防止（`@media print`）。

---

## インストール方法

### 1. GitHub リポジトリから直接インストール
```bash
npx skills add fxzoa/prop-hld-ir-html-skill
```

または明示的にスキル名を指定する場合：
```bash
npx skills add fxzoa/prop-hld-ir-html-skill --skill prop-hld-ir-html
```

### 2. ローカル環境からの検証・追加
```bash
npx skills add ./path/to/prop-hld-ir-html-skill
```

---

## インストール後の確認

```bash
# スキル一覧の確認
npx skills list

# スキルの実行確認
npx skills run prop-hld-ir-html
```

---

## ディレクトリ構成

```text
prop-hld-ir-html-skill/
├── README.md
├── skill.json                         # スキル定義マニフェスト
├── SKILL.md                           # ルート定義
└── skills/
    └── prop-hld-ir-html/              # スキル本体
        ├── SKILL.md                   # スキル仕様・CSSトークン規格・プロンプト定義
        └── resources/
            └── template.html          # 実務向けHTMLテンプレート（紙と墨、レスポンシブ表組み）
```
