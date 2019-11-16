# Sample app using Quarkus with MySQL

## Start mysql with following:
docker run \
    --name mysql \
    -p 3306:3306 \
    -e MYSQL_DATABASE=quarkus \
    -e MYSQL_USER=user \
    -e MYSQL_PASSWORD=password \
    -e MYSQL_ROOT_PASSWORD=admin \
    -d \
    mysql:latest

## Start app with:
mvn compile quarkus:dev

## Connect to endpoint at
 http://localhost:8080/person