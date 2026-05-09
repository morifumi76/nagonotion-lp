# nagonotion-lp

Notion 勉強ワークショップ「なごNotion」の集客LP。

## 概要
- 名古屋・なごのキャンパスで開催する Notion 勉強ワークショップの単発回への申込を集めるランディングページ
- 主催：ジョウホウソース株式会社（代表：森田 文弥）
- 公開URL：https://nagonotion.johosauce.com

## 技術スタック
- HTML（静的）
- Tailwind CSS（CDN）
- 補助 CSS（`style.css`）
- ホスティング：Vercel
- ドメイン：`nagonotion.johosauce.com`（Xserver で `johosauce.com` を管理、CNAME で Vercel に向けている）

## ローカルでの確認
ビルド不要。ファイルを直接ブラウザで開けば確認できます。

```bash
open index.html
```

## ファイル構成
```
nagonotion-lp/
├─ index.html      … LP本体
├─ style.css       … Tailwind の補助スタイル
├─ README.md       … 本ファイル
├─ docs/specs/     … 仕様書置き場
└─ public/images/  … 画像置き場（差し替え用）
```

## 差し替え箇所一覧
本番運用前に、以下を実データへ差し替えてください。`index.html` 内の `<!-- TODO: 差し替え -->` コメントが該当箇所です。

### ロゴ・画像
- ヘッダーロゴ画像（現状はテキスト「なごNotion」）
- ヒーローのキービジュアル（必要に応じて）
- 主催者プロフィール写真

### Notion リンク（現状すべて `#`）
- 申込みフォーム（Notion）… ヒーローCTA／ヘッダー／最終CTA の3か所
- 当日の流れ 詳細ページ
- 直近のテーマ予告（テーマ一覧ページ）
- 主催者プロフィール詳細ページ
- 過去アーカイブ一覧ページ

### テキスト
- 直近の開催日程（ヒーロー内 `YYYY/MM/DD（◯）HH:MM〜`）
- 直近のテーマ予告 3件分（日付・タイトル）
- 定員人数（参加費・定員・持ち物セクションの「◯名」）

## 公開フロー（参考）
1. ローカルでコードを編集
2. `git add . && git commit -m "更新内容"`
3. `git push origin main`
4. Vercel が自動でデプロイ → `https://nagonotion.johosauce.com` に反映

## 注記
- 本会は会場として「なごのキャンパス」を利用していますが、**なごのキャンパス公式の主催・後援イベントではありません**。
- なごのキャンパスのロゴ・固有デザイン要素は使用していません。

## 作者
森田 文弥 / ジョウホウソース株式会社
