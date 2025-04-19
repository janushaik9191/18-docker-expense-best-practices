FROM mysql:8.0
ENV MYSQL_ROOT_PASSWORD=ExpenseApp@1
RUN groupadd expense && \
    useradd -g expense expense
ADD scripts/*.sql /docker-entrypoint-initdb.d
USER expense
    # MYSQL_DATABASE=transactions \
    # MYSQL_USER=expense \
    # MYSQL_PASSWORD=ExpenseApp@1
    # chown -R expense:expense /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d
    # the above command for ownership not working due to permissions issue of /var/lib/mysql 