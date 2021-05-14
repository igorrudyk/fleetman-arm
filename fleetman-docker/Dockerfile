FROM openjdk:8u131-jdk-alpine
RUN apk add --update \
    curl \
    && rm -rf /var/cache/apk/*

EXPOSE 8080

WORKDIR /usr/local/bin/

COPY webapp.jar webapp.jar

CMD ["java", "-Xmx50m","-jar","webapp.jar"]