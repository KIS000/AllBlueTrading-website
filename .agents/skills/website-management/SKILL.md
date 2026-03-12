---
name: website-management
description: All Blue Trading ウェブサイトの管理・更新手順
---

# Website Management Skill

All Blue Trading コーポレートサイトの管理・更新を行うためのスキルです。

## サイト構成

```
AllBlueTrading website/
├── index.html      # メインページ（HTML構造・JSロジック）
├── styles.css      # スタイルシート
└── .agents/
    └── skills/
        └── website-management/
            └── SKILL.md   # このファイル
```

## ローカルでの確認方法

```bash
cd "/Users/ik/Dev/Antigravity/AllBlueTrading website"
npx -y serve .
```

ブラウザで `http://localhost:3000` にアクセスして確認できます。

## コンテンツの更新

### 会社情報を変更する
`index.html` 内の `<table class="info-table">` を編集：
- 所在地、設立、代表、事業内容の「—」を実際の情報に置き換える

### キャッチコピーを変更する
`index.html` 内の `.hero-title` セクションの `<span class="hero-title-line">` のテキストを変更する

### お問い合わせ先を変更する
`index.html` 内の `mailto:info@example.com` を実際のメールアドレスに変更する

## デプロイ

静的サイトのため、以下のホスティングサービスにデプロイ可能：
- **Netlify**: リポジトリ連携またはフォルダドラッグ&ドロップ
- **Vercel**: `npx -y vercel` でデプロイ
- **GitHub Pages**: リポジトリに push して Settings > Pages で有効化

## デザインルール

- **カラー**: 黒（`#000`, `#0a0a0a`, `#111`）× 白（`#fff`, `#f8f8f8`）のみ使用
- **フォント**: Inter + Noto Sans JP
- **アニメーション**: 控えめなフェードイン・ホバー効果に留める
