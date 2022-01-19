```bash
nmap -vv --reason -Pn -T4 -sV -p 80 --script="banner,(http* or ssl*) and not (brute or broadcast or dos or external or http-slowloris* or fuzzer)" -oN "/root/results/10.10.10.56/scans/tcp80/tcp_80_http_nmap.txt" -oX "/root/results/10.10.10.56/scans/tcp80/xml/tcp_80_http_nmap.xml" 10.10.10.56
```

[/root/results/10.10.10.56/scans/tcp80/tcp_80_http_nmap.txt](file:///root/results/10.10.10.56/scans/tcp80/tcp_80_http_nmap.txt):

```
# Nmap 7.92 scan initiated Mon Jan 17 17:01:57 2022 as: nmap -vv --reason -Pn -T4 -sV -p 80 "--script=banner,(http* or ssl*) and not (brute or broadcast or dos or external or http-slowloris* or fuzzer)" -oN /root/results/10.10.10.56/scans/tcp80/tcp_80_http_nmap.txt -oX /root/results/10.10.10.56/scans/tcp80/xml/tcp_80_http_nmap.xml 10.10.10.56
Nmap scan report for 10.10.10.56
Host is up, received user-set (0.080s latency).
Scanned at 2022-01-17 17:01:57 EST for 20s

Bug in http-security-headers: no string output.
PORT   STATE SERVICE REASON         VERSION
80/tcp open  http    syn-ack ttl 63 Apache httpd 2.4.18 ((Ubuntu))
|_http-mobileversion-checker: No mobile version detected.
|_http-wordpress-enum: Nothing found amongst the top 100 resources,use --script-args search-limit=<number|all> for deeper analysis)
|_http-server-header: Apache/2.4.18 (Ubuntu)
|_http-jsonp-detection: Couldn't find any JSONP endpoints.
| http-vhosts: 
|_128 names had status 200
| http-php-version: Logo query returned unknown hash 1694158b3f7adc637066c13aed71a979
|_Credits query returned unknown hash 1694158b3f7adc637066c13aed71a979
|_http-date: Mon, 17 Jan 2022 22:02:13 GMT; +6s from local time.
| http-methods: 
|_  Supported Methods: GET HEAD POST OPTIONS
|_http-stored-xss: Couldn't find any stored XSS vulnerabilities.
|_http-dombased-xss: Couldn't find any DOM based XSS.
|_http-comments-displayer: Couldn't find any comments.
|_http-exif-spider: ERROR: Script execution failed (use -d to debug)
| http-sitemap-generator: 
|   Directory structure:
|     /
|       Other: 1; jpg: 1
|   Longest directory structure:
|     Depth: 0
|     Dir: /
|   Total files found (by extension):
|_    Other: 1; jpg: 1
| http-useragent-tester: 
|   Status for browser useragent: 200
|   Allowed User Agents: 
|     Mozilla/5.0 (compatible; Nmap Scripting Engine; https://nmap.org/book/nse.html)
|     libwww
|     lwp-trivial
|     libcurl-agent/1.0
|     PHP/
|     Python-urllib/2.5
|     GT::WWW
|     Snoopy
|     MFC_Tear_Sample
|     HTTP::Lite
|     PHPCrawl
|     URI::Fetch
|     Zend_Http_Client
|     http client
|     PECL::HTTP
|     Wget/1.13.4 (linux-gnu)
|_    WWW-Mechanize/1.34
|_http-drupal-enum: Nothing found amongst the top 100 resources,use --script-args number=<number|all> for deeper analysis)
|_http-referer-checker: Couldn't find any cross-domain scripts.
|_http-csrf: Couldn't find any CSRF vulnerabilities.
|_http-fetch: Please enter the complete path of the directory to save data in.
| http-headers: 
|   Date: Mon, 17 Jan 2022 22:02:13 GMT
|   Server: Apache/2.4.18 (Ubuntu)
|   Last-Modified: Fri, 22 Sep 2017 20:01:19 GMT
|   ETag: "89-559ccac257884"
|   Accept-Ranges: bytes
|   Content-Length: 137
|   Vary: Accept-Encoding
|   Connection: close
|   Content-Type: text/html
|   
|_  (Request type: HEAD)
|_http-title: Site doesn't have a title (text/html).
|_http-malware-host: Host appears to be clean
|_http-devframework: Couldn't determine the underlying framework or CMS. Try increasing 'httpspider.maxpagecount' value to spider more pages.
|_http-config-backup: ERROR: Script execution failed (use -d to debug)
|_http-wordpress-users: [Error] Wordpress installation was not found. We couldn't find wp-login.php
|_http-litespeed-sourcecode-download: Request with null byte did not work. This web server might not be vulnerable
|_http-chrono: Request times for /; avg: 207.22ms; min: 204.39ms; max: 211.74ms
|_http-errors: Couldn't find any error pages.
|_http-feed: Couldn't find any feeds.

Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Mon Jan 17 17:02:17 2022 -- 1 IP address (1 host up) scanned in 20.11 seconds

```
