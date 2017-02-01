# Errors

Edvisor.io will respond with a 200 success code even if there are operational errors. This follows the GraphQL specification. All errors will be described in an `errors` array in the response.

```json
#Sample error response

{
  "data": {
    "agencyCompany": null
  },
  "errors": [
    {
      "message": "Unauthenticated",
      "locations": [
        {
          "line": 2,
          "column": 3
        }
      ],
      "path": [
        "agencyCompany"
      ]
    }
  ]
}
```
