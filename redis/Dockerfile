FROM redis:4-alpine
COPY redis-entrypoint.sh .
RUN mkdir -p /etc/redis &&\
    mkdir -p /var/lib/redis/sentinel &&\
    touch /var/log/sentinel.log &&\
    chown redis:redis /var/log/sentinel.log &&\
    mv redis-entrypoint.sh /etc/redis/redis-entrypoint.sh &&\
    chown redis:redis /etc/redis/redis-entrypoint.sh

ENTRYPOINT [ "/etc/redis/redis-entrypoint.sh" ]