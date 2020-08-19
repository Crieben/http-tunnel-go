# http-tunnel-go
A Cross-Platform HTTP Tunnel written using Go

# Usage
```
  -auth string
    	Proxy Authentication [username:password] (optional)
  -payload string
    	Payload (required)
  -port int
    	Server Port (default 8888)
  -proxy string
    	Proxy Server [host:port] (required)
```

## Example:
Without proxy authentication:

```./http-tunnel-go -proxy 52.77.245.227:8080 -port 8888 -payload "CONNECT [host_port] HTTP/1.0[crlf][crlf]"```

With proxy authentication:

```./http-tunnel-go -proxy 52.77.245.227:8080 -port 8888 -auth leo:leo -payload "CONNECT [host_port] HTTP/1.0[crlf][crlf]"```


## Notes
Version 0.0.2 and above needs base64 encoded payload. So you need to base64 it first before executing.

## License
Non-Profit Open Software License 3.0 (NPOSL-3.0)
