# Public Accept Estimate

Public endpoint to accept an estimates

## Request

`PATCH https://api.zipbooks.com/v2/public/estimates/2a8f92a0-b090-4cf9-9d72-4724f66f43e5/accept`

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
     
     -H 'authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJjYWxsZXIiOm51bGwsInN1YiI6IjE2MTQiLCJpc3MiOiJodHRwczpcL1wvYXBwLnppcGJvb2tzLmNvbVwvdjJcL2F1dGhcL2xvZ2luIiwiaWF0IjoxNTY3NTM5NjM2LCJleHAiOjE1ODMwOTE2MzYsIm5iZiI6MTU2NzUzOTYzNiwianRpIjoiNzlmNWY0YzMtOGFkYy00NGQyLTgyNDctOTk0MjU5YjBiODdhIiwic3RlYWx0aCI6ImZhbHNlIiwiYWNjb3VudF9pZCI6MjAxMiwidXBkYXRlZF9hdCI6IjIwMTktMDktMDMgMTk6NDA6MzZaIn0.DkLSa-1CkCo7r74-obVGKunJ4YdwcpC1p32SehAygig' \
     
     "https://api.zipbooks.com/v2/public/estimates/2a8f92a0-b090-4cf9-9d72-4724f66f43e5/accept"
```
