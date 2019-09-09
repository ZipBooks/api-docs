

## create



```shell
curl -X POST \
  
    -H 'accept: application/vnd.api+json' \
    -H 'content-type: application/vnd.api+json' \
    -H 'authorization: Bearer <token>' \
  "https://api.zipbooks.com/v2/estimates"
```

> Example Response:

```json
{
  "data": {
    "attributes": {
      "archived-at": "date_time|nullable",
      "created-at": "date_time|readonly",
      "currency-code": "currency|nullable",
      "date": "date|nullable",
      "days-out": "integer|nullable",
      "discount": "string|nullable",
      "external-id": "uuid|nullable",
      "history": [],
      "notes": "string|nullable",
      "number": "string|required",
      "po-number": "string|nullable",
      "sent-date": "date|readonly",
      "status": "string|nullable",
      "subtotal": "decimal|nullable",
      "terms": "string|nullable",
      "title": "string|nullable",
      "total": "decimal|nullable",
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
      "line-items": {
        "data": [
          {
            "id": "2990",
            "type": "line-item"
          }
        ]
      },
      "logo-cloud-file": {
        "data": {
          "id": "1",
          "type": "cloud-file"
        }
      }
    },
    "type": "estimate"
  },
  "included": [
    {
      "attributes": {
        "address-1": "09387 Felicity Tunnel",
        "address-2": "Apt. 353",
        "allow-review-invites": true,
        "archived-at": null,
        "city": "Borer",
        "country": "Sao Tome and Principe",
        "created-at": "2019-09-09T17:21:31Z",
        "department": "Voluptas eos impedit cumque et!",
        "display-name": "Casandra Haley",
        "email": "jermain.damore@reichel.org",
        "expenses": "0.00",
        "first-name": "Casandra",
        "industry": "Autem autem!",
        "is-1099-required": true,
        "is-visible": true,
        "last-name": "Haley",
        "name": "Elliot Goyette",
        "notes": "Fuga sit vel!",
        "phone": "(660) 909-9037",
        "postal-code": "23146",
        "revenue": "0.00",
        "state": "GA",
        "suggested-next-estimate-number": "2",
        "suggested-next-invoice-number": "ELLIOT-0001",
        "unbilled-journal-entry-lines": false,
        "unbilled-time-entries": false,
        "updated-at": "2019-09-09T17:21:31Z",
        "website": "http://bosco.name"
      },
      "id": "1831",
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
        "created-at": "2019-09-09T17:21:31Z",
        "discount": null,
        "end-date": null,
        "name": "Cross-platform methodical internetsolution",
        "notes": "notes",
        "order": null,
        "quantity": "1",
        "rate": "22.69",
        "start-date": null,
        "taxes": null,
        "type": "time-entry",
        "updated-at": "2019-09-09T17:21:31Z"
      },
      "id": "2990",
      "relationships": {
        "chart-account": {
          "data": null
        },
        "line-itemable": {
          "data": {
            "id": "1",
            "type": "estimate"
          }
        }
      },
      "type": "line-item"
    },
    {
      "attributes": {
        "category": null,
        "content-type": "image/png",
        "created-at": "2019-09-09T17:21:31Z",
        "download-url": null,
        "filename": "logo.png",
        "height": 0,
        "is-explicit": false,
        "is-uploaded": false,
        "size": null,
        "token": "05d665b3-8c36-48af-92d5-855dc743e61d",
        "updated-at": "2019-09-09T17:21:31Z",
        "width": 0
      },
      "id": "7299",
      "type": "cloud-file"
    }
  ],
  "jsonapi": {
    "version": "1.0"
  }
}
```

### HTTP Request

`POST https://api.zipbooks.com/v2/estimates`


