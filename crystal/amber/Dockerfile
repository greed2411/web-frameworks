FROM crystallang/crystal:0.26.1

WORKDIR /usr/src/app

COPY shard.yml ./
COPY src src
COPY config config

RUN shards build --release --no-debug

CMD bin/server
