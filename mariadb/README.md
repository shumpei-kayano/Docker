### 起動のやり方
```
docker compose up -d
```
<font color="red">※compose.yamlのディレクトリで実行すること！</font>
| 環境変数              | 意味                       | 
| :-------------------- | -------------------------- | 
| MARIADB_ROOT_PASSWORD | ルートユーザーのパスワード | 
| MARIADB_DATABASE      | データベース名             | 
| MARIADB_USER          | データベースのユーザー名   | 
| MARIADB_PASSWORD      | データベースのパスワード   | 

[DockerHub:mariadb](https://hub.docker.com/_/mariadb)

### コンテナの中に入る方法
```
# コンテナの中に入る
docker compose exec /bin/bash
# データベースへログインする
mariadb -u testuser -D testdb -p
```