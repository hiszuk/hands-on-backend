FROM mysql:5.7-debian

# (2) パッケージアップデート
RUN apt-get update

# (3) スクリプトと各種設定ファイルのコピー
COPY ./etc/mysql/mysql.conf.d/mysqld.cnf /etc/mysql/mysql.conf.d/
COPY ./etc/mysql/conf.d/mysql.cnf /etc/mysql/conf.d/

# (4) mysqldの実行
CMD ["mysqld","--character-set-server=utf8","--collation-server=utf8_unicode_ci","--default-time-zone=Asia/Tokyo"]
