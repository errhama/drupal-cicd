# Use the official MySQL image
FROM ubuntu/mysql

# Set environment variables
ENV MYSQL_DATABASE=drupaldb
ENV MYSQL_USER=root
ENV MYSQL_PASSWORD=newpassword

# Copy the initialization SQL file into the container
COPY ./docker/mysql/init /docker-entrypoint-initdb.d/

# Expose the port
EXPOSE 3306
