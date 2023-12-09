### 概要
- Terraform実行用Dockerコンテナ
- Terraform1.5系の最新versionをインストール

### インストール用URL
* Terraform
https://developer.hashicorp.com/terraform/install

* tfenv
https://github.com/tfutils/tfenv

### 利用手順
```
# ディレクトリ移動
cd docker-terraform

# 起動
docker-compose up -d

# docker接続
docker exec -it terraform.local bash

# 停止、削除
docker-compose down --rmi all --volumes --remove-orphans
```