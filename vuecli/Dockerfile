FROM node:10.15.3-alpine

# 静的コンテンツを配信するシンプルな http サーバをインストールする
# RUN npm install -g http-server

# カレントワーキングディレクトリとして 'app' フォルダを指定する
WORKDIR /app

# vuecliインストール
RUN npm install -g @vue/cli

#shファイルをコンテナにコピー
COPY ./scripts/docker.start.sh /scripts/start.sh

#shフォルダの権限追加（全員実行可）
RUN chmod +x /scripts/*

#初期実行
# ENTRYPOINT [ "/scripts/start.sh" ]
