---
layout: default
title: General
parent: Endpoints
nav_order: 1
---

# General
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

### /app/ (GET)

#### Request cURL

```
curl http://localhost:5001/app/
```

#### Response body

```
{"message":"Your API works! (200)"}
```

#### Response headers

```
HTTP/1.1 200 OK
X-Powered-By: Express
Access-Control-Allow-Origin: *
Content-Type: application/json; charset=utf-8
Content-Length: 35
ETag: W/"23-KNmhzXgQhtEE5ovS3fuLixylNK0"
Date: Fri, 29 Apr 2022 01:36:28 GMT
Connection: keep-alive
Keep-Alive: timeout=5
```