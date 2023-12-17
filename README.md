# Emercoin DNS, Alfis DNS and Unbound DNS in a docker

Get access to blockchain-based dns systems on your PC (EmerDNS, Alfis DNS and ClearNet)

## Install
Clone git:

```
git clone https://github.com/RNDpacman/blockchain_dns_system.git
```
```
cd ./blockchain_dns_system
```
Run containers with a compose:

```
docker-compose up -d
```

Wait a while for the blockchain data to download and try it.

Check progress download emercoin blockchain:
```
docker exec emer-dns emercoin-cli -datadir=/emc getinfo

...
 "blocks": 639227,
...

```
## Check resolve
Alfis DNS:
```
host howto.ygg 127.0.0.1
```
EmerDNS:
```
host rtfm.emc 127.0.0.1

```
Clearnet
```
host iana.org 127.0.0.1
```
## Custom

If you want something special you can configure unbound.conf to suit your needs:
```
vim ./unbound.conf
```
For example, enable logging:
```
server:
  log-queries: yes
  log-replies: yes
  logfile: /dev/stdout
  verbosity: 3
```
View logs:
```
docker compose logs unbound
```
