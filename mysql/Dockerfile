# FROM arm64v8/mysql:8.3.0
FROM biarms/mysql:5.7

# docker 会自动执行以下目录的 *.sh, *.sql, *.sql.gz
COPY ./init_scripts/ /docker-entrypoint-initdb.d

# conf 文件拷贝到镜像对应位置
COPY ./my.cnf /etc/mysql/my.cnf

EXPOSE 3306