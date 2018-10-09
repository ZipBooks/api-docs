# Contacts

## List All Contacts

```shell
curl -X GET \
  https://api.zipbooks.com/v2/contacts \  
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
        "last": "/v2/contacts?page[page]=2&page[page-size]=100",
        "next": "/v2/contacts?page[page]=2&page[page-size]=100",
        "self": "/v2/contacts?page[page]=1&page[page-size]=100"
    },
    "meta": {
        "from": 1,
        "to": 1,
        "total": 120,
        "unfiltered-total": 120
    },
    "data": [
        {
            "attributes": {
                "address-1": "4383 Torphy Mountains",
                "address-2": null,
                "archived-at": null,
                "city": "Jonesville",
                "country": "PL",
                "created-at": "2018-10-03T15:23:21.000000Z",
                "department": null,
                "email": "dickens.sarina@example.net",
                "expenses": "4668.95",
                "external-source": null,
                "first-name": "Mercedes",
                "industry": null,
                "is-1099-required": false,
                "last-name": "Greenholt",
                "name": "Little-Dibbert",
                "notes": null,
                "phone": "+1-285-877-7471",
                "postal-code": "95027-8264",
                "revenue": "28198.30",
                "state": "MN",
                "suggested-next-estimate-number": "36",
                "suggested-next-invoice-number": "LITTLE-0002",
                "unbilled-journal-entry-lines": true,
                "unbilled-time-entries": false,
                "updated-at": "2018-10-08T22:52:49.000000Z",
                "website": "miller.info"
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
                "integration-object": {
                    "data": null
                },
                "invoices": {},
                "people": {},
                "projects": {},
                "public-profile": {
                    "data": {
                        "id": "ZGlja2Vucy5zYXJpbmFAZXhhbXBsZS5uZXQ",
                        "type": "public-profile"
                    }
                },
                "recurring-profiles": {},
                "time-entries": {}
            },
            "type": "contact"
        },
        ...
    ],
    "included": [
        {
            "attributes": {
                ...
            },
            "id": "ZGlja2Vucy5zYXJpbmFAZXhhbXBsZS5uZXQ",
            "type": "public-profile"
        }
    ]
}
```

This endpoint retrieves all contacts.

### HTTP Request

`GET https://api.zipbooks.com/v2/contacts`

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
page[page] | 1 | Pagination page number.
page[page-size] | 100 | Pagination page size.
