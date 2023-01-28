---
layout: default
title: Issue
parent: Endpoints
nav_order: 4
---

# Issue
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

### /app/issue/all
#### Request cURL

```
    curl http://localhost:5000/app/issue/all
```
#### Response body
{% raw %}
```
       {{ location: String, latitude: Number, longitude: Number, description: String, status: String, datetimeOpen: Number, datetimeClosed: Number, datetimePermanent: Number, votes: Number}, { location: String, latitude: Number, longitude: Number, description: String, status: String, datetimeOpen: Number, datetimeClosed: Number, datetimePermanent: Number, votes: Number}}
```
{% endraw %}
#### Response headers

```
        HTTP/1.1 200 OK
        X-Powered-By: Express
        Content-Type: application/json; charset=utf-8
        Content-Length: 366
        ETag: W/"23-KNmhzXgQhtEE5ovS3fuLixylNK0"
        Date: Thu, 28 Apr 2022 15:07:49 GMT
        Connection: keep-alive
        Keep-Alive: timeout=5
```

### /app/issue/:id
#### Request cURL

```
 curl http://localhost:5000/app/issue/:id
```
#### Response body
{% raw %}

```
 { location: String, latitude: Number, longitude: Number, description: String, status: String, datetimeOpen: Number, datetimeClosed: Number, datetimePermanent: Number, votes: Number}
```
{% endraw %}
#### Response headers

```
    HTTP/1.1 200 OK
    X-Powered-By: Express
    Content-Type: application/json; charset=utf-8
    Content-Length: 183
    ETag: W/"23-KNmhzXgQhtEE5ovS3fuLixylNK0"
    Date: Thu, 28 Apr 2022 15:07:49 GMT
    Connection: keep-alive
    Keep-Alive: timeout=5
```

### /app/issue/add
#### Request cURL

```
curl http://localhost:5000/app/issue/add
```
#### Response body
{% raw %}

```
{(200)}
```
{% endraw %}
#### Response headers

```
HTTP/1.1 200 OK
X-Powered-By: Express
Content-Type: application/json; charset=utf-8
Content-Length: 3
ETag: W/"23-KNmhzXgQhtEE5ovS3fuLixylNK0"
Date: Thu, 28 Apr 2022 15:07:49 GMT
Connection: keep-alive
Keep-Alive: timeout=5
```
### /app/issue/update/:id
#### Request cURL

```
curl http://localhost:5000/app/issue/update:id
```
#### Response body
{% raw %}

```
 {(200)}
```
{% endraw %}
#### Response headers

```
HTTP/1.1 200 OK
X-Powered-By: Express
Content-Type: application/json; charset=utf-8
Content-Length: 3
ETag: W/"23-KNmhzXgQhtEE5ovS3fuLixylNK0"
Date: Thu, 28 Apr 2022 15:07:49 GMT
Connection: keep-alive
Keep-Alive: timeout=5
```
### /app/issue/delete/:id
#### Request cURL

```
curl http://localhost:5000/app/issue/delete:id
```
#### Response body
{% raw %}

```
 {(200)}
```
{% endraw %}
#### Response headers

```
HTTP/1.1 200 OK
X-Powered-By: Express
Content-Type: application/json; charset=utf-8
Content-Length: 3
ETag: W/"23-KNmhzXgQhtEE5ovS3fuLixylNK0"
Date: Thu, 28 Apr 2022 15:07:49 GMT
Connection: keep-alive
Keep-Alive: timeout=5
```