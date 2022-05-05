FROM openjdk:11.0.14-jdk-slim-bullseye

RUN ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime && \
    echo "Asia/Shanghai" > /etc/timezone

WORKDIR /home/apps/
ADD target/forecast-1.0.0.jar .
ADD start.sh .

ENTRYPOINT ["sh", "/home/apps/start.sh"]
