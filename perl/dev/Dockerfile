FROM repo.coloseo.io/base

RUN apk update && apk upgrade \
  && apk add perl perl-dev build-base wget curl \
  && curl -L https://cpanmin.us | perl - App::cpanminus \
  && rm -rf /var/cache/apk/*
