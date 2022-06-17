docker network create mynetwork

docker run --network mynetwork --name postgres_test -ePOSTGRES_USER=postgres -e POSTGRES_PASSWORD=contrasena -e POSTGRES_DB=test postgres

docker inspect postgres_test (sacamos la ip y se la añadimos al application.properties)

docker java -jar X.jar (arranca mi jar, pero dentro del directorio target)

docker build -t nombre (me crea la imagen con ese nombre)

docker run --network=mynetwork -p8081:8081 nombre (arranca la aplicación dentro de la red que le he especificado)

///////////////////////

docker ps (vemos los que existen)

docker ps -a vemos los que están en marcha)