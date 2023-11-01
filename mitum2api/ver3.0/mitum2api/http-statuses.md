# HTTP Statuses

When making requests to the API, you will receive responses that include standard HTTP statuses, including error codes.

If an issue occurs, the response's status code will indicate the specific error, while the response body typically contains additional details about the encountered problem.



In general, a status code in the 200 range signifies that the request was successfully processed without errors.

Status codes in the 400 range usually indicate issues with the request itself. \
For instance, it may signify incorrect parameter entry, signature validation failure, an attempt to perform an unauthorized action, the non-existence of the requested object, or an invalid request.

Status codes in the 500 range generally point to a server-side problem. This means that there is an issue on the provider's end, and the request cannot be fulfilled at the moment.



Responses for errors in the 400 and 500 range will include a JSON object in their response body, which contains attributes with error messages



#### Example of Response for Error

```json
// 400 Bad Request
{
    "message":  "handle new operation; fail to preprocess CreateAccountsItem: keys of target already exists"
}
```

