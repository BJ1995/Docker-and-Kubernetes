FROM ubuntu
RUN apt-get update
RUN apt-get install -y maven openjdk-8-jdk
WORKDIR /words
COPY /src ./src/
COPY pom.xml .
RUN mvn verify
CMD java -Xmx8m -Xms8m -jar target/words.jar 
EXPOSE 8080