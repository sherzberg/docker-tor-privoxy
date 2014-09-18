Docker Tor Privoxy
==================

Simple container for turning a tor proxy into http proxy

Usage
-----

```bash
$ docker run --name tor_1 -d -p 9050:9050 -p 9053:9053 sherzberg/tor-proxy
$ docker run --link tor_1:tor_1 -p 8118:8118 -i sherzberg/tor-privoxy
```

You can now connect to the http proxy via port 8118.

License
-------

[See LICENSE](/LICENSE)
