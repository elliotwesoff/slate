---
title: GuardianPro API V2 Reference

language_tabs: # must be one of https://git.io/vQNgJ
  - json

toc_footers:
  - <a href='https://github.com/slatedocs/slate'>Documentation Powered by Slate</a>

includes:
  - errors

search: true

code_clipboard: true
---

# Introduction

Welcome to the GuardianPro API V2 documentation. Contained within you will find
up-to-date API endpoints used by the Angular front end, HTTP request and response
examples for each.

All examples will assume a host base URL of: `http://guardianpro.com/api/v2`

# Authentication

Free data for all!

# Players

## Search for players

```json
[
    {
        "CustomerID": 1,
        ...
    },
    {
        "CustomerID": 2,
        ...
    }
]
```

### HTTP Request

`POST /players/search`

### URL Parameters

Parameter | Description
--------- | -----------
playerId | The CustomerID of the player
identification | The number on the customer's valid ID card
lastName | The last name of the customer
firstName | The first name of the customer
date | The date of the customer's last transaction


## Get a specific player

```json
{
    "CustomerID": 1
}
```

Returns a player with a matching CustomerID

### HTTP Request

`GET /players/1`
