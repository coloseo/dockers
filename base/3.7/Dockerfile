FROM alpine:3.7

RUN echo http://mirrors.aliyun.com/alpine/v3.7/main > /etc/apk/repositories && \
    echo http://mirrors.aliyun.com/alpine/v3.7/community >> /etc/apk/repositories && \
    apk update && apk upgrade && \
    apk add --no-cache ca-certificates bash tzdata && \
    rm -rf /var/cache/apk/*
