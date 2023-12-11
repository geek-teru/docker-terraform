### 概要
- Terraform実行用Dockerコンテナ
- Amazon Linux release 2023
- Terraform1.5系の最新versionをインストール

### インストール用URL
* Amazonlinux
https://hub.docker.com/_/amazonlinux/

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