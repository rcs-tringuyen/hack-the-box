```bash
whatweb --color=never --no-errors -a 3 -v http://10.10.10.56:80 2>&1
```

[/root/results/10.10.10.56/scans/tcp80/tcp_80_http_whatweb.txt](file:///root/results/10.10.10.56/scans/tcp80/tcp_80_http_whatweb.txt):

```
WhatWeb report for http://10.10.10.56:80
Status    : 200 OK
Title     : <None>
IP        : 10.10.10.56
Country   : RESERVED, ZZ

Summary   : HTTPServer[Ubuntu Linux][Apache/2.4.18 (Ubuntu)], Apache[2.4.18], HTML5

Detected Plugins:
[ Apache ]
	The Apache HTTP Server Project is an effort to develop and
	maintain an open-source HTTP server for modern operating
	systems including UNIX and Windows NT. The goal of this
	project is to provide a secure, efficient and extensible
	server that provides HTTP services in sync with the current
	HTTP standards.

	Version      : 2.4.18 (from HTTP Server Header)
	Google Dorks: (3)
	Website     : http://httpd.apache.org/

[ HTML5 ]
	HTML version 5, detected by the doctype declaration


[ HTTPServer ]
	HTTP server header string. This plugin also attempts to
	identify the operating system from the server header.

	OS           : Ubuntu Linux
	String       : Apache/2.4.18 (Ubuntu) (from server string)

HTTP Headers:
	HTTP/1.1 200 OK
	Date: Mon, 17 Jan 2022 22:02:05 GMT
	Server: Apache/2.4.18 (Ubuntu)
	Last-Modified: Fri, 22 Sep 2017 20:01:19 GMT
	ETag: "89-559ccac257884-gzip"
	Accept-Ranges: bytes
	Vary: Accept-Encoding
	Content-Encoding: gzip
	Content-Length: 134
	Connection: close
	Content-Type: text/html



```
