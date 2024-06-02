FROM mvance/unbound

LABEL org.opencontainers.image.title="Decentralized DNS"

LABEL org.opencontainers.image.description="Decentralized DNS on Emercoin DNS and Alfis DNS blockchain systems"

LABEL org.opencontainers.image.authors="info@wg0.xyz"

LABEL org.opencontainers.image.source="https://github.com/RNDpacman/blockchain_dns_system"

WORKDIR /opt/unbound/etc/unbound

COPY ./emc-stub-records.conf ./insecure-dns.conf ./unbound.conf ./ygg-forward-records.conf .


