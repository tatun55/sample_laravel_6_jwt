# 【動作確認済(2020年現在)】Laravel6.xでJWT認証機能を実装するサンプル(最低限の構成)

## 機能
- サインアップ
  - ./api/register
- ログイン
  - ./api/login
- ログアウト
  - ./api/logout
- トークン再発行機能
  - ./api/refresh

## 参考
[jwtインストールや設定 \- ララベル\(Laravel\)にトークンベース認証システムを実装するためjwt\(Json Web Token\)ミドルウェア\(Middleware\)をインストールして設定する方法について説明します。](https://dev-yakuza.github.io/laravel/jwt/)

[jwt:会員登録 \- トークンベース認証システムであるjwt\(Json Web Token\)を使って会員登録を実装してみます。](https://dev-yakuza.github.io/laravel/jwt-signup/)

[jwt:ログイン \- トークンベース認証システムであるjwt\(Json Web Token\)を使ってログイン手続きを実装して見ましょう。](https://dev-yakuza.github.io/laravel/jwt-signin/)

[jwt:ユーザ情報 \- トークンベース認証システムであるjwt\(Json Web Token\)を使ってログインしたユーザ情報を取得する方法についてみてみましょう。](https://dev-yakuza.github.io/laravel/jwt-user-info/)

[jwt:トークン更新 \- トークンベース認証システムであるjwt\(Json Web Token\)を使ってログインした後取得したjwtトークンを更新\(Refresh\)する機能を追加して見ましょう。](https://dev-yakuza.github.io/laravel/jwt-refresh-token/)

[jwt:ログワウと \- jwt\(Json Web Token\)認証システムのログアウト機能を実装する方法について見て見ます。](https://dev-yakuza.github.io/laravel/jwt-logout/)

※ 基本的に書いてあるとおりで動きますが、
app/Controllers/JWTAuthController.php
```
use Illuminate\Support\Facades\Auth;
```
の追記が記載されていませんので、追記してください。
