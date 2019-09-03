# Index Invoice



## Request

`GET https://api.zipbooks.com/v2/invoices`

## Response

- **Status:** 200 OK
- **Body:**

```json
{
  "data": [
    {
      "attributes": {
        "accept-credit-cards": "boolean",
        "accept-paypal": "boolean",
        "archived-at": null,
        "created-at": "1986-07-11T11:00:00Z",
        "currency-code": "string",
        "date": "string",
        "days-outstanding": null,
        "due-date": "string",
        "external-id": "string",
        "google-drive-id": "string",
        "notes": "string",
        "number": "string",
        "paid-total": "string",
        "po-number": "string",
        "sent-date": null,
        "status": "string",
        "terms": "string",
        "title": "string",
        "total": "string",
        "updated-at": "1986-07-11T11:00:00Z"
      },
      "id": "666",
      "relationships": {
        "account": {
          "data": {
            "id": "1892",
            "type": "account"
          }
        },
        "contact": {
          "data": {
            "id": "1084",
            "type": "contact"
          }
        },
        "estimate": {
          "data": null
        },
        "line-items": {
          "data": [
            {
              "id": "1500",
              "type": "line-item"
            },
            {
              "id": "1501",
              "type": "line-item"
            }
          ]
        },
        "logo-cloud-file": {
          "data": {
            "id": "4478",
            "type": "cloud-file"
          }
        },
        "recurring-profile": {
          "data": null
        }
      },
      "type": "invoice"
    }
  ],
  "included": [
    {
      "attributes": {
        "address-1": "string",
        "address-2": "string",
        "allow-review-invites": "boolean",
        "archived-at": null,
        "city": "string",
        "country": "string",
        "created-at": "1986-07-11T11:00:00Z",
        "department": "string",
        "display-name": "string",
        "email": "string",
        "expenses": "string",
        "first-name": "string",
        "industry": "string",
        "is-1099-required": "boolean",
        "is-visible": "boolean",
        "last-name": "string",
        "name": "string",
        "notes": "string",
        "phone": "string",
        "postal-code": "string",
        "revenue": "string",
        "state": "string",
        "suggested-next-estimate-number": "string",
        "suggested-next-invoice-number": "string",
        "unbilled-journal-entry-lines": "boolean",
        "unbilled-time-entries": "boolean",
        "updated-at": "1986-07-11T11:00:00Z",
        "website": "string"
      },
      "id": "1084",
      "relationships": {
        "account": {
          "data": {
            "id": "1892",
            "type": "account"
          }
        },
        "estimates": {},
        "integration-object": {},
        "invoices": {},
        "payment-bank-accounts": {
          "data": []
        },
        "people": {},
        "projects": {},
        "public-profile": {},
        "recurring-profiles": {},
        "time-entries": {}
      },
      "type": "contact"
    },
    {
      "attributes": {
        "created-at": "1986-07-11T11:00:00Z",
        "discount": "string",
        "end-date": "string",
        "name": "string",
        "notes": "string",
        "order": "integer",
        "quantity": "string",
        "rate": "string",
        "start-date": "string",
        "taxes": [],
        "type": "Est veniam magni quasi.",
        "updated-at": "1986-07-11T11:00:00Z"
      },
      "id": "1500",
      "relationships": {
        "chart-account": {
          "data": null
        },
        "line-itemable": {
          "data": {
            "id": "666",
            "type": "invoice"
          }
        }
      },
      "type": "line-item"
    },
    {
      "attributes": {
        "created-at": "1986-07-11T11:00:00Z",
        "discount": "string",
        "end-date": "string",
        "name": "string",
        "notes": "string",
        "order": "integer",
        "quantity": "string",
        "rate": "string",
        "start-date": "string",
        "taxes": [],
        "type": "Id.",
        "updated-at": "1986-07-11T11:00:00Z"
      },
      "id": "1501",
      "relationships": {
        "chart-account": {
          "data": null
        },
        "line-itemable": {
          "data": {
            "id": "666",
            "type": "invoice"
          }
        }
      },
      "type": "line-item"
    },
    {
      "attributes": {
        "category": null,
        "content-type": "string",
        "created-at": "1986-07-11T11:00:00Z",
        "download-url": "string",
        "filename": "string",
        "height": "integer",
        "is-explicit": "boolean",
        "is-uploaded": "boolean",
        "size": null,
        "token": "string",
        "updated-at": "1986-07-11T11:00:00Z",
        "width": "integer"
      },
      "id": "4478",
      "type": "cloud-file"
    }
  ],
  "jsonapi": {
    "version": "string"
  },
  "links": {
    "self": "string"
  },
  "meta": {
    "from": "integer",
    "to": "integer",
    "total": "integer",
    "unfiltered-total": "integer"
  }
}
```

## Example

```bash
curl -X GET \
     
     -H 'accept: application/vnd.api+json' \
     
     -H 'content-type: application/vnd.api+json' \
     
     -H 'authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJjYWxsZXIiOm51bGwsInN1YiI6IjE1NjMiLCJpc3MiOiJodHRwczpcL1wvYXBwLnppcGJvb2tzLmNvbVwvdjJcL2F1dGhcL2xvZ2luIiwiaWF0IjoxNTY3NTMzMjk1LCJleHAiOjE1ODMwODUyOTUsIm5iZiI6MTU2NzUzMzI5NSwianRpIjoiNDE3M2NjMzktMmJiMC00YWNhLTllZjYtMTE0ZGM1NDg1ZjVjIiwic3RlYWx0aCI6ImZhbHNlIiwiYWNjb3VudF9pZCI6MTg5MiwidXBkYXRlZF9hdCI6IjIwMTktMDktMDMgMTc6NTQ6NTVaIn0.2iqsLDuUvtP8XSu8VyjrjcR1HrFKHDm91yXtXnm9oQM' \
     
     "https://api.zipbooks.com/v2/invoices"
```
