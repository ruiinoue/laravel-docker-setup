# laravel-docker-setup

## 基本オプションコマンド

コンテナの立ち上げ

`$ docker-compose up -d --build`

起動コンテナの確認

`$ docker-compose ps`

コンテナに入る

`$ docker-compose exec [サービス名] bash`

コンテナに直で入る

`$ docker compose exec [サービス名] [実行コマンド]`

コンテナを破棄

`$ docker-compose down`

環境の破壊

`$ $ docker-compose down --rmi all --volumes --remove-orphans`
