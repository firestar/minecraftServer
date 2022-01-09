FROM openjdk:17-slim

RUN apt update -y && apt install -y git

COPY ./BuildTools.jar /

RUN java -jar ./BuildTools.jar -o /srv/

WORKDIR /running

CMD java -jar /srv/*.jar

 
