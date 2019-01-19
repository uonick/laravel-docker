ARG DB_PORT
ARG MYSQL_VERSION

FROM mysql:${MYSQL_VERSION}
RUN ln -snf /usr/share/zoneinfo/UTC /etc/localtime && echo UTC > /etc/timezone && chown -R mysql:root /var/lib/mysql/

CMD ["mysqld"]

EXPOSE ${DB_PORT}
