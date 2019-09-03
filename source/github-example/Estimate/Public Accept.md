# Public Accept Estimate

Public endpoint to accept an estimates

## Request

`PATCH https://api.zipbooks.com/v2/public/estimates/8c1ebeb6-dfba-4b50-837b-9a033d334c3e/accept`

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
     
     -H 'authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJjYWxsZXIiOm51bGwsInN1YiI6IjE2NjMiLCJpc3MiOiJodHRwczpcL1wvYXBwLnppcGJvb2tzLmNvbVwvdjJcL2F1dGhcL2xvZ2luIiwiaWF0IjoxNTY3NTMzMzIwLCJleHAiOjE1ODMwODUzMjAsIm5iZiI6MTU2NzUzMzMyMCwianRpIjoiYjY3ZDM4YzQtYjEzNy00ZDFkLTk4NjMtYzRhNGVmYzYzZGViIiwic3RlYWx0aCI6ImZhbHNlIiwiYWNjb3VudF9pZCI6MjA1MiwidXBkYXRlZF9hdCI6IjIwMTktMDktMDMgMTc6NTU6MjBaIn0.ICsltsu1gRqz8Q7_DUA0GQIWvBtclJcnwNr9Brc5ytU' \
     
     "https://api.zipbooks.com/v2/public/estimates/8c1ebeb6-dfba-4b50-837b-9a033d334c3e/accept"
```
