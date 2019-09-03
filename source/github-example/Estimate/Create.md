# Create Estimate



## Request

`POST https://api.zipbooks.com/v2/estimates`

## Response

- **Status:** 201 Created
- **Body:**

```json
{
  "data": {
    "attributes": {
      "archived-at": null,
      "created-at": "datetime",
      "currency-code": "string",
      "date": "string",
      "days-out": "integer",
      "discount": null,
      "external-id": "string",
      "history": [],
      "notes": null,
      "number": "string",
      "po-number": null,
      "sent-date": null,
      "status": null,
      "subtotal": null,
      "terms": null,
      "title": null,
      "total": "string",
      "updated-at": "datetime"
    },
    "id": "105",
    "relationships": {
      "account": {
        "data": {
          "id": "2013",
          "type": "account"
        }
      },
      "contact": {
        "data": {
          "id": "1244",
          "type": "contact"
        }
      },
      "line-items": {
        "data": [
          {
            "id": "1815",
            "type": "line-item"
          }
        ]
      },
      "logo-cloud-file": {
        "data": {
          "id": "4869",
          "type": "cloud-file"
        }
      }
    },
    "type": "estimate"
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
        "created-at": "datetime",
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
        "updated-at": "datetime",
        "website": "string"
      },
      "id": "1244",
      "relationships": {
        "account": {
          "data": {
            "id": "2013",
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
        "created-at": "datetime",
        "discount": null,
        "end-date": null,
        "name": "string",
        "notes": "string",
        "order": null,
        "quantity": "string",
        "rate": "string",
        "start-date": null,
        "taxes": null,
        "type": "time-entry",
        "updated-at": "datetime"
      },
      "id": "1815",
      "relationships": {
        "chart-account": {
          "data": null
        },
        "line-itemable": {
          "data": {
            "id": "105",
            "type": "estimate"
          }
        }
      },
      "type": "line-item"
    },
    {
      "attributes": {
        "category": null,
        "content-type": "string",
        "created-at": "datetime",
        "download-url": null,
        "filename": "string",
        "height": "integer",
        "is-explicit": "boolean",
        "is-uploaded": "boolean",
        "size": null,
        "token": "string",
        "updated-at": "datetime",
        "width": "integer"
      },
      "id": "4869",
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
     
     -H 'authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJjYWxsZXIiOm51bGwsInN1YiI6IjE2MTUiLCJpc3MiOiJodHRwczpcL1wvYXBwLnppcGJvb2tzLmNvbVwvdjJcL2F1dGhcL2xvZ2luIiwiaWF0IjoxNTY3NTM5NjM2LCJleHAiOjE1ODMwOTE2MzYsIm5iZiI6MTU2NzUzOTYzNiwianRpIjoiYjFhYTc4ZTYtODk5Ny00YzBiLThjODgtYzQ3NDRiZjhlYzc4Iiwic3RlYWx0aCI6ImZhbHNlIiwiYWNjb3VudF9pZCI6MjAxMywidXBkYXRlZF9hdCI6IjIwMTktMDktMDMgMTk6NDA6MzZaIn0.PjlBH16jy82MRXkQ90CWZ8SCudotGaB1wfcLxLRGOZE' \
     
     "https://api.zipbooks.com/v2/estimates"
```
