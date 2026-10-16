# Base image
FROM mysql/mysql-server:5.7

# ENVIRONMENT VARIABLES
ENV MYSQL_ROOT_PASSWORD=root
ENV MYSQL_USER=root
ENV MYSQL_DATABASE=your_database_name

# PROVDING PORTS
EXPOSE 3306

# COPYING and ensuring permissions
COPY database.sql /docker-entrypoint-initdb.d/
RUN chmod 644 /docker-entrypoint-initdb.d/database.sql
