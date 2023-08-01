# Copy of (Methods description)

{% swagger method="get" path="" baseUrl="" summary="https://<provider's base-url>/" expanded="true" fullWidth="false" %}
{% swagger-description %}
node information of mitum-currency node
{% endswagger-description %}

{% swagger-response status="200: OK" description="" %}

{% endswagger-response %}

{% swagger-response status="400: Bad Request" description="" %}

{% endswagger-response %}

{% swagger-response status="403: Forbidden" description="" %}

{% endswagger-response %}

{% swagger-response status="404: Not Found" description="" %}

{% endswagger-response %}

{% swagger-response status="500: Internal Server Error" description="" %}

{% endswagger-response %}
{% endswagger %}



#### Response examples

{% tabs %}
{% tab title="200" %}
```json
{
    "_hint": "mitum-currency-hal-v0.0.1",
    "_embedded": [
        {
            "network_id": "bWl0dW0=",
            "last_manifest": {
                "proposed_at": "2023-08-01T06:53:21.57886608Z",
                "states_tree": null,
                "hash": "HVdhQDf6FK1NHLVj8d85DPuNo1khp1zfVFYswhM49Hza",
                "previous": "ErVzpsDr5Aj2BofmqBhNunsdTmrwfGYp7pwGyQy1KM5n",
                "proposal": "G1tu1dSvwMdbpvKUSR82rrA2cEqjUN5kmnQFA3tjjfQB",
                "operations_tree": null,
                "suffrage": "E2rk7KVFU76YGTddXG3g7rAuWZ89zDMdjMy5UghRsTK9",
                "_hint": "manifest-v0.0.1",
                "height": 258200
            },
            "network_policy": {
                "suffrage_candidate_limiter": {
                    "_hint": "currency-fixed-suffrage-candidate-limiter-rule-v0.0.1",
                    "limit": 1
                },
                "_hint": "currency-network-policy-v0.0.1",
                "max_operations_in_proposal": 99,
                "suffrage_candidate_lifespan": 333333333,
                "max_suffrage_size": 3,
                "suffrage_withdraw_lifespan": 0
            },
            "local": {
                "address": "no0sas",
                "publickey": "zaycqtbVxeR8VnQ7Zdqf3Z3G1imC4YyY9GBGYiEKtKx2mpu",
                "parameters": {
                    "_hint": "isaac-params-v0.0.1",
                    "threshold": "67.0",
                    "interval_broadcast_ballot": "3s",
                    "wait_preparing_init_ballot": "5s",
                    "ballot_stuck_wait": "33s",
                    "ballot_stuck_resolve_after": "1m6s",
                    "max_try_handover_y_broker_sync_data": 33
                },
                "conn_info": "127.0.0.1:4320#tls_insecure",
                "uptime": "1026436.214",
                "version": "v0.0.1"
            },
            "consensus": {
                "state": "CONSENSUS",
                "suffrage": {
                    "nodes": [
                        {
                            "address": "no0sas",
                            "publickey": "zaycqtbVxeR8VnQ7Zdqf3Z3G1imC4YyY9GBGYiEKtKx2mpu",
                            "_hint": "suffrage-node-state-value-v0.0.1",
                            "start": 1
                        }
                    ],
                    "height": 0
                }
            },
            "_hint": "node-info-v0.0.1"
        }
    ],
    "_links": {
        "self": {
            "href": "/"
        }
    }
}
```
{% endtab %}

{% tab title="400" %}
```json
Bad request
```
{% endtab %}

{% tab title="403" %}
```json
```
{% endtab %}

{% tab title="404" %}
```json
// Some code
```
{% endtab %}

{% tab title="500" %}
```json
// Some code
```
{% endtab %}
{% endtabs %}

