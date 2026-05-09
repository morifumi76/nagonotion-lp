# nagonotion-lp

## 概要
Notion 勉強ワークショップ「なごNotion」の集客LP。
名古屋・なごのキャンパスで開催する単発回への申込（Notion フォーム）への遷移を主ゴールとする。

## 技術スタック
- フレームワーク: なし（静的HTML）
- 言語: HTML / CSS / 最小限の JS
- スタイル: Tailwind CSS（CDN）＋ 補助 `style.css`
- デプロイ先: Vercel
- 独自ドメイン: `nagonotion.johosauce.com`（親ドメイン `johosauce.com` は Xserver 管理）

## フォルダ構成
```
nagonotion-lp/
├─ index.html      … LP本体（1ファイルで全セクション）
├─ style.css       … 補助スタイル（フォーカスリング等）
├─ README.md       … 差し替え箇所一覧と運用ガイド
├─ docs/specs/     … 仕様書置き場
└─ public/images/  … 画像置き場
```

## このプロジェクト固有のルール
- デザインは「ミニマル / モダン / クリーン / 余白多め / 誠実」を厳守。装飾は最小限。
- カラーパレット（`tailwind.config` で定義）から外れた色を新規追加しない。
  - 背景 `#FFFFFF` / `#FAFAFA` / 本文 `#1A1A1A` / サブ `#6B6B6B` / 区切り `#E5E5E5` / アクセント `#111111` / `#2A4A8B`（深い藍：CTAやリンクのみ）
- フォントは `Noto Sans JP` と `Inter` のみ。明朝体・装飾フォントは使わない。
- スマホファースト（375px起点）。セクション間の上下余白は 80〜120px を目安。
- アクセント色は「ヒーローCTA」と「最終CTA」など、ここぞの 1〜2 か所のみ。
- 「**なごのキャンパス公式の主催・後援ではありません**」の注記を、会場情報セクションとフッターから外さないこと。
- なごのキャンパスのロゴ・固有のデザイン要素は使用しない。
- 各種 Notion リンクは `#` プレースホルダ ＋ `<!-- TODO: 差し替え -->` コメントで管理し、リンクが増減してもコメントを残す。
- パスワード・APIキーは絶対にコミットしない。

## 主要な外部サービス
- Notion: 申込みフォーム／当日の流れ／テーマ予告／プロフィール／アーカイブの遷移先
- Vercel: ホスティング・SSL自動発行
- Xserver: 親ドメイン `johosauce.com` のDNS管理（CNAME `nagonotion → cname.vercel-dns.com`）
- GitHub: `johosauce/nagonotion-lp`

## 現在の状態
- LP（index.html）実装済み・全セクション配置済み
- Vercel デプロイ済み・カスタムドメイン `nagonotion.johosauce.com` 紐付け済み
- 差し替え対象（日程・Notion リンク・写真・ロゴ）はプレースホルダで残置中。本番公開前に README の「差し替え箇所一覧」を参照して更新すること。
