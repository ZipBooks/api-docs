# Authentication

> To authorize, use this code:

```shell
curl -X POST \
  https://api.zipbooks.com/v2/auth/login \
  -H 'Content-Type: application/json' \
  -d '{
	"email": "test@example.com",
	"password": "password"
}'
```

> Example Response:

```json
{
    "tokens": [
        {
            "user_id": 1,
            "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJjYWxsZXIiOm51bGwsInN1YiI6MSwiaXNzIjoiaHR0cHM6XC9cL2FwcC56aXBib29rcy5jb21cL3YyXC9hdXRoXC9sb2dpbiIsImlhdCI6MTUzOTExMTI1NSwiZXhwIjoxNTU0NjYzMjU1LCJuYmYiOjE1MzkxMTEyNTUsImp0aSI6IjEwNzA2ZDdiLTQzNTMtNDdhNC05NTY1LTMwNDU1ZDQ4NzhlYSIsInN0ZWFsdGgiOiJmYWxzZSIsInVwZGF0ZWRfYXQiOiIyMDE4LTEwLTA5IDE4OjU0OjAwLjAwMDAwMFoifQ.eyTgZ0na9eRSTOQ9RzTukBa9z5QdhIQpz1ztzIHbBGg",
            "account_name": "ZipBooks"
        }
    ]
}
```

The ZipBooks API uses JSON web tokens (JWT) for authentication. When you "log in" a user, you will be sent back a three-part, period-delimited string called "token" (see example response).

You must send this token with all subsequent API requests.
