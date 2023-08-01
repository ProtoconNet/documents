# HTTP Statuses

Along with the HTTP methods that the API responds to, it will also return standard HTTP statuses, including error codes.

In the event of a problem, the status will contain the error code, while the body of the response will usually contain additional information about the problem that was encountered.

In general, if the status returned is in the 200 range, it indicates that the request was fulfilled successfully and that no error was encountered.

Return codes in the 400 range typically indicate that there was an issue with the request that was sent. For example, it might mean that you didn’t enter a parameter correctly, failed to validate a signature, requested an unauthorized action, the object you're requesting doesn't exist, or the request is invalid.

If you receive a status in the 500 range, this generally indicates a node-side problem. This means that provider are having an issue on our end and cannot fulfill your request currently.

400 and 500 level error responses will include a JSON object in their body, including the message attributes.

#### Example Error Response

```json
// 400 Bad Request
{
    "message":  "handle new operation; fail to preprocess CreateAccountsItem: keys of target already exists"
}
```

