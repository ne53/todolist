# caclico-bfd

`calico` に対してネットワークの障害検出を高速に行うプロトコルである`BFD` を実装する

## メモ

- `Calico Cloud` には実装されているが[OSS版には実装されていない](https://docs.tigera.io/calico-cloud/reference/resources/bfdconfig)

- プルリクエスト自体は歓迎されているがenv varではなく、API構造を変更する必要があると[指摘されている](https://github.com/projectcalico/calico/issues/4607)

-  `BFD` が実装されていないのはかなり不便であるため、雑な形になってもいいのでフォークして実装する

## 関連リンク

- [BFD configuration](https://docs.tigera.io/calico-cloud/reference/resources/bfdconfig) - Calico Documentation - Tigera

- [bird.cfg.template](https://github.com/projectcalico/calico/blob/master/confd/etc/calico/confd/templates/bird.cfg.template) - projectcalico/calico

- [ルーティングソフトウェア BIRD の使いかた](https://blog.cybozu.io/entry/bird) - Cybozu Inside Out

- [Support BFD in the confd generated bird configuration #4607](https://github.com/projectcalico/calico/issues/4607)