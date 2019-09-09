

## public_unaccept

Public endpoint to un-accept an estimates

```shell
curl -X PATCH \
  
    -H 'accept: application/vnd.api+json' \
    -H 'content-type: application/vnd.api+json' \
    -H 'authorization: Bearer <token>' \
  "https://api.zipbooks.com/v2/public/estimates/891ae61a-0765-4aba-840e-eaa688d8745c/unaccept"
```

> Example Response:

```json
{
  "data": {
    "attributes": {
      "currency-code": "currency|nullable",
      "date": "date|nullable",
      "days-out": "integer|nullable",
      "discount": "string|nullable",
      "external-id": "uuid|nullable",
      "history": [
        {
          "action": "unaccepted",
          "created_at": "2019-09-09T17:21:28Z"
        },
        {
          "action": "accepted",
          "created_at": "2019-09-09T17:21:28Z"
        },
        {
          "action": "unaccepted",
          "created_at": "2019-09-09T17:21:28Z"
        },
        {
          "action": "sent",
          "created_at": "2019-09-09T17:21:28Z"
        },
        {
          "action": "accepted",
          "created_at": "2019-09-09T17:21:28Z"
        }
      ],
      "notes": "string|nullable",
      "number": "string|required",
      "po-number": "string|nullable",
      "status": "string|nullable",
      "subtotal": "decimal|nullable",
      "terms": "string|nullable",
      "title": "string|nullable",
      "total": "decimal|nullable"
    },
    "id": "1",
    "relationships": {
      "account": {},
      "contact": {},
      "line-items": {},
      "logo-cloud-file": {}
    },
    "type": "estimate"
  },
  "jsonapi": {
    "version": "1.0"
  }
}
```

### HTTP Request

`PATCH https://api.zipbooks.com/v2/public/estimates/891ae61a-0765-4aba-840e-eaa688d8745c/unaccept`


