# Navidrome Music Server on Docker

[Navidrome](https://www.navidrome.org/)のサーバをDockerで構築するためのリポジトリ。

## Description

NavidromeはSubsonic APIを実装した軽量な音楽サーバである。Subsonic APIをサポートするクライアントアプリを用いて、スマートフォンやPCから音楽をストリーミング再生できる。

## Requirements

下記環境で動作を確認している。

- Docker 28.3.3
- Docker Compose 2.39.1

## Usage

1. このリポジトリをクローンする
1. `data`ディレクトリを作成する
1. `compose.yaml`の`volumes`セクションを編集し、`/music`に音楽データの保存先を指定する
1. コンテナを`docker compose up -d`で起動する
1. ブラウザで`http://<ホストのIPアドレス>:45335`にアクセスする
1. 初回アクセス時に管理者ユーザの設定を行う
1. Subsonic APIをサポートするクライアントアプリを用いて、音楽をストリーミング再生する

## Author

- [NakuRei](https://github.com/NakuRei)

## License

[MIT License](LICENSE)
