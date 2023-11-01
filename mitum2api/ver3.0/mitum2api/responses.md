# Responses

If the request is successful, the response body is sent back in the form of a JSON object.

The JSON object contains hint message of the resource that was the target of the request. \
In addition, the \_embedded field contains specific information.



#### Response for a Single Object

For example, a GET request to '/account/$ACCOUNT\_ADDRESS\` returns an object with the hint message "mitum-currency-account-value".

```json
{
      "_hint": "mitum-currency-hal-v0.0.1",
      "_embedded": {
        "_hint": "mitum-currency-account-value-v0.0.1",
        "hash": "7f5yLXDPJoFuVwRvF2Dw2iCDrKA9xVmMHuqxrgY3hpKb",
        "address": "d7f09d4f066733589da01e06c953ca45af7d6a9feca",
        "keys": {
          "_hint": "mitum-currency-contract-account-keys-v0.0.1",
          "hash": "BGtXqEudPbNqxRWrWvNmrrtPtBcBZMdEjkFwcVgrdFUr",
          "keys": [],
          "threshold": 100
        },
        "balance": [
          {
            "amount": "100",
            "currency": "PEN",
            "_hint": "mitum-currency-amount-v0.0.1"
          }
        ],
        "height": 50194
      }
}
```

