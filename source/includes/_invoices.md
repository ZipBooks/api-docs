# Invoices

## List All Invoices

```shell
curl -X GET \
  https://api.zipbooks.com/v2/invoices \  
  -H 'Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJjYWxsZXIiOm51bGwsInN1YiI6MSwiaXNzIjoiaHR0cHM6XC9cL2FwcC56aXBib29rcy5jb21cL3YyXC9hdXRoXC9sb2dpbiIsImlhdCI6MTUzOTExMTI1NSwiZXhwIjoxNTU0NjYzMjU1LCJuYmYiOjE1MzkxMTEyNTUsImp0aSI6IjEwNzA2ZDdiLTQzNTMtNDdhNC05NTY1LTMwNDU1ZDQ4NzhlYSIsInN0ZWFsdGgiOiJmYWxzZSIsInVwZGF0ZWRfYXQiOiIyMDE4LTEwLTA5IDE4OjU0OjAwLjAwMDAwMFoifQ.eyTgZ0na9eRSTOQ9RzTukBa9z5QdhIQpz1ztzIHbBGg' \
  -H 'Content-Type: application/json'
```

> Example Response:

```json
{
    "jsonapi": {
        "version": "1.0"
    },
    "links": {
        "last": "/v2/invoices?page[page]=3&page[page-size]=50",
        "next": "/v2/invoices?page[page]=2&page[page-size]=50",
        "self": "/v2/invoices?page[page]=1&page[page-size]=50"
    },
    "meta": {
        "from": 1,
        "to": 50,
        "total": 150,
        "unfiltered-total": 150
    },
    "data": [
        {
            "attributes": {
                "accept-credit-cards": true,
                "accept-paypal": false,
                "archived-at": null,
                "created-at": "2018-10-09T19:23:49.000000Z",
                "currency-code": "USD",
                "date": "2018-10-09",
                "days-outstanding": null,
                "due-date": "2018-11-08",
                "external-id": "26dca2ff-3228-452f-b68e-069dcc4b9243",
                "google-drive-id": null,
                "history": [
                    {
                        "action": "updated",
                        "date": "2018-10-09T19:24:04.000000Z"
                    },
                    {
                        "action": "invoice_created",
                        "date": "2018-10-09T19:23:49.000000Z"
                    }
                ],
                "notes": null,
                "number": "LITTLE-0001",
                "paid-total": "0.00",
                "po-number": null,
                "sent-date": null,
                "status": "Draft",
                "terms": "Net 30",
                "title": null,
                "total": "189.22",
                "updated-at": "2018-10-09T19:24:04.000000Z"
            },
            "id": "187",
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
                            "id": "1350",
                            "type": "line-item"
                        }
                    ]
                },
                "logo-cloud-file": {
                    "data": {
                        "id": "257",
                        "type": "cloud-file"
                    }
                },
                "recurring-profile": {
                    "data": null
                }
            },
            "type": "invoice"
        },
        ...
    ],
    "included": [
        {
            "attributes": {
                ...
            },
            "id": "1",
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
                ...
            },
            "id": "257",
            "type": "cloud-file"
        },
        {
            "attributes": {
                "created-at": "2018-10-09T19:23:49.000000Z",
                "discount": "10.00",
                "end-date": null,
                "name": "Accounting",
                "notes": null,
                "order": 1,
                "quantity": "4.0000",
                "rate": "50.0000",
                "start-date": null,
                "taxes": [
                    {
                        "id": "1",
                        "name": "Sales",
                        "rate": "5.123457"
                    }
                ],
                "type": "time-entry",
                "updated-at": "2018-10-09T19:24:04.000000Z"
            },
            "id": "1350",
            "relationships": {
                "chart-account": {
                    "data": null
                },
                "line-itemable": {
                    "data": {
                        "id": "187",
                        "type": "invoice"
                    }
                }
            },
            "type": "line-item"
        }
    ],
}
```

This endpoint retrieves all invoices.

### HTTP Request

`GET https://api.zipbooks.com/v2/invoices`

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
page[page] | 1 | Pagination page number.
page[page-size] | 50 | Pagination page size.
