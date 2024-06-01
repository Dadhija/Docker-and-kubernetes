FROM openjdk:11

WORKDIR /app


COPY Chat .
COPY Dockerfile .



RUN javac -d Chat/out/production/Chat Chat/src/*.java

ENV PORT 32000

EXPOSE $PORT

CMD ["java", "-cp", "Chat/out/production/Chat", "ChatServer", "32000"]