Script to check validity and expiration of SSL certificate on HTTPS site

```
user@host:~$ ./https_ssl_cert_check.sh valid valid.example.com 443
1
user@host:~$ ./https_ssl_cert_check.sh valid invalid.duckdns.org 443
0
user@host:~$ ./https_ssl_cert_check.sh valid expired.example.com 443
0
user@host:~$ ./https_ssl_cert_check.sh expire effective-next-90-days.example.com 443
90
user@host:~$ ./https_ssl_cert_check.sh expire expired.example.com 443
-37
```
