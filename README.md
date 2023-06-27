# Emercoin DNS, Alfis DNS and Unbound DNS in a docker

Get access to blockchain-based dns systems on your PC (EmerDNS, Alfis DNS)


Clone git:

```
git clone https://github.com/RNDpacman/blockchain_dns_system.git
```
```
cd ./blockchain_dns_system
```

Run buld docker image:

```
docker build -t unbound ./unbound
```

Run containers with a compose:

```
docker-compose up -d
```

Wait a while for the blockchain data to download.

And try it:

```
dig @127.0.0.1 howto.ygg aaaa
dig @127.0.0.1 rtfm.emc
dig @127.0.0.1 iana.org
 
```