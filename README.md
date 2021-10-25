# docker-wordpress
dockerでwordpress環境の構築テンプレート。

## 起動
`docker compose up` or `docker compose up -d`

## 停止
`docker compose down`

## エラー対応
- Error establishing a database connection
古いvolumeがないか確認する。削除。  
`docker volume prune`
- wp-config.phpとdocker設定があっているかを確認。
