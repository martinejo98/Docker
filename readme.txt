docker network create mynetwork

docker run --network mynetwork --name postgres_test -e POSTGRES_USER=postgres -e POSTGRES_PASSWORD=contrasena -e POSTGRES_DB=test postgres

docker inspect postgres_test (sacamos la ip y se la añadimos al application.properties)