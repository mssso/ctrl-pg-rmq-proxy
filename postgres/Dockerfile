FROM postgres:12

WORKDIR /tmp 

RUN apt-get install -y build-essential git postgresql-server-dev-12 \
        && git clone https://github.com/omniti-labs/pg_amqp.git \
        && cd pg_amqp \
        && make clean \
        && make install \
        && cd .. \
&& rm -rf pg_amqp
