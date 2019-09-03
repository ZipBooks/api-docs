

## Create



```shell
curl -X POST \
  
    -H 'accept: application/vnd.api+json' \
  
    -H 'content-type: application/vnd.api+json' \
  
    -H 'authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJjYWxsZXIiOm51bGwsInN1YiI6IjE5MDkiLCJpc3MiOiJodHRwczpcL1wvYXBwLnppcGJvb2tzLmNvbVwvdjJcL2F1dGhcL2xvZ2luIiwiaWF0IjoxNTY3NTQwNjEwLCJleHAiOjE1ODMwOTI2MTAsIm5iZiI6MTU2NzU0MDYxMCwianRpIjoiMTNkNmUyYzYtYTdmZS00YmVhLTljZTktNTA4NzIxMmQ4Njg1Iiwic3RlYWx0aCI6ImZhbHNlIiwiYWNjb3VudF9pZCI6MjcxNiwidXBkYXRlZF9hdCI6IjIwMTktMDktMDMgMTk6NTY6NTBaIn0.ik7lVtWPGeuDYMh8aPSVPqTxYt3F9wUNseK6262_bpg' \
  
  "https://api.zipbooks.com/v2/invoices"
```

> Example Response:

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
      "notes": null,
      "number": "string",
      "paid-total": "string",
      "po-number": null,
      "sent-date": null,
      "status": "string",
      "terms": null,
      "title": null,
      "total": "string",
      "updated-at": "datetime"
    },
    "id": "1250",
    "relationships": {
      "account": {
        "data": {
          "id": "2716",
          "type": "account"
        }
      },
      "contact": {
        "data": {
          "id": "1674",
          "type": "contact"
        }
      },
      "estimate": {
        "data": null
      },
      "line-items": {
        "data": [
          {
            "id": "2565",
            "type": "line-item"
          }
        ]
      },
      "logo-cloud-file": {
        "data": {
          "id": "6347",
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
      "id": "1674",
      "relationships": {
        "account": {
          "data": {
            "id": "2716",
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
        "updated-at": "datetime"
      },
      "id": "2565",
      "relationships": {
        "chart-account": {
          "data": null
        },
        "line-itemable": {
          "data": {
            "id": "1250",
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
      "id": "6347",
      "type": "cloud-file"
    }
  ],
  "jsonapi": {
    "version": "string"
  }
}
```

### HTTP Request

`POST https://api.zipbooks.com/v2/invoices`


