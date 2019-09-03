# Create Invoice



## Request

`POST https://api.zipbooks.com/v2/invoices`

## Response

- **Status:** 201 Created
- **Body:**

```json
{
  "data": {
    "attributes": {
      "accept-credit-cards": "boolean",
      "accept-paypal": "boolean",
      "archived-at": null,
      "created-at": "1986-07-11T11:00:00Z",
      "currency-code": "string",
      "date": "string",
      "days-outstanding": null,
      "due-date": null,
      "external-id": "string",
      "google-drive-id": null,
      "notes": null,
      "number": "string",
      "paid-total": "string",
      "po-number": null,
      "sent-date": null,
      "status": "string",
      "terms": null,
      "title": null,
      "total": "string",
      "updated-at": "1986-07-11T11:00:00Z"
    },
    "id": "753",
    "relationships": {
      "account": {
        "data": {
          "id": "2042",
          "type": "account"
        }
      },
      "contact": {
        "data": {
          "id": "1184",
          "type": "contact"
        }
      },
      "estimate": {
        "data": null
      },
      "line-items": {
        "data": [
          {
            "id": "1661",
            "type": "line-item"
          }
        ]
      },
      "logo-cloud-file": {
        "data": {
          "id": "4822",
          "type": "cloud-file"
        }
      },
      "recurring-profile": {
        "data": null
      }
    },
    "type": "invoice"
  },
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
      "id": "1184",
      "relationships": {
        "account": {
          "data": {
            "id": "2042",
            "type": "account"
          }
        },
        "estimates": {},
        "integration-object": {},
        "invoices": {},
        "payment-bank-accounts": {},
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
        "end-date": null,
        "name": "string",
        "notes": "string",
        "order": null,
        "quantity": "string",
        "rate": "string",
        "start-date": null,
        "taxes": [
          {
            "id": "",
            "name": null,
            "rate": "string"
          }
        ],
        "type": "time-entry",
        "updated-at": "1986-07-11T11:00:00Z"
      },
      "id": "1661",
      "relationships": {
        "chart-account": {
          "data": null
        },
        "line-itemable": {
          "data": {
            "id": "753",
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
        "download-url": null,
        "filename": "string",
        "height": "integer",
        "is-explicit": "boolean",
        "is-uploaded": "boolean",
        "size": null,
        "token": "string",
        "updated-at": "1986-07-11T11:00:00Z",
        "width": "integer"
      },
      "id": "4822",
      "type": "cloud-file"
    }
  ],
  "jsonapi": {
    "version": "string"
  }
}
```

## Example

```bash
curl -X POST \
     
     -H 'accept: application/vnd.api+json' \
     
     -H 'content-type: application/vnd.api+json' \
     
     -H 'authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJjYWxsZXIiOm51bGwsInN1YiI6IjE2NTEiLCJpc3MiOiJodHRwczpcL1wvYXBwLnppcGJvb2tzLmNvbVwvdjJcL2F1dGhcL2xvZ2luIiwiaWF0IjoxNTY3NTMzMzE4LCJleHAiOjE1ODMwODUzMTgsIm5iZiI6MTU2NzUzMzMxOCwianRpIjoiNGY5YzEyZDQtNDMzMS00ZTkwLWE1ZWEtZTJjODQ1M2MyMGRjIiwic3RlYWx0aCI6ImZhbHNlIiwiYWNjb3VudF9pZCI6MjA0MiwidXBkYXRlZF9hdCI6IjIwMTktMDktMDMgMTc6NTU6MThaIn0.cF-uBPyssE14iHElk1wHXCnqtjtQVQ4V31nb9_QJNSc' \
     
     "https://api.zipbooks.com/v2/invoices"
```
