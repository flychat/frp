# Dockerfile and docker-compose for `fatedier/frp`

## Added

- frp 0.28.2
- docker-compose up -d 
	- then you'll get a socks5 proxy
	- port: 7019 
- privilege_token=frp

## Usage

```bash
# frpc
cp config/frpc.sample.ini config/frpc.ini
emacs -nw config/frpc.ini
docker-compose up -d frpc

# frps
cp config/frps.sample.ini config/frps.ini
emacs -nw config/frps.ini
docker-compose up -d frps
```

> Also check [ `docker-compose.yml` ](docker-compose.yml) for ports settings.

## SEEALSO

- [fatedier/frp](https://github.com/fatedier/frp)
