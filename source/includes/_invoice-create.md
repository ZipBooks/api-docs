

## create



```shell
curl -X POST \
  
    -H 'accept: application/vnd.api+json' \
    -H 'content-type: application/vnd.api+json' \
    -H 'authorization: Bearer <token>' \
  "https://api.zipbooks.com/v2/invoices"
```

> Example Response:

```json
{
  "data": {
    "attributes": {
      "accept-credit-cards": "boolean|nullable",
      "accept-paypal": "boolean|nullable",
      "archived-at": "date_time|readonly",
      "created-at": "date_time|readonly",
      "currency-code": "currency|nullable",
      "date": "date",
      "days-outstanding": "integer|nullable",
      "due-date": "date|nullable",
      "external-id": "uuid|readonly",
      "google-drive-id": "string|nullable",
      "notes": "string|nullable",
      "number": "string|required",
      "paid-total": "string",
      "po-number": "string|nullable",
      "sent-date": "date|readonly",
      "status": "string",
      "terms": "string|nullable",
      "title": "string|nullable",
      "total": "string",
      "updated-at": "date_time|readonly"
    },
    "id": "1",
    "relationships": {
      "account": {
        "data": {
          "id": "1",
          "type": "account"
        }
      },
      "contact": {
        "data": {
          "id": "1",
          "type": "contact"
        }
      },
      "estimate": {
        "data": null
      },
      "line-items": {
        "data": [
          {
            "id": "2964",
            "type": "line-item"
          }
        ]
      },
      "logo-cloud-file": {
        "data": {
          "id": "1",
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
        "address-1": "58 Karolann Vista",
        "address-2": "Suite 518",
        "allow-review-invites": true,
        "archived-at": null,
        "city": "Wyman",
        "country": "Angola",
        "created-at": "2019-09-09T17:21:25Z",
        "department": "Vero totam.",
        "display-name": "Giuseppe Watsica",
        "email": "colin2090@hickle.org",
        "expenses": "0.00",
        "first-name": "Giuseppe",
        "industry": "Fugiat atque labore.",
        "is-1099-required": false,
        "is-visible": false,
        "last-name": "Watsica",
        "name": "Otilia Gleason",
        "notes": "Quis aut laudantium rerum?",
        "phone": "717/545-4637",
        "postal-code": "80477",
        "revenue": "0.00",
        "state": "FL",
        "suggested-next-estimate-number": "OTILIA-0001",
        "suggested-next-invoice-number": "2",
        "unbilled-journal-entry-lines": false,
        "unbilled-time-entries": false,
        "updated-at": "2019-09-09T17:21:25Z",
        "website": "http://durgan.org"
      },
      "id": "1817",
      "relationships": {
        "account": {
          "data": {
            "id": "1",
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
        "created-at": "2019-09-09T17:21:25Z",
        "discount": "5",
        "end-date": null,
        "name": "Cross-platform methodical internetsolution",
        "notes": "notes",
        "order": null,
        "quantity": "1",
        "rate": "100",
        "start-date": null,
        "taxes": [
          {
            "id": "",
            "name": null,
            "rate": "5"
          }
        ],
        "type": "time-entry",
        "updated-at": "2019-09-09T17:21:25Z"
      },
      "id": "2964",
      "relationships": {
        "chart-account": {
          "data": null
        },
        "line-itemable": {
          "data": {
            "id": "1",
            "type": "invoice"
          }
        }
      },
      "type": "line-item"
    },
    {
      "attributes": {
        "category": null,
        "content-type": "image/png",
        "created-at": "2019-09-09T17:21:25Z",
        "download-url": null,
        "filename": "logo.png",
        "height": 0,
        "is-explicit": false,
        "is-uploaded": false,
        "size": null,
        "token": "4a23b9e8-69f7-421f-93f3-4fe3605fd7f0",
        "updated-at": "2019-09-09T17:21:25Z",
        "width": 0
      },
      "id": "7250",
      "type": "cloud-file"
    }
  ],
  "jsonapi": {
    "version": "1.0"
  }
}
```

### HTTP Request

`POST https://api.zipbooks.com/v2/invoices`


