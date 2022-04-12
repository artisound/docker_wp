# Dockerで爆速Wordpress環境構築

## セットアップ(Windows)
* [Windws Terminal](https://www.microsoft.com/ja-jp/p/windows-terminal/9n0dx20hk701?activetab=pivot:overviewtab)
* [Visual Studio Code](https://azure.microsoft.com/ja-jp/products/visual-studio-code/)
* [WSL2](https://docs.microsoft.com/ja-jp/windows/wsl/install)
* [Docker Desktop for Windows](https://docs.docker.com/desktop/windows/install/)


## 環境構築
```
$ docker-comopse up -d
```

|サービス|URL|
|-|-|
|WordPress|http://localhost:8000/|
|phpMyAdmin|http://localhost:8080/|

### Wordpressにつながらない場合...
./public/wp-config.phpの設定情報を確認してください。