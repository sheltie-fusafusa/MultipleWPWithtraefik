# MultipleWP With traefik

複数のWordpressをtraefikで管理するサンプル  
一つのサーバで複数Wordpressを動かしたくなったため、各Wordpressはdocker-composeで構築し、traefikにてルーティングを行うことにしました

# ブログ
より詳細な内容は以下の自分のブログを参考にしてください  
https://sheltie-garage.xyz/tech/2022/05/traefik%e3%82%92%e5%88%a9%e7%94%a8%e3%81%97%e3%81%a6%e8%a4%87%e6%95%b0wordpress%e3%82%921%e5%8f%b0%e3%81%ae%e3%82%b5%e3%83%bc%e3%83%90%e3%81%ab%e6%a7%8b%e7%af%89%e3%81%99%e3%82%8b/

# 注意点
* 事前にDokerネットワークを作成しておきます（コマンド例：docker network create --subnet=192.168.1.0/24 traefik）
* .envファイルは共通なので、各wordpressフォルダに設置する必要があります

# 参考
traefikのdocker-composeは以下リポジトリのものを利用しています  
https://github.com/bubelov/traefik-letsencrypt-compose

