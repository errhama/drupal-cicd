# Use the official MySQL image
FROM mysql:8.0

RUN apt-get update && apt-get install -y procps

# Set environment variables
ENV MYSQL_ROOT_PASSWORD=rootpassword
ENV MYSQL_DATABASE=drupaldb
ENV MYSQL_USER=dbuser
ENV MYSQL_PASSWORD=fwfiweio

# Copy the initialization SQL file into the container
COPY  ./docker/mysql/init  /docker-entrypoint-initdb.d/

# Expose the port
EXPOSE 3306