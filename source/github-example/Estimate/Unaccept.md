# Unaccept Estimate

Un-accepts an estimates

## Request

`PATCH https://api.zipbooks.com/v2/estimates/84/unaccept`

## Response

- **Status:** 200 OK
- **Body:**

```json
{
  "data": {
    "attributes": {
      "archived-at": "string",
      "created-at": "1986-07-11T11:00:00Z",
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
      "updated-at": "1986-07-11T11:00:00Z"
    },
    "id": "84",
    "relationships": {
      "account": {
        "data": {
          "id": "2052",
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

## Example

```bash
curl -X PATCH \
     
     -H 'accept: application/vnd.api+json' \
     
     -H 'content-type: application/vnd.api+json' \
     
     -H 'authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJjYWxsZXIiOm51bGwsInN1YiI6IjE2NjMiLCJpc3MiOiJodHRwczpcL1wvYXBwLnppcGJvb2tzLmNvbVwvdjJcL2F1dGhcL2xvZ2luIiwiaWF0IjoxNTY3NTMzMzIxLCJleHAiOjE1ODMwODUzMjEsIm5iZiI6MTU2NzUzMzMyMSwianRpIjoiMzlkMjk5ZDgtMWVhOS00OTQzLThjYWUtOTdiZDNkZDM5MTE5Iiwic3RlYWx0aCI6ImZhbHNlIiwiYWNjb3VudF9pZCI6MjA1MiwidXBkYXRlZF9hdCI6IjIwMTktMDktMDMgMTc6NTU6MjBaIn0.E3AompWkqVj0RUnll_6OvtjoxVq50G_MEUsRe8TCOzQ' \
     
     "https://api.zipbooks.com/v2/estimates/84/unaccept"
```
