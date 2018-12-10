ARG MYSQL_PORT
ARG MYSQL_VERSION
ARG MYSQL_ROOT_USER
ARG MYSQL_ROOT_PASSWORD

FROM mysql:${MYSQL_VERSION}
RUN ln -snf /usr/share/zoneinfo/UTC /etc/localtime && echo UTC > /etc/timezone && chown -R mysql:root /var/lib/mysql/

COPY config-overrides.cnf /etc/mysql/conf.d/my.cnf

CMD ["mysqld"]

EXPOSE ${MYSQL_PORT}
