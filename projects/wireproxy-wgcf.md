# wireproxy-wgcf

`wireproxy` と Cloudflare Warp 非公式クライアントである `wgcf` を組み合わせ、コンテナ上で動作するWarp経由のSOCKS5/HTTP プロキシを構築する

## メモ

-   `warp-docker` の代替を目指す

- `wireproxy` を使用することで[--cap-add NET_ADMIN](https://qiita.com/muddydixon/items/d2982ab0846002bf3ea8)の使用を[回避](https://febc-yamamoto.hatenablog.jp/entry/2022/10/24/075354)できるか検証

-  `wireproxy` 側のリポジトリをベースに開発を行う

- 起動時に `register` および `generate` を実行し、プロファイルを自動生成する `docker-entrypoint.sh` を作成する

## 関連リンク

- [1.1.1.1](https://1.1.1.1/) -  The free app that makes your Internet faster.

- [wireproxy ](https://github.com/pufferffish/wireproxy) - A wireguard client that exposes itself as a socks5/http proxy or tunnels.

- [wgcf](https://github.com/ViRb3/wgcf) - wgcf is an unofficial, cross-platform CLI for [Cloudflare Warp](https://1.1.1.1/)

- [warp-docker](https://github.com/cmj2002/warp-docker) - Run official  [Cloudflare WARP](https://1.1.1.1/)  client in Docker.