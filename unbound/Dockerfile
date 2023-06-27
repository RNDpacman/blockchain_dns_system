FROM mvance/unbound

LABEL name="BlockChain DNS"

WORKDIR /opt/unbound/etc/unbound

COPY ./emc-stub-records.conf .

COPY ./insecure-dns.conf .

COPY ./unbound.conf .

COPY ./ygg-forward-records.conf .


