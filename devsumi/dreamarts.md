石田けんすけさん
Dreamarts CTO

## 既存のアプリをマイクロ化してクーバーで管理
- なぜマイクロサービスか
- あ
- a

- 1APIごとに1Docker
- 手に負えなくなってきている
- リファクタリングしたい
### コンテナオーケストレーションでいける？
- kubernetes as a service流行ってきた
- Azure使おう
### マイクロサービス化
- インターフェース化した
- 従来の実装を維持する（ラッピングする）
- springboot + swagger
- コンテナ化
 - WARいらない
 - 組み込みTomcat
 - ビルドプロセスにdocker build 組み込み
- springboot + docker
- イメージをACRにプッシュ
- ACR = プライベートdocker hub
- マイクロサービスにしていくと大量にIPを消費するため、十分なサイズのサブネットを仮想ネットワークに
- サービスのデプロイ
- yamlをたくさん書く
- springbootに設定ファイルを渡す仕組み
 - configMapに登録しておく
 - 参照する
 - コンテナ起動時にファイルとしてマップされる
- yamlの管理　kustomize
 - 共通する定義を作って、そこから継承していく感じ
 - immutable configMap
  - クーバーはconfigmapを変更してもpodを自動で更新してくれない
  - kustomizeでconfigmap名にハッシュ値をいれてimmutable化
- ログ収集
 - deamonset使う
 - kibanaで可視化
- パフォーマンスについて
### CNCF で勉強
### Netflix OSS もマイクロサービス化している
