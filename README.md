#budowanie obrazu maven:
mvn spring-boot:build-image -Dspring-boot.build-image.imageName=czarek7777/example:hello


#odpalanie na docker lokalnie:
docker run -p 8080:8080 czarek7777/example:hello

#logowanie do dockerhub:
docker login --username=czarek7777

#push
docker push czarek7777/example:hello
