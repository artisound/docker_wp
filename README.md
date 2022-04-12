# Dockerで爆速WordPress環境構築

## セットアップ(Windows)
* [Windws Terminal](https://www.microsoft.com/ja-jp/p/windows-terminal/9n0dx20hk701?activetab=pivot:overviewtab)
* [Visual Studio Code](https://azure.microsoft.com/ja-jp/products/visual-studio-code/)
* [WSL2](https://docs.microsoft.com/ja-jp/windows/wsl/install)
* [Docker Desktop for Windows](https://docs.docker.com/desktop/windows/install/)


## 環境構築・起動
オプション`-d`でバッググラウンド起動
```
$ docker-compose up -d
```

|サービス|URL|
|-|-|
|WordPress|http://localhost:8000/|
|phpMyAdmin|http://localhost:8080/|

### WordPressにつながらない場合...
./public/wp-config.phpの設定情報を確認してください。

## Dockerコマンド
### ● コンテナの確認
```
$ docker-compose ps
```
### ● docker-compose.ymlの変更を反映させる
コンテナの再構築
```
$ docker-compose up -d
```
### ● Dockerfile or ビルド処理の変更を反映させる
```
$ docker-compose up -d --build
```
### ● コンテナの停止
```
$ docker-compose stop
```
### ● コンテナの再起動
```
$ docker-compose restart
```
### ● コンテナの削除
```
$ docker-compose rm
```
### ● コンテナの停止、削除、ネットワーク削除、イメージ削除
```
$ docker-compose down --rmi all
```