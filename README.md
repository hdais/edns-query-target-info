# edns-query-target-info

## tl;dr
```
$ dig _acme-challenge.eqt.name @8.8.8.8 +short
"hijacked"
```
```
$ dig _acme-challenge.eqt.name @eqt.hdais.net | grep status
   ... status: NXDOMAIN ...
```
