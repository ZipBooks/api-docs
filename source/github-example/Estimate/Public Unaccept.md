# Public Unaccept Estimate

Public endpoint to un-accept an estimates

## Request

`PATCH https://api.zipbooks.com/v2/public/estimates/8c1ebeb6-dfba-4b50-837b-9a033d334c3e/unaccept`

## Response

- **Status:** 200 OK
- **Body:**

```json
{
  "data": {
    "attributes": {
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
      "status": "string",
      "subtotal": null,
      "terms": "string",
      "title": "string",
      "total": "string"
    },
    "id": "8c1ebeb6-dfba-4b50-837b-9a033d334c3e",
    "relationships": {
      "account": {},
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
     
     -H 'authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJjYWxsZXIiOm51bGwsInN1YiI6IjE2NjMiLCJpc3MiOiJodHRwczpcL1wvYXBwLnppcGJvb2tzLmNvbVwvdjJcL2F1dGhcL2xvZ2luIiwiaWF0IjoxNTY3NTMzMzIwLCJleHAiOjE1ODMwODUzMjAsIm5iZiI6MTU2NzUzMzMyMCwianRpIjoiYjY3ZDM4YzQtYjEzNy00ZDFkLTk4NjMtYzRhNGVmYzYzZGViIiwic3RlYWx0aCI6ImZhbHNlIiwiYWNjb3VudF9pZCI6MjA1MiwidXBkYXRlZF9hdCI6IjIwMTktMDktMDMgMTc6NTU6MjBaIn0.ICsltsu1gRqz8Q7_DUA0GQIWvBtclJcnwNr9Brc5ytU' \
     
     "https://api.zipbooks.com/v2/public/estimates/8c1ebeb6-dfba-4b50-837b-9a033d334c3e/unaccept"
```
