# 画面一覧
- ログインページ
- ユーザー登録ページ
- ユーザー情報詳細ページ
- ユーザー情報編集ページ
- トップページ
- サイト別トップページ
- 問題ページ
- 解答ページ
- 結果ページ
- 学習履歴ページ

# API設計
## 機能
- ユーザー登録/削除
- ログイン/ログアウト
- 自分の情報の取得/更新
- 問題取得
- 解答
- 学習履歴取得

## エンドポイント
||endpoint||method||機能||
|-------------|------|------|
|/users|POST|ユーザーの新規登録|
|/users/:id|GET|特定のユーザー情報取得|
|/users/:id|PUT/PATCH|特定のユーザー情報更新|
|/users/:id|DELETE|特定のユーザーの情報削除|
|/users/:id/answers|POST|問題の解答送信|
|/users/:id/answers|GET|解答履歴取得|
|/problems|POST|新規問題登録|
|/problems|GET|問題取得|
|/problems/:id|GET|特定の問題取得|
|/oauth2/token|POST|ログイン|
