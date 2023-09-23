FROM nginx

# インクルード用のディレクトリ内を削除
RUN rm -f /etc/nginx/conf.d/*

# Nginxの設定ファイルをコンテナにコピー
# ADD nginx.conf /etc/nginx/nginx.conf
# ADD default.conf /etc/nginx/conf.d/default.conf
ADD app.conf /etc/nginx/conf.d/app.conf

# コンテナの使用ポート指定
# EXPOSE 80

# ビルド完了後にNginxを起動
CMD /usr/sbin/nginx -g 'daemon off;' -c /etc/nginx/nginx.conf
