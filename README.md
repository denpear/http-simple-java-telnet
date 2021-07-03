# http-simple-java-telnet
HTTP протокол: понимать web лучше
telnet httpbin.org 80
Trying 52.201.75.114...
Connected to httpbin.org.
Escape character is '^]'.
GET / HTTP/1.1
Host: httpbin.org


POST /post HTTP/1.1
Host: httpbin.org
Connection: close
Content-type: application/json
Content-length: 14



telnet httpbin.org 80
Trying 54.91.118.50...
Connected to httpbin.org.
Escape character is '^]'.
POST /post HTTP/1.1
Host: httpbin.org
Connection: close
Content-type: application/json
Content-length: 16

{"text":true}

HTTP/1.1 200 OK
Date: Sat, 03 Jul 2021 14:11:05 GMT
Content-Type: application/json
Content-Length: 372
Connection: close
Server: gunicorn/19.9.0
Access-Control-Allow-Origin: *
Access-Control-Allow-Credentials: true

{
  "args": {},
  "data": "{\"text\":true}\r\n\r",
  "files": {},
  "form": {},
  "headers": {
    "Content-Length": "16",
    "Content-Type": "application/json",
    "Host": "httpbin.org",
    "X-Amzn-Trace-Id": "Root=1-60e06feb-7968f36d4e53e47a293cdfbc"
  },
  "json": {
    "text": true
  },
  "origin": "194.186.31.230",
  "url": "http://httpbin.org/post"
}


HTTP протокол: понимать web лучше
