## Webサーバー利用だけではないNGINXソリューション
- 田辺 茂也[NGINX]

### NGINXの紹介
#### NGINX社
- オープンソースのnginx開発
- 製品
 - NGINX Plus
   - webサーバーおなじみ
   - ロードバランサーなどにも使える
 - NGINX WAF
   - オープンソースのファイアウォール
 - NGINX Controller
   - NGINX Plusのための集中監視および管理
 - NGINX Unit
   - 複数言語のサポート
- NGINXにより１０倍簡素化・８０％コスト削減

### NGINX Plus
- 高性能なアプリケーションの配信
  - 詳細で豊富なメトリック
  - 強力な負荷分散
  - ヘルスチェック
    - ヘルスチェック用のURLを用意
  - サービスレジストリの結合
  - HTTP/HTTPS/H2/gRPC/TCP/UDP
- NGINX Plusのダッシュボード
  - http://demo.nginx.com
- ロードバランサー・キャッシュ
  - 完全なソフトウェア負荷分散
- APIゲートウェイとして
  - NGINX Plusを買っている人達はAPIゲートウェイとして使っている人達が多い

### NGINX WAF
- 高度なWEBアプリケーションファイアウォール
  - レイヤ7攻撃保護など

### マイクロサービスへの取り組み
- NGINXは、さまざまなマイクロサービスアーキテクチャをサポート
  - Proxy Model
  - Router Mesh Model

### NGINX Unit
- ダイナミックWeb・アプリケーションサーバー
  - シンプル・継承
  - 多言語に対応
  - RESTful JSON APIでの動的な設定
  - オープンソース
  - NGINX Plusユーザーはサポート利用可
  - NGINXをサイドカーに
- dockerhubにイメージある

### 動的なルーティング：サービスの検出


## 本日のスライドは
- 「https://speakerdeck.com/nginx_jp/developers-summit-2019」
