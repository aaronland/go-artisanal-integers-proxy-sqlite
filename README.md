# go-artisanal-integers-proxy-sqlite

Go SQLite-backed proxy for artisanal integer services.

## Install

You will need to have both `Go` and the `make` programs installed on your computer. Assuming you do just type:

```
make bin
```

All of this package's dependencies are bundled with the code in the `vendor` directory.

## Tools

### proxy-server

```
./bin/proxy-server -h
Usage of ./bin/proxy-server:
  -brooklyn-integers
	Use Brooklyn Integers as an artisanal integer source.
  -dsn string
       A valid SQLite DSN string. (default ":memory:")
  -host string
    	Host to listen on. (default "localhost")
  -httptest.serve string
    		  if non-empty, httptest.NewServer serves on this address and blocks
  -loglevel string
    	    Log level. (default "info")
  -london-integers
	Use London Integers as an artisanal integer source.
  -min int
       The minimum number of artisanal integers to keep on hand at all times. (default 5)
  -mission-integers
	Use Mission Integers as an artisanal integer source.
  -port int
    	Port to listen on. (default 8080)
  -protocol string
    	    The protocol to use for the proxy server. (default "http")
```

## See also:

* https://github.com/aaronland/go-artisanal-integers-proxy
* https://github.com/aaronland/go-artisanal-integers
* https://github.com/whosonfirst/go-whosonfirst-sqlite
