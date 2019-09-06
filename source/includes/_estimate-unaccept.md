

## unaccept

Un-accepts an estimates

```shell
curl -X PATCH \
  
    -H 'accept: application/vnd.api+json' \
    -H 'content-type: application/vnd.api+json' \
    -H 'authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJjYWxsZXIiOm51bGwsInN1YiI6IjEwMzEiLCJpc3MiOiJodHRwczpcL1wvYXBwLnppcGJvb2tzLmNvbVwvdjJcL2F1dGhcL2xvZ2luIiwiaWF0IjoxNTY3ODEwODQ1LCJleHAiOjE1ODMzNjI4NDUsIm5iZiI6MTU2NzgxMDg0NSwianRpIjoiMDY1NGEzNzUtMzhlZi00YzgxLWIzNWUtM2FlMTE0M2Q0MzY5Iiwic3RlYWx0aCI6ImZhbHNlIiwiYWNjb3VudF9pZCI6MTIzMSwidXBkYXRlZF9hdCI6IjIwMTktMDktMDYgMjM6MDA6NDVaIn0.add-Zh--rSW8tQeGtB1-bEnOLcrWsHMGGYf01JDpL6g' \
  "https://api.zipbooks.com/v2/estimates/41/unaccept"
```

> Example Response:

```json
{
  "data": {
    "attributes": {
      "archived-at": "string",
      "created-at": "datetime",
      "currency-code": "string",
      "date": "string",
      "days-out": "integer",
      "discount": "string",
      "external-id": "string",
      "history": [
        {
          "action": "string",
          "created_at": "string"
        },
        {
          "action": "string",
          "created_at": "string"
        },
        {
          "action": "string",
          "created_at": "string"
        }
      ],
      "notes": "string",
      "number": "string",
      "po-number": "string",
      "sent-date": "string",
      "status": "string",
      "subtotal": null,
      "terms": "string",
      "title": "string",
      "total": "string",
      "updated-at": "datetime"
    },
    "id": "41",
    "relationships": {
      "account": {
        "data": {
          "id": "1231",
          "type": "account"
        }
      },
      "contact": {},
      "line-items": {},
      "logo-cloud-file": {}
    },
    "type": "estimate"
  },
  "jsonapi": {
    "version": "string"
  }
}
```

### HTTP Request

`PATCH https://api.zipbooks.com/v2/estimates/41/unaccept`


