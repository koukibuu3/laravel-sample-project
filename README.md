## これはなに

PHP学習用のサンプルプロジェクトの社内向け資料です。

## 共通要件

PHPとその他の関連技術を用いてアプリケーションを作成すること。

| 項目 | 内容 |
| --- | --- |
| 使用言語 | PHP 8.3.4 （2024/04最新） |
| フレームワーク | Laravel 11 （2024/04最新） |
| データベース | MySQL, PostgreSQL, その他 |
| テンプレートエンジン | Blade |
| フロントエンドフレームワーク | Vue, React, なし, その他 |
| 開発環境 | Docker, Git |

## 課題

以下いずれか（両方でも可）を選んで実施してください。

### A. タスク管理システム

普段PJで使うようなタスク管理アプリケーションの作成を通して、[CRUD](https://developer.mozilla.org/ja/docs/Glossary/CRUD) の実装を経験します。

- [要件](docs/taskApplication.md)

### B. 問い合わせ管理システム

問い合わせを受けるユーザ側と、問い合わせを管理する管理者側の2機能の連携から成り立つアプリケーションを作成します。

- [要件](docs/contactApplication.md)

## 留意事項

- コミットは適切に分割すること
    - 実際にPJでレビューを依頼する際と遜色ない粒度を意識するとGood
- 必要に応じてコメントで意図や補足説明を入れること
    - 説明する際に理解しずらい箇所や意識したポイントを記載いただくとGood
- 要件で定義されていない項目に関しては各自で判断して定義すること
    - 要件はいかようにも解釈できるよう雑に書いているので好きに解釈してください
- 無理はしないこと
    - プロジェクトの作業、および自分の睡眠時間は犠牲にしないでください

## 始め方

### 方法1: このリポジトリをcloneして始める

```sh
# リポジトリをclone
git clone https://github.com/koukibuu3/laravel-sample-project.git

# 初期スクリプトを実行
composer provision

# コンテナを立ち上げる
docker-compose up -d # もしくは ./vendor/bin/sail up -d

# テーブルを作成する
docker-compose exec laravel.test composer migrate
```

### 方法2: Laravel公式ドキュメントを参考に始める

https://laravel.com/docs/11.x
