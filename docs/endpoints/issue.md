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