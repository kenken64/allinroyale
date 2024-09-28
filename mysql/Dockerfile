# Use the official MySQL image as a base
FROM mysql:latest


# Set the default user for the MySQL image
USER mysql

ENV MYSQL_DATABASE=allinroyaledb 
#ENV MYSQL_USER=root
ARG MYSQL_ROOT_PASSWORD
ENV MYSQL_ROOT_PASSWORD=${MYSQL_ROOT_PASSWORD}
#ADD ./sql-scripts/database.sql /docker-entrypoint-initdb.d
ADD mysqld.cnf /etc/mysql/mysql.conf.d/mysqld.cnf

EXPOSE 3306:3306
EXPOSE 33060:33060
