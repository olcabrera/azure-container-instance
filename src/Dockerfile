FROM python:3.10-alpine

RUN apk update && apk upgrade && \
    apk add --no-cache bash

RUN apk add ffmpeg


WORKDIR /app
COPY ./src/ ./
RUN chmod +x ./docker-entrypoint.sh

EXPOSE 80/tcp
CMD ["./docker-entrypoint.sh"]
