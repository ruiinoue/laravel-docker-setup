# laravel-docker-setup

## 基本オプションコマンド

コンテナの立ち上げ

`$ docker-compose up -d --build`

起動コンテナの確認

`$ docker-compose ps`

コンテナに入る

`$ docker-compose exec [サービス名] bash`

コンテナに直で入る

`$ docker-compose exec [サービス名] [実行コマンド]`

コンテナを破棄

`$ docker-compose down`

環境の破壊

`$ docker-compose down --rmi all --volumes --remove-orphans`

## 再構築オプション

①githubからクローン

`$ git clone git@github.com:ruiinoue/laravel-docker-setup.git`

②composerを参照

`$ docker-compose exec app bash`

`$ composer install`

③.env 環境変数ファイルを作成

`$ cp .env.example .env`

④アプリケーションキーを生成

`$ php artisan key:generate`

⑤シンボリックリンクを張る

`$ php artisan storage:link`

⑥storage, bootstrap/cacheに書き込み権限を与える

`$ chmod -R 777 storage bootstrap/cache`
