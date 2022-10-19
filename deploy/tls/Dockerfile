FROM alpine:3.16
ENTRYPOINT [ "/entrypoint.sh" ]

RUN apk add --no-cache --update --upgrade ca-certificates postgresql-client
RUN apk add -X https://dl-cdn.alpinelinux.org/alpine/v3.16/main -u alpine-keys
RUN apk add --no-cache --update --upgrade --repository=http://dl-cdn.alpinelinux.org/alpine/edge/testing cfssl

COPY . .
