## dorkali
Dorkali a program written in golang to search query in search engines.

## Installing
Install script by:
```bash
GO111MODULE=off go get -u github.com/aWolver/dorkali/cmd/...
```

> Script will install in $GOPATH/bin

Or use git:
```bash
git clone https://github.com/aWolver/dorkali
```
```bash
cd dorkali
```
```bash
go build ./cmd/dorkali/...
```

## Using
Call dorkali to see help message:
```bash
$ dorkali
Dorkali a program written in golang to dorks queries in search engines

Usage:
	./dorkali [list | version [engineName] | help [engineName]]
	./dorkali engineName [OPTIONS]

*Commands:
	version [engineName]   print version, or engine version if pass engineName, and exit
	list                   print list of engines and exit
	help [engineName]      print this help, or print engine help if pass engineName, and exit
```

Then you can use `list` command to see engines:
```bash
$ dorkali list
Registered engines:
  ...
```

You can see help of engine you want with `dorkali help engineName`, here for example `google`:
```bash
$ dorkali help google
```

**Example**
```bash
┌─[awolver]─[~]
└──╼ $ dorkali google -n 2 "my ip"
https://whatismyipaddress.com/learning/ip-addresses
https://www.whatismyip.com/
```


