### Terraform install
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

# コンテナ内作業 -------------------
# ディレクトリ作成 
git clone ${terraform}

# 停止、削除
docker-compose down --rmi all --volumes --remove-orphans
```