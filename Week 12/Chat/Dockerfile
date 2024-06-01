FROM openjdk:11

WORKDIR /app


COPY Chat .
COPY Dockerfile .



RUN javac -d out/production/Chat src/*.java

ENV PORT 32000

EXPOSE $PORT

CMD ["java", "-cp", "out/production/Chat", "ChatServer", "32000"]