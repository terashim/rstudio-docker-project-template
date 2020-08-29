ローカル Docker RStudio Server プロジェクトのテンプレート
==================================================

## 前提条件

- [Docker Desktop](https://www.docker.com/products/docker-desktop) for Windows/Mac
    - Docker 18.06 以上

## 初期設定

1. ブラウザで [terashim/rstudio-docker-project-template](https://github.com/terashim/rstudio-docker-project-template) を開き、このテンプレートから新規リポジトリをさくせいする。
2. そのリポジトリをローカルマシンにクローンする
3. 以下のファイルを編集する
    - `_rstudio/Dockerfile`
        - ベースイメージの変更、パッケージのインストール、グローバルオプションの設定などを行う。
    - `_rstudio/docker-compose.yml`
        - ビルドするイメージ名 `your-project-name:latest` を変更する。

---

## 使い方

1. RStudio Server を開始する:
    ```sh
    docker-compose up -d
    ```
2. ブラウザで <http://localhost:8787> を開き RStudio Server に接続する。
3. R プロジェクト `/home/rstudio/project/project.Rproj` を開く
4. 分析を行う
5. RStudio Server を停止する:
    ```sh
    docker-compose down
    ```
