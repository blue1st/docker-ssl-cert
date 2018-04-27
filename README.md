# docker-ssl-cert

Creating a Self-Signed SSL Certificate on Docker

## Usage

```bash
docker run --rm \
	-v $PWD:/ssl/ \
	-e COUNTROY=JP \
	-e STATE=Tokyo \
	-e LOCAL=Shibuya \
	-e ORGANIZATION=hogehoge \
	-e UNIT=fugafuga \
	-e FQDN=piyopiyo.net \
	blue1st/ssl-cert
Generating RSA private key, 2048 bit long modulus
............+++
............+++
e is 65537 (0x10001)
Signature ok
subject=/C=JP/ST=Tokyo/L=Shibuya/O=hogehoge/OU=fugafuga/CN=piyopiyo.net
Getting Private key

$ ls
server.crt	server.csr	server.key
```

