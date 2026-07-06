# YamaTrip (ヤマトリップ)

Next.jsとSupabaseを用いた、「登山 ＋ 下山後の楽しみ（温泉・食事処）」をセットで記録・共有できるコミュニティアプリです。

## アプリ概要
「山自体の情報はたくさんあるけれど、下山した後のルート（近くの温泉や美味しいご飯）を一目で網羅できるサービスが欲しい」という登山好きの課題を解決するために開発しました。

## サイトイメージ
![トップページ](https://github.com/kjob331/YamaTrip/blob/main/public/images/top.png?raw=true)

## サイトURL
- 本環境：https://yama-trip.vercel.app/
- テスト用アカウント (※デモ環境のためメール認証省略)
  - メールアドレス：`jirou@au.com`
  - パスワード：`jirou2222`

---

## 使用技術
- フロントエンド：Next.js 15.0 (React 19)
- バックエンド：Next.js 15.0 (Server Actions / API Routes)
- データベース：Supabase (PostgreSQL)
- ストレージ：Supabase Storage (画像アップロード用)
- デプロイ：Vercel
  本番環境のホスティングに採用。GitHubの `main` ブランチと連携させ、プッシュ時に自動ビルド・デプロイが行われるCI/CDフローを構築しています。
- バージョン管理：Git、GitHub
- テスト・デバッグ：DevTools (Chrome)

## 設計ドキュメント
- [要件定義・基本設計・詳細設計の一覧_Googleスプレッドシート](https://docs.google.com/spreadsheets/d/1QX1W0dDTDDAWHH39mY0Be4LiU5QC_3Dx-ipYAeAnDO4/edit?usp=sharing)
- 詳細設計時のワイヤーフレーム、ER図、ワークフロー図、SUPABASEのRLS設定の画像は[docsディレクトリ](docs/)に格納しています。

## 機能一覧
・ユーザー登録、ログイン、ログアウト機能
・マイページ機能
・新規投稿作成機能（山名、登山記録、温泉名・感想、食事処名・感想、写真のアップロード）
・投稿編集、削除機能
・最新投稿一覧表示機能
・投稿詳細表示機能
・山名による部分一致検索機能
・AIハイライト機能（Google Gemini API連携）
・登山リアルタイム天気情報機能（Weather API連携）

## テスト・修正の設計及び実施書
- [テスト・修正の設計及び実施書_Googleスプレッドシート](https://docs.google.com/spreadsheets/d/1MOdiU0AjcNdVJQ6LuaObR7MIRlf8rA-VntHr6vOXRSU/edit?usp=sharing)

## アプリの改善案
- [アプリの改善案_Googleスプレッドシート](https://docs.google.com/spreadsheets/d/1qBeG12q0D39IeA8tPj1i__x1U-VmaRKPVL9Po0Klpmw/edit?usp=sharing)

## 備考
- [ESLintの実行結果_GitHub Actions](https://github.com/kjob331/YamaTrip/actions/runs/28734187588)
