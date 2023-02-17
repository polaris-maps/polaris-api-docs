---
layout: default
title: User
parent: Endpoints
nav_order: 2
---

# User
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

### /app/user/all (GET)
#### Request cURL
```
curl https://accessnav-api-git-ctine987.apps.cloudapps.unc.edu/app/user/all
```

#### Response body
{% raw %}
```
{{ firstName: John, lastName: Doe, email: test@email.com, favoriteLocations: [], issueInterractions: [], issuesCreated: [] },
{ firstName: John, lastName: Doe, email: test@email.com, favoriteLocations: [], issueInterractions: [], issuesCreated: [] },}
```
{% endraw %}

### /app/user/:id (GET)
#### Request cURL
```
curl https://accessnav-api-git-ctine987.apps.cloudapps.unc.edu/app/user/:id
```

#### Response body
{% raw %}
```
{ firstName: John, lastName: Doe, email: test@email.com, favoriteLocations: [], issueInterractions: [], issuesCreated: [] }
```
{% endraw %}


### /app/user/add (GET)
#### Request cURL
```
curl https://accessnav-api-git-ctine987.apps.cloudapps.unc.edu/app/user/add
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

### /app/user/update/:id (GET)
#### Request cURL

```
curl https://accessnav-api-git-ctine987.apps.cloudapps.unc.edu/app/user/all
```

#### Response body
{% raw %}
```
{200}
```
{% endraw %}


### /app/user/delete/:id (GET)
#### Request cURL

```
curl https://accessnav-api-git-ctine987.apps.cloudapps.unc.edu/app/user/delete/:id
```

#### Response body
{% raw %}
```
{200}
```
{% endraw %}