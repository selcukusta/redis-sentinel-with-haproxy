FROM haproxy:1.9.4-alpine

COPY haproxy.cfg .

RUN mkdir -p /etc/haproxy &&\
    cp haproxy.cfg /etc/haproxy/haproxy.cfg

CMD [ "haproxy", "-f", "/etc/haproxy/haproxy.cfg" ]