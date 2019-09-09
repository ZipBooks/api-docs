

## duplicate

Duplicates an invoice

```shell
curl -X POST \
  
    -H 'accept: application/vnd.api+json' \
    -H 'content-type: application/vnd.api+json' \
    -H 'authorization: Bearer <token>' \
  "https://api.zipbooks.com/v2/invoices/1229/duplicate"
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
            "id": "2799",
            "type": "line-item"
          },
          {
            "id": "2800",
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
        "address-1": "9620 McClure Club",
        "address-2": "Suite 533",
        "allow-review-invites": true,
        "archived-at": null,
        "city": "Kassulke",
        "country": "Kazakhstan",
        "created-at": "2019-09-09T17:21:01Z",
        "department": "Sed sint.",
        "display-name": "Kareem Schuppe",
        "email": "wilmer2046@grimes.name",
        "expenses": "0.00",
        "first-name": "Kareem",
        "industry": "Quidem ipsam velit!",
        "is-1099-required": true,
        "is-visible": true,
        "last-name": "Schuppe",
        "name": "Mrs. Nigel Nicolas Jr.",
        "notes": "Voluptas!",
        "phone": "(344) 289-5915",
        "postal-code": "43251",
        "revenue": "0.00",
        "state": "HI",
        "suggested-next-estimate-number": "MRSNIG-0001",
        "suggested-next-invoice-number": "test-3",
        "unbilled-journal-entry-lines": false,
        "unbilled-time-entries": false,
        "updated-at": "2019-09-09T17:21:01Z",
        "website": "http://mckenzie.net"
      },
      "id": "1716",
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
        "created-at": "2019-09-09T17:21:02Z",
        "discount": "0.62",
        "end-date": null,
        "name": "Corrupti consequuntur porro.",
        "notes": "Dicta!",
        "order": 5,
        "quantity": "972.4900",
        "rate": "30.4500",
        "start-date": null,
        "taxes": [],
        "type": "Et laudantium delectus.",
        "updated-at": "2019-09-09T17:21:02Z"
      },
      "id": "2799",
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
        "created-at": "2019-09-09T17:21:02Z",
        "discount": "0.68",
        "end-date": null,
        "name": "Beatae itaque voluptatem enim vero.",
        "notes": "Provident ratione.",
        "order": 482,
        "quantity": "984.5000",
        "rate": "924.5400",
        "start-date": null,
        "taxes": [],
        "type": "A praesentium.",
        "updated-at": "2019-09-09T17:21:02Z"
      },
      "id": "2800",
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
        "created-at": "2019-09-09T17:21:02Z",
        "download-url": null,
        "filename": "logo.png",
        "height": 0,
        "is-explicit": false,
        "is-uploaded": false,
        "size": null,
        "token": "6a18ed1f-21ef-4b65-aee6-5caacf7b8232",
        "updated-at": "2019-09-09T17:21:02Z",
        "width": 0
      },
      "id": "6898",
      "type": "cloud-file"
    }
  ],
  "jsonapi": {
    "version": "1.0"
  }
}
```

### HTTP Request

`POST https://api.zipbooks.com/v2/invoices/1229/duplicate`


