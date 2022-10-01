FROM mcr.microsoft.com/devcontainers/universal:2-linux
LABEL Name=dev-Linxu-Universal Version=0.0.1

WORKDIR /app

COPY .mvn/ .mvn
COPY mvnw pom.xml ./
RUN ./mvnw dependency:resolve

COPY src ./src

CMD ["./mvnw", "spring-boot:run"]
