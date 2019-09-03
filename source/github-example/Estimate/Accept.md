# Accept Estimate

Accepts an estimates

## Request

`PATCH https://api.zipbooks.com/v2/estimates/104/accept`

## Response

- **Status:** 204 No Content
- **Body:**

```json
""
```

## Example

```bash
curl -X PATCH \
     
     -H 'accept: application/vnd.api+json' \
     
     -H 'content-type: application/vnd.api+json' \
     
     -H 'authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJjYWxsZXIiOm51bGwsInN1YiI6IjE2MTQiLCJpc3MiOiJodHRwczpcL1wvYXBwLnppcGJvb2tzLmNvbVwvdjJcL2F1dGhcL2xvZ2luIiwiaWF0IjoxNTY3NTM5NjM2LCJleHAiOjE1ODMwOTE2MzYsIm5iZiI6MTU2NzUzOTYzNiwianRpIjoiNjM5NmYyNjAtZjc1MS00MThjLWJhY2MtNjRmODQwYzZhYWVmIiwic3RlYWx0aCI6ImZhbHNlIiwiYWNjb3VudF9pZCI6MjAxMiwidXBkYXRlZF9hdCI6IjIwMTktMDktMDMgMTk6NDA6MzZaIn0.D1SKBYvgYDo5zkyri23NzLV4C-RCIVzK6FNx6lLNQZk' \
     
     "https://api.zipbooks.com/v2/estimates/104/accept"
```
