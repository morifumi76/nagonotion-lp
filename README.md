# なごNotion LP

Notion勉強ワークショップ「なごNotion」の集客LPです。スマホファーストの静的HTML/CSS構成で、ロゴ・写真・開催情報・Notionリンクを後から差し替えやすいようにしています。

## ファイル構成

- `index.html`：LP本体
- `style.css`：デザイン、レスポンシブ、アクセシビリティ調整
- `assets/nago-notion-icon.svg`：なごNotionアイコン、ファビコン
- `assets/nago-notion-icon.png`：なごNotionアイコン、Apple Touch Icon用
- `assets/workshop-venue.jpg`：ワークショップ会場写真
- `assets/johosauce-text-logo.png`：右上リンク用の会社テキストロゴ
- `assets/johosauce-icon.png`：会社アイコン
- `assets/fumiya-morita-profile.png`：主催者プロフィール写真
- `assets/characters/`：4キャラクターの吹き出し用画像
- `assets/characters/animated/`：CSSスプライト用の横長アニメーション画像
- `README.md`：差し替え箇所一覧

## 差し替え箇所

`index.html` 内の `ここを差し替え` コメントを検索してください。

- サイト名：ヘッダー左の `.logo-text`。現在はアイコンなしの `なごNotion`。
- ファビコン：`assets/nago-notion-icon.svg`。Apple Touch Iconは `assets/nago-notion-icon.png`。
- 右上の会社ロゴ：`assets/johosauce-text-logo.png` とヘッダー内の `.header-company-logo`。リンク先は `https://johosauce.com`。
- 写真：ヒーロー右側の `.photo-slot`。現在は `assets/workshop-venue.jpg`。
- 主催者プロフィール写真：`assets/fumiya-morita-profile.png` と主催者プロフィール内の `.profile-photo`。
- キャラクター吹き出し：`index.html` の `.character-callout`。動きは `assets/characters/animated/` のCSSスプライト。
- 直近日程：ヒーロー内の `近日公開`。
- 開催頻度：ヒーロー右側の `月2回`。
- Notion申込フォームURL：ヒーローCTA、最終CTA。現在は `https://johosauce.notion.site/Notion-35b64d2aa0e880018871ee3bc3197c03?pvs=74`。
- 当日の流れNotionページURL：当日の流れセクション。現在は `https://www.notion.so/morifumi76/35b64d2aa0e8805ebad8ffd1bedcbe46`。
- 直近テーマNotionページURL：直近のテーマ予告セクション。現在は `https://www.notion.so/morifumi76/35b64d2aa0e8805ebad8ffd1bedcbe46`。
- 主催者プロフィールNotionページURL：主催者プロフィールセクション。現在は `https://johosauce.notion.site`。
- 過去アーカイブNotionページURL：過去アーカイブセクション。現在は `https://johosauce.notion.site/35b64d2aa0e88037b3c5eefbaf966eec?pvs=74`。
- 定員：参加費・定員・持ち物セクションの `各回少人数制予定`。
- 所在地・連絡先：フッターの所在地と問い合わせリンク。現在の問い合わせ先は `https://johosauce.notion.site/27c64d2aa0e8802ba7a3c70435788fca`。

## Googleマップ

会場は以下の住所でGoogleマップを埋め込んでいます。

愛知県名古屋市西区那古野2丁目14-1

埋め込み先を変更する場合は、会場情報セクションの `iframe src` と `Googleマップで開く` リンクの `href` を差し替えてください。

## 表示確認

静的ファイルなので、`index.html` をブラウザで開くだけで確認できます。ローカルサーバーで確認する場合は次のコマンドを使えます。

```bash
python3 -m http.server 8000
```

その後、ブラウザで `http://localhost:8000` を開いてください。
