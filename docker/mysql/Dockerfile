# Use the official MySQL image
FROM ubuntu/mysql

# Set environment variables
ENV MYSQL_ROOT_PASSWORD=newpassword
ENV MYSQL_DATABASE=drupaldb
ENV MYSQL_USER=hamza
ENV MYSQL_PASSWORD=newpassword

# Copy the initialization SQL file into the container
COPY ./docker/mysql/init /docker-entrypoint-initdb.d/

# Expose the port
EXPOSE 3306
