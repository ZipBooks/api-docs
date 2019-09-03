# Duplicate Invoice

Duplicates an invoice

## Request

`POST https://api.zipbooks.com/v2/invoices/1203/duplicate`

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
      "created-at": "datetime",
      "currency-code": "string",
      "date": "string",
      "days-outstanding": null,
      "due-date": null,
      "external-id": "string",
      "google-drive-id": null,
      "notes": "string",
      "number": "string",
      "paid-total": "string",
      "po-number": "string",
      "sent-date": null,
      "status": "string",
      "terms": "string",
      "title": "string",
      "total": "string",
      "updated-at": "datetime"
    },
    "id": "1205",
    "relationships": {
      "account": {
        "data": {
          "id": "2640",
          "type": "account"
        }
      },
      "contact": {
        "data": {
          "id": "1631",
          "type": "contact"
        }
      },
      "estimate": {
        "data": null
      },
      "line-items": {
        "data": [
          {
            "id": "2495",
            "type": "line-item"
          },
          {
            "id": "2496",
            "type": "line-item"
          }
        ]
      },
      "logo-cloud-file": {
        "data": {
          "id": "6210",
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
      "id": "1631",
      "relationships": {
        "account": {
          "data": {
            "id": "2640",
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
        "discount": "string",
        "end-date": null,
        "name": "string",
        "notes": "string",
        "order": "integer",
        "quantity": "string",
        "rate": "string",
        "start-date": null,
        "taxes": [],
        "type": "Ipsa iusto nam vero.",
        "updated-at": "datetime"
      },
      "id": "2495",
      "relationships": {
        "chart-account": {
          "data": null
        },
        "line-itemable": {
          "data": {
            "id": "1205",
            "type": "invoice"
          }
        }
      },
      "type": "line-item"
    },
    {
      "attributes": {
        "created-at": "datetime",
        "discount": "string",
        "end-date": null,
        "name": "string",
        "notes": "string",
        "order": "integer",
        "quantity": "string",
        "rate": "string",
        "start-date": null,
        "taxes": [],
        "type": "Ipsum qui sunt.",
        "updated-at": "datetime"
      },
      "id": "2496",
      "relationships": {
        "chart-account": {
          "data": null
        },
        "line-itemable": {
          "data": {
            "id": "1205",
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
      "id": "6210",
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
     
     -H 'authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJjYWxsZXIiOm51bGwsInN1YiI6IjE4OTMiLCJpc3MiOiJodHRwczpcL1wvYXBwLnppcGJvb2tzLmNvbVwvdjJcL2F1dGhcL2xvZ2luIiwiaWF0IjoxNTY3NTQwNjAzLCJleHAiOjE1ODMwOTI2MDMsIm5iZiI6MTU2NzU0MDYwMywianRpIjoiZGIwZDUzYWUtY2JlYi00NWNiLWIxYTgtZWQwNmM1MWMwZjZjIiwic3RlYWx0aCI6ImZhbHNlIiwiYWNjb3VudF9pZCI6MjY0MCwidXBkYXRlZF9hdCI6IjIwMTktMDktMDMgMTk6NTY6NDNaIn0.KohmJxtu0VHvWpkz1CtjB_SBwTvx8yKMqP3SYY6D5uw' \
     
     "https://api.zipbooks.com/v2/invoices/1203/duplicate"
```
