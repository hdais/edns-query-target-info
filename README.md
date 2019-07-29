# edns-query-target-info
enables “name-based” virtual hosting for DNS authoritative server

## tl;dr
```
$ dig _acme-challenge.algorithm13.net TXT @8.8.8.8 +short
"hijacked"
```
```
$ dig _acme-challenge.algorithm13.net TXT @res-eqt.hdais.net | grep status
... status: NXDOMAIN ...
```

## Implementation
### Authoritative server
[eqt-server](https://github.com/hdais/eqt-server)
### Full service resolver
[Unbound forked branch "edns-query-target"](https://github.com/hdais/unbound/tree/edns-query-target)

`git clone -b edns-query-target https://github.com/hdais/unbound/`
