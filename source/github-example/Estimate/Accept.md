# Accept Estimate

Accepts an estimates

## Request

`PATCH https://api.zipbooks.com/v2/estimates/84/accept`

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
     
     -H 'authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJjYWxsZXIiOm51bGwsInN1YiI6IjE2NjMiLCJpc3MiOiJodHRwczpcL1wvYXBwLnppcGJvb2tzLmNvbVwvdjJcL2F1dGhcL2xvZ2luIiwiaWF0IjoxNTY3NTMzMzIxLCJleHAiOjE1ODMwODUzMjEsIm5iZiI6MTU2NzUzMzMyMSwianRpIjoiZDY0MDk4MWYtNTIzYy00NTY2LTgwODYtNTZkYTdmYmUyZWEzIiwic3RlYWx0aCI6ImZhbHNlIiwiYWNjb3VudF9pZCI6MjA1MiwidXBkYXRlZF9hdCI6IjIwMTktMDktMDMgMTc6NTU6MjBaIn0.E6gHu42DLw3Gum_uw3GhD93B0QDMwjQS1EAzw_PW3FM' \
     
     "https://api.zipbooks.com/v2/estimates/84/accept"
```
