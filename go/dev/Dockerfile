FROM repo.coloseo.io/base

RUN echo '@edge http://nl.alpinelinux.org/alpine/edge/main' >> /etc/apk/repositories
RUN echo '@community http://nl.alpinelinux.org/alpine/edge/community' >> /etc/apk/repositories

RUN apk update && apk upgrade
RUN apk add curl make git bzr mercurial go@community

RUN rm -rf /var/cache/apk/*

RUN mkdir /go
ENV GOPATH /go

