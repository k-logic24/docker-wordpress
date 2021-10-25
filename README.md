# docker-wordpress
dockerでwordpress環境の構築テンプレート。

## 起動
`docker compose up` or `docker compose up -d`

## 停止
`docker compose down`

## メモ
app配下にwp-includesがあるのは、エディタ（IDE）都合上、integration使用で読み込ませるため。  
不要なら削除しても構わない。

## エラー対応
- Error establishing a database connection
古いvolumeがないか確認する。削除。  
`docker volume prune`
- wp-config.phpとdocker設定があっているかを確認。
