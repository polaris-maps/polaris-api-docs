---
layout: default
title: Indoor Issue
parent: Endpoints
nav_order: 4
---

# Indoor Issue
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

### /app/indoorIssue/all
#### Request cURL
```
curl https://accessnav-api-git-ctine987.apps.cloudapps.unc.edu/app/indoorindoorIssue/all
```

#### Response body
{% raw %}
```
[
    {
        "_id": "6242966907941f5e76b34770",
        "location": "Rosenau Hall",
        "latitude": 35.905877677908045,
        "longitude": -79.05360645370045,
        "description": "Automatic door broken",
        "status": "Closed",
        "datetimeOpen": 1634359400378,
        "datetimeClosed": 1635309497378,
        "datetimePermanent": 0,
        "votes": [
            "31"
        ],
        "__v": 0
    },
    {
        "_id": "6242989036c1d86631672ab2",
        "location": "Peabody Hall",
        "latitude": 35.91062629670515,
        "longitude": -79.05362209913692,
        "description": "Elevator maintenance",
        "status": "Closed",
        "datetimeOpen": 1644359400378,
        "datetimeClosed": 1645309497378,
        "datetimePermanent": 0,
        "votes": [
            "32"
        ],
        "__v": 0
    }
]
```
{% endraw %}


### /app/indoorIssue/:id
#### Request cURL

```
curl https://accessnav-api-git-ctine987.apps.cloudapps.unc.edu/app/indoorIssue/:id
```

#### Response body
{% raw %}
```
{
    "_id": "6242989036c1d86631672ab2",
    "location": "Peabody Hall",
    "latitude": 35.91062629670515,
    "longitude": -79.05362209913692,
    "description": "Elevator maintenance",
    "status": "Closed",
    "datetimeOpen": 1644359400378,
    "datetimeClosed": 1645309497378,
    "datetimePermanent": 0,
    "votes": [
        "32"
    ],
    "__v": 0
}
```
{% endraw %}


### /app/indoorIssue/add
#### Request cURL
```
curl -X POST 'https://accessnav-api-git-ctine987.apps.cloudapps.unc.edu/app/indoorIssue/add' -H "Content-type: application/json" -d '{
  "location": "Test Hall",
  "category": "Test",
  "description": "Test indoorIssue",
  "status": "Open",
  "datetimeOpen": 1658532213016,
  "datetimeClosed": 0,
  "datetimePermanent": 0,
  "votes": 1
}'
```

#### Response body
{% raw %}
```
{
    "location": "Test Hall",
    "category": "Test",
    "description": "Test indoorIssue",
    "status": "Open",
    "datetimeOpen": 1658532213016,
    "datetimeClosed": 0,
    "datetimePermanent": 0,
    "votes": [
        "1"
    ],
    "_id": "63e948b91f0bdf63525ca500",
    "__v": 0
}
```
{% endraw %}


### /app/indoorIssue/update/:id
#### Request cURL
```
curl https://accessnav-api-git-ctine987.apps.cloudapps.unc.edu/app/indoorIssue/update:id
```

#### Response body
{% raw %}
```
 {(200)}
```
{% endraw %}


### /app/indoorIssue/delete/:id
#### Request cURL
```
curl https://accessnav-api-git-ctine987.apps.cloudapps.unc.edu/app/indoorIssue/delete:id
```

#### Response body
{% raw %}
```
 {(200)}
```
{% endraw %}