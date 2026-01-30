# ARG「海蝕機関」完全版 v2.0

## 📋 プロジェクト概要

架空の秘密組織「海蝕機関」を舞台としたWebベースのARG（Alternate Reality Game）プロジェクトの完全版です。
公開サイト（東亜先端研究株式会社）と内部ポータル（解奇日記）の二層構造により、段階的な没入体験を提供します。

**バージョン**: 2.0.0  
**リリース日**: 2026年1月30日  
**制作**: © 志文--

## 🎯 v2.0の新機能

### 📰 公開サイトの大幅拡充
- **ニュースページ**: 10件の記事（事案報告、プレスリリース、研究成果）
- **FAQページ**: 30問以上のQ&A、検索機能付き
- **企業情報**: 詳細な会社概要、沿革、組織図
- **事業内容**: 4サービスの詳細説明、料金表
- **研究姿勢**: 基本理念、倫理規範、品質管理プロセス
- **お問い合わせ**: 特殊案件フォーム（隠し要素）

### 🔍 内部ポータルの機能強化
- **高度な検索**: 部門・脅威レベル・日付フィルター
- **タイムライン表示**: 時系列での事案可視化
- **プログレストラッカー**: 12種類のバッジシステム
- **ブックマーク機能**: メモ・タグ・共有機能
- **テーママネージャー**: 5つのプリセット、カスタマイズ可能

### 🎮 謎解き要素の追加
- 20以上のイースターエッグ
- 複数の認証コードパス
- コンソールログのヒント
- 黒塗りテキスト
- Konamiコード

## 🚀 クイックスタート

### ローカルサーバーの起動

```bash
# Python 3の場合
cd ARG-main-complete
python -m http.server 8000

# Node.jsの場合
npx http-server -p 8000
```

ブラウザで `http://localhost:8000` にアクセス

### デモアカウント

**内部ポータルログイン**:
- URL: `http://localhost:8000/internal/login.html`
- ユーザーID: `GUEST`
- パスワード: `boundary2026`

**認証コード**:
- `boundary` - 境界
- `kaishoku` - 海蝕

## 📁 ディレクトリ構造

```
ARG-main-complete/
├── index.html              # トップページ（謎解き要素付き）
├── company.html            # 企業情報（詳細版・500行）
├── services.html           # 事業内容（556行）
├── research.html           # 研究姿勢（503行）
├── contact.html            # お問い合わせ（特殊フォーム・435行）
├── news.html              # ニュース（NEW・466行）
├── faq.html               # FAQ（NEW・513行）
├── styles.css             # メインスタイルシート
├── privacy.html           # プライバシーポリシー
├── 404.html               # エラーページ
├── sitemap.xml            # サイトマップ
├── robots.txt             # ロボットファイル
│
├── internal/              # 内部ポータル
│   ├── login.html         # ログイン
│   ├── index.html         # ダッシュボード
│   ├── search.html        # 高度な検索（NEW）
│   ├── dashboard.html     # 統合ダッシュボード（NEW）
│   ├── diaries.html       # 日記
│   ├── log-detail.html    # 日報詳細
│   ├── protocol.html      # 機密規約
│   ├── about.html         # 部門情報
│   ├── chat.html          # チャット（予定）
│   │
│   ├── css/
│   │   ├── main.css
│   │   ├── components.css
│   │   └── ui_improvements.css  # NEW
│   │
│   ├── js/
│   │   ├── main.js
│   │   ├── search.js
│   │   ├── search_enhanced.js     # NEW
│   │   ├── progress_tracker.js    # NEW
│   │   ├── bookmark_manager.js    # NEW
│   │   ├── theme_manager.js       # NEW
│   │   ├── components.js
│   │   └── utils.js
│   │
│   ├── deta/
│   │   ├── logs.json               # 元の3件
│   │   ├── logs_enhanced.json      # NEW: 11件
│   │   ├── diaries.json            # 元の3件
│   │   └── diaries_enhanced.json   # NEW: 12件
│   │
│   ├── division/          # 部門別ページ
│   │   ├── convergence.html
│   │   ├── port.html
│   │   ├── craft.html
│   │   ├── support.html
│   │   └── foreign.html
│   │
│   └── components/
│       ├── header.html
│       └── footer.html
│
└── docs/                  # ドキュメント
    ├── ARG_海蝕機関_評価と拡張計画書.docx
    ├── ARG_海蝕機関_コンテンツ例集.docx
    ├── IMPLEMENTATION_GUIDE.md
    ├── UI_UX_IMPROVEMENTS_README.md
    └── PUBLIC_SITE_README.md
```

## 🎯 主要機能

### 公開サイト

| ページ | 内容 | 行数 |
|--------|------|------|
| index.html | トップページ + 謎解き | 400+ |
| company.html | 会社概要、沿革、組織図 | 500+ |
| services.html | 4サービス詳細、料金表 | 556 |
| research.html | 理念、倫理、品質管理 | 503 |
| contact.html | フォーム + 特殊案件 | 435 |
| news.html | 10記事、フィルター機能 | 466 |
| faq.html | 30問、検索機能 | 513 |

### 内部ポータル

| 機能 | 説明 |
|------|------|
| 高度な検索 | 部門・脅威レベル・日付フィルター |
| タイムライン | 時系列表示 |
| プログレストラッカー | 12バッジ、自動記録 |
| ブックマーク | メモ・タグ・共有 |
| テーマ | 5プリセット + カスタム |

### データ

- **日報**: 11件（権限レベル1-4）
- **日記**: 12件（多様な視点）
- **ニュース**: 10記事
- **FAQ**: 30問以上

## 🔐 イースターエッグ一覧

| 場所 | トリガー | 結果 |
|------|---------|------|
| index.html | ロゴを7回クリック | 座標ヒント |
| index.html | Konamiコード | 内部ポータルへ |
| company.html | 組織ボックス5回 | ログインID表示 |
| company.html | Konamiコード | 画面エフェクト |
| services.html | 黒塗り3回クリック | 内容表示 |
| research.html | 警告5回クリック | 緊急メッセージ |
| contact.html | ロゴ5回クリック | 認証コード表示 |
| contact.html | 特殊案件 + 認証 | 内部ポータルへ |
| faq.html | 「海蝕」で検索 | ヒント表示 |
| news.html | 黒塗り3回クリック | 内容表示 |

## 📊 コンテンツ統計

- **HTMLページ**: 25+
- **JavaScriptファイル**: 10+
- **CSSファイル**: 15+
- **JSONデータ**: 4ファイル
- **ドキュメント**: 5ファイル
- **総コード行数**: 7,000行以上
- **日報**: 11件
- **日記**: 12件
- **ニュース**: 10記事
- **FAQ**: 30問以上
- **バッジ**: 12種類
- **イースターエッグ**: 20+

## 🛠️ 使用技術

- HTML5, CSS3
- Vanilla JavaScript (ES6+)
- JSON (データ管理)
- SessionStorage (認証)
- LocalStorage (設定・進捗)
- CSS Variables (テーマ)
- ES6 Modules
- Google Fonts

## 📱 レスポンシブ対応

全ページがモバイル対応:
- デスクトップ: 1920px+
- タブレット: 768-1919px
- スマートフォン: ~767px

## 🎮 推奨プレイフロー

1. **発見**: トップページから探索開始
2. **疑問**: 企業情報で違和感を感じる
3. **探索**: ニュース・FAQで異常を発見
4. **謎解き**: 黒塗り、コンソールヒントを探す
5. **突破**: 認証コードで内部ポータルへ
6. **没入**: 日報・日記で世界観を理解
7. **達成**: バッジ獲得、全コンテンツ探索

## 📚 ドキュメント

詳細は `docs/` ディレクトリ参照:
- `IMPLEMENTATION_GUIDE.md` - 実装ガイド
- `UI_UX_IMPROVEMENTS_README.md` - UI/UX詳細
- `PUBLIC_SITE_README.md` - 表サイト詳細
- `評価と拡張計画書.docx` - プロジェクト評価
- `コンテンツ例集.docx` - 追加コンテンツ例

## 🔄 v1.0からの変更点

### 追加されたページ
- news.html (ニュース)
- faq.html (よくある質問)
- dashboard.html (統合ダッシュボード)

### 拡張されたページ
- company.html: 100行 → 500行
- services.html: 150行 → 556行
- research.html: 200行 → 503行
- contact.html: 200行 → 435行

### 新機能
- プログレストラッカー
- ブックマーク機能
- テーママネージャー
- 高度な検索
- タイムライン表示

### データ拡充
- 日報: 3件 → 11件
- 日記: 3件 → 12件
- イースターエッグ: 5個 → 20個以上

## ⚠️ 注意事項

このプロジェクトはフィクションです:
- 実在の人物・団体・事件とは無関係
- 架空の電話番号・住所を使用
- 個人情報を収集しない
- 倫理的なコンテンツ

## 🔮 今後の拡張予定

- バックエンド実装 (Node.js + Express)
- データベース (PostgreSQL)
- 本格的な認証 (JWT)
- リアルタイムイベント (Socket.io)
- マルチメディアコンテンツ
- コミュニティ機能
- モバイルアプリ (PWA)

## 📄 ライセンス

フィクションARGプロジェクトとして提供

---

**制作**: © 志文-- All Rights Reserved.  
**バージョン**: 2.0.0  
**リリース**: 2026年1月30日
