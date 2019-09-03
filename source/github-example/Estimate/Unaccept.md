# Unaccept Estimate

Un-accepts an estimates

## Request

`PATCH https://api.zipbooks.com/v2/estimates/104/unaccept`

## Response

- **Status:** 200 OK
- **Body:**

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
    "id": "104",
    "relationships": {
      "account": {
        "data": {
          "id": "2012",
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
     
     -H 'authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJjYWxsZXIiOm51bGwsInN1YiI6IjE2MTQiLCJpc3MiOiJodHRwczpcL1wvYXBwLnppcGJvb2tzLmNvbVwvdjJcL2F1dGhcL2xvZ2luIiwiaWF0IjoxNTY3NTM5NjM2LCJleHAiOjE1ODMwOTE2MzYsIm5iZiI6MTU2NzUzOTYzNiwianRpIjoiZWUwY2FlODctOGM3ZC00YjNmLWFkY2QtMWE4MmNlOGFhN2VjIiwic3RlYWx0aCI6ImZhbHNlIiwiYWNjb3VudF9pZCI6MjAxMiwidXBkYXRlZF9hdCI6IjIwMTktMDktMDMgMTk6NDA6MzZaIn0.NfpxtZX5uylBk1BUq73up3gcQHQberGDUyiHDt_W4sE' \
     
     "https://api.zipbooks.com/v2/estimates/104/unaccept"
```
