
# invoice


## List



```shell
curl -X GET \
  
    -H 'accept: application/vnd.api+json' \
    -H 'content-type: application/vnd.api+json' \
    -H 'authorization: Bearer <token>' \
  "https://api.zipbooks.com/v2/invoices"
```

> Example Response:

```json
{
  "data": [
    {
      "attributes": {
        "accept-credit-cards": true,
        "accept-paypal": true,
        "archived-at": null,
        "created-at": "2019-09-09T17:21:02Z",
        "currency-code": "USD",
        "date": "2017-04-04",
        "days-outstanding": null,
        "due-date": "2017-02-28",
        "external-id": "f98aed8a-6d89-44ee-9126-15889fe610e9",
        "google-drive-id": "Debitis?",
        "notes": "Incidunt repudiandae ratione est?",
        "number": "Est qui ad dolores reiciendis?",
        "paid-total": "0.00",
        "po-number": "Et explicabo placeat aut optio.",
        "sent-date": null,
        "status": "Draft",
        "terms": "Earum esse possimus voluptate?",
        "title": "Consequuntur.",
        "total": "221150.32",
        "updated-at": "2019-09-09T17:21:02Z"
      },
      "id": "1232",
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
              "id": "2804",
              "type": "line-item"
            },
            {
              "id": "2803",
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
    }
  ],
  "included": [
    {
      "attributes": {
        "address-1": "74854 Roma River",
        "address-2": "Apt. 041",
        "allow-review-invites": true,
        "archived-at": null,
        "city": "Lake Cayla",
        "country": "Jamaica",
        "created-at": "2019-09-09T17:21:02Z",
        "department": "Voluptas sunt.",
        "display-name": "Victoria Connelly",
        "email": "keshaun2022@cronin.com",
        "expenses": "0.00",
        "first-name": "Victoria",
        "industry": "Unde.",
        "is-1099-required": true,
        "is-visible": false,
        "last-name": "Connelly",
        "name": "Lenna Gottlieb",
        "notes": "Molestiae consequatur.",
        "phone": "947/313-5830",
        "postal-code": "04671",
        "revenue": "0.00",
        "state": "KY",
        "suggested-next-estimate-number": "LENNAG-0001",
        "suggested-next-invoice-number": "Est qui ad dolores reiciendis?",
        "unbilled-journal-entry-lines": false,
        "unbilled-time-entries": false,
        "updated-at": "2019-09-09T17:21:02Z",
        "website": "http://beahan.biz"
      },
      "id": "1717",
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
        "created-at": "2019-09-09T17:21:02Z",
        "discount": "0.94",
        "end-date": "2017-06-07",
        "name": "Dolorum praesentium perspiciatis officiis!",
        "notes": "Voluptate!",
        "order": 930,
        "quantity": "472.8900",
        "rate": "173.4100",
        "start-date": "2017-07-05",
        "taxes": [],
        "type": "Deleniti magni quidem dignissimos?",
        "updated-at": "2019-09-09T17:21:02Z"
      },
      "id": "2803",
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
        "discount": "0.08",
        "end-date": "2017-05-30",
        "name": "Corporis illo!",
        "notes": "Incidunt id amet quos et!",
        "order": 34,
        "quantity": "425.7000",
        "rate": "328.9500",
        "start-date": "2017-07-16",
        "taxes": [],
        "type": "Beatae omnis sed dolor!",
        "updated-at": "2019-09-09T17:21:02Z"
      },
      "id": "2804",
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
        "download-url": "http://somefakeurl.com/that/will-be-inherited",
        "filename": "logo.png",
        "height": 0,
        "is-explicit": false,
        "is-uploaded": false,
        "size": null,
        "token": "3f827631-7974-4ad9-a743-9a62f6476d0e",
        "updated-at": "2019-09-09T17:21:02Z",
        "width": 0
      },
      "id": "6906",
      "type": "cloud-file"
    }
  ],
  "jsonapi": {
    "version": "1.0"
  },
  "links": {
    "self": "v2/invoices?page[page]=1&page[page-size]=50"
  },
  "meta": {
    "from": 1,
    "to": 1,
    "total": 1,
    "unfiltered-total": 1
  }
}
```

### HTTP Request

`GET https://api.zipbooks.com/v2/invoices`


### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
page[page] | 1 | Pagination page number.
page[page-size] | 50 | Pagination page size.

