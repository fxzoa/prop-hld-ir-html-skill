# it-html-document-skill

`it-html-document` スキルを別 PC やチーム環境に `npx skills add` で 1 コマンド導入するための配布用 Git リポジトリです。

---

## 概要

IT現場で使われる文書の読み手は、基本的に**「判断したい」**人です。  
本スキルは、過剰な装飾（グラデーション・絵文字・アイコンカード）を排し、**紙と墨を基調とした高視認性タイポグラフィ、余白設計、本章の結論ボックス、対比グリッド、レスポンシブ表組み、印刷最適化CSS** によって読み手の迅速な意思決定を促すドキュメントを構築する専門スキルです。

* **Zero External Dependencies**: 外部CDN、外部スクリプト、Webフォントに依存しないオフライン稼働保証。
* **Decision-Making Focus**: 絵文字・不要グラデーションを全廃し、構造・図表・比較表で判断材料を提供。
* **Responsive & Print-Ready**: モバイルでのテーブル縦積みリフロー（`data-label`）および印刷改ページ崩れ防止（`@media print`）。

---

## インストール方法

### 1. GitHub リポジトリから直接インストール
```bash
npx skills add btczoa/it-html-document-skill
```

または明示的にスキル名を指定する場合：
```bash
npx skills add btczoa/it-html-document-skill --skill it-html-document
```

### 2. ローカル環境からの検証・追加
```bash
npx skills add ./path/to/it-html-document-skill
```

---

## インストール後の確認

```bash
# スキル一覧の確認
npx skills list

# スキルの実行確認
npx skills run it-html-document
```

---

## ディレクトリ構成

```text
it-html-document-skill/
├── README.md
├── skill.json                         # スキル定義マニフェスト
├── SKILL.md                           # ルート定義
└── skills/
    └── it-html-document/              # スキル本体
        ├── SKILL.md                   # スキル仕様・CSSトークン規格・プロンプト定義
        └── resources/
            └── template.html          # 実務向けHTMLテンプレート（紙と墨、レスポンシブ表組み）
```
