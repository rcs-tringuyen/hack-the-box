```bash
curl -sSik http://10.10.10.56:80/
```

[/root/results/10.10.10.56/scans/tcp80/tcp_80_http_curl.html](file:///root/results/10.10.10.56/scans/tcp80/tcp_80_http_curl.html):

```
HTTP/1.1 200 OK
Date: Mon, 17 Jan 2022 22:02:04 GMT
Server: Apache/2.4.18 (Ubuntu)
Last-Modified: Fri, 22 Sep 2017 20:01:19 GMT
ETag: "89-559ccac257884"
Accept-Ranges: bytes
Content-Length: 137
Vary: Accept-Encoding
Content-Type: text/html

 <!DOCTYPE html>
<html>
<body>

<h2>Don't Bug Me!</h2>
<img src="bug.jpg" alt="bug" style="width:450px;height:350px;">

</body>
</html>


```
