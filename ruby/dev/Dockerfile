FROM repo.coloseo.io/ruby

RUN apk update && apk upgrade \
    && apk add curl git make \
    openssl-dev libssl1.0 build-base libxml2-dev libxslt-dev libbz2 libevent-dev libffi-dev glib-dev ncurses-dev readline-dev yaml-dev zlib-dev \
    libpq sqlite-dev mariadb-libs postgresql-dev \
    ruby-dev ruby ruby-io-console ruby-bundler \
    && rm -rf /var/cache/apk/*

# Now upate bundler: https://github.com/iron-io/dockers/issues/50
RUN gem install --no-rdoc --no-ri bundler
