# Estimates

## List All Estimates

```shell
curl -X GET \
  https://api.zipbooks.com/v2/estimates \  
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
        "last": "/v2/estimates?page[page]=3&page[page-size]=100",
        "next": "/v2/estimates?page[page]=2&page[page-size]=100",
        "self": "/v2/estimates?page[page]=1&page[page-size]=100"
    },
    "meta": {
        "from": 1,
        "to": 1,
        "total": 250,
        "unfiltered-total": 250
    },
    "data": [
        {
            "attributes": {
                "archived-at": null,
                "created-at": "2018-10-03T15:23:25.000000Z",
                "currency-code": "USD",
                "date": "2017-10-04",
                "days-out": 29,
                "discount": "",
                "external-id": "uEQsw1nO7FNUnNrCjg8BymL4RdAR8Ql0POvseWK8",
                "history": [
                    {
                        "action": "updated",
                        "created_at": "2018-10-09T19:37:42.000000Z"
                    },
                    {
                        "action": "accepted",
                        "created_at": "2017-11-02T00:00:00.000000Z"
                    },
                    {
                        "action": "sent",
                        "created_at": "2017-10-04T00:00:00.000000Z"
                    }
                ],
                "notes": "a note",
                "number": "34",
                "po-number": null,
                "sent-date": "2017-10-04T00:00:00.000000Z",
                "status": "Accepted",
                "subtotal": null,
                "terms": "some terms",
                "title": "Johanna Mann III",
                "total": "108.65",
                "updated-at": "2018-10-09T19:37:42.000000Z"
            },
            "id": "8",
            "relationships": {
                "account": {
                    "data": {
                        "id": "1",
                        "type": "account"
                    }
                },
                "contact": {
                    "data": {
                        "id": "2",
                        "type": "contact"
                    }
                },
                "line-items": {
                    "data": [
                        {
                            "id": "403",
                            "type": "line-item"
                        }
                    ]
                },
                "logo-cloud-file": {
                    "data": {
                        "id": "80",
                        "type": "cloud-file"
                    }
                }
            },
            "type": "estimate"
        },
        ...
    ],
    "included": [
        {
            "attributes": {
                ...
            },
            "id": "2",
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
            "id": "80",
            "type": "cloud-file"
        },
        {
            "attributes": {
                "created-at": "2018-10-03T15:23:25.000000Z",
                "discount": null,
                "end-date": null,
                "name": "Upgradable attitude-oriented task-force",
                "notes": "Similique ut adipisci explicabo dolore. Quae quas voluptates sapiente et amet est ipsam. Ut aut ullam fugiat.",
                "order": 1,
                "quantity": "4.5100",
                "rate": "21.9000",
                "start-date": null,
                "taxes": [
                    {
                        "id": "6",
                        "name": "Sales",
                        "rate": "5"
                    }
                ],
                "type": "time-entry",
                "updated-at": "2018-10-09T19:37:42.000000Z"
            },
            "id": "403",
            "relationships": {
                "chart-account": {
                    "data": null
                },
                "line-itemable": {
                    "data": {
                        "id": "8",
                        "type": "estimate"
                    }
                }
            },
            "type": "line-item"
        }
    ]
}
```

This endpoint retrieves all estimates.

### HTTP Request

`GET https://api.zipbooks.com/v2/estimates`

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
page[page] | 1 | Pagination page number.
page[page-size] | 100 | Pagination page size.
