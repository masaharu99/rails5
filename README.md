# Rails5の環境構築

## バージョン
Ruby：2.5.9
Rails：5.2.1

## 構築手順
1. `docker compose build`でイメージをビルドする
2. `docker compose run web rails new . --database=postgresql`でRailsアプリケーションを作成する
3. `database.yml`のdefault設定に下記を追加する
```
host: db
username: postgres
password: password
```
