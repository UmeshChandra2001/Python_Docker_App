# Base image
FROM mysql/mysql-server:5.7

# ENVIRONMENT VARIABLES
ENV MYSQL_ROOT_PASSWORD=root
ENV MYSQL_USER=root

# PROVDING PORTS
EXPOSE 3306

# COPYING
COPY database.sql /docker-entrypoint-initdb.d/database.sql
