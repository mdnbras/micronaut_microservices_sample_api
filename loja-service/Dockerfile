#FROM adoptopenjdk/openjdk13-openj9:jdk-13.0.2_8_openj9-0.18.0-alpine-slim
FROM adoptopenjdk/openjdk11-openj9:jdk-11.0.1.13
COPY build/libs/loja-service-*-all.jar loja-service.jar
CMD ["java", "-Dcom.sun.management.jmxremote", "-Xmx128m", "-XX:+IdleTuningGcOnIdle", "-Xtune:virtualized", "-jar", "loja-service.jar"]