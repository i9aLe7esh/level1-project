from bryandollery/maven-repo as build

arg rebuile 

COPY src /home/app/src
COPY pom.xml /home/app
RUN mvn -f /home/app/pom.xml clean package

from adoptopenjdk/openjdk11:alpine

copy --from=build home/app/target/person-service-1.0.0.jar / 
CMD ["java", "-Dspring.profiles.active=postgresql", "-Dspring.datasource.url=jdbc:postgresql://petclinic-db:5432/petclinic", "-jar", "person-service-1.0.0.jar"]

EXPOSE 8081
