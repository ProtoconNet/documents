# Links

The `_links` object:

1. is returned as part of the response body.
2. provides a way to get additional information.
3. can contain various fields as requested.



#### Sample Links Object

```
{
    "_links": {
        "operations": {
            "href": "/account/d7f09d4f066733589da01e06c953ca45af7d6a9feca/operations"
        },
        "operations:{offset}": {
            "templated": true,
            "href": "/account/d7f09d4f066733589da01e06c953ca45af7d6a9feca/operations?offset={offset}"
        },
        "operations:{offset,reverse}": {
            "templated": true,
            "href": "/account/d7f09d4f066733589da01e06c953ca45af7d6a9feca/operations?offset={offset}&reverse=1"
        },
        "block": {
          "href": "/block/50194"
        },
        "self": {
          "href": "/account/d7f09d4f066733589da01e06c953ca45af7d6a9feca"
        }
    }
}
```

