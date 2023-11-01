---
description: /
---

# 1. Get node information

{% swagger method="get" path="/" baseUrl="http://node_IP" summary="Get suffrage-node information of the currently connected Mitum-network." expanded="false" fullWidth="false" %}
{% swagger-description %}
&#x20;The response includes network policy, local node settings, information about the node consensus process, and information about the latest block.
{% endswagger-description %}

{% swagger-response status="200: OK" description="node information" %}

{% endswagger-response %}

{% swagger-response status="500: Internal Server Error" description="" %}

{% endswagger-response %}
{% endswagger %}



#### Response Headers

<table><thead><tr><th width="226">Key</th><th>Value</th></tr></thead><tbody><tr><td>Content-Type</td><td>application/hal+json; charset=utf-8</td></tr><tr><td>Request-Id</td><td>(ex) cj4apiih16elnoamgpng</td></tr><tr><td>X-Mitum-Encoder-Hint</td><td>son-encoder-v2.0.0</td></tr><tr><td>Date</td><td>(ex) Tue, 01 Aug 2023 06:57:14 GMT</td></tr><tr><td>Content-Length</td><td>(ex) 1417</td></tr></tbody></table>



#### Response Examples

{% tabs %}
{% tab title="200" %}
```json
{
    "_hint": "mitum-currency-hal-v0.0.1",
    "_embedded": [
        {
            "consensus": {
                "state": "CONSENSUS",
                "suffrage": {
                    "nodes": [
                        {
                            "publickey": "28diDScgSoStgj2Goket5wC7xTeo2E2w5q2shZiy98yFEmpu",
                            "_hint": "suffrage-node-state-value-v0.0.1",
                            "start": 1,
                            "address": "no0sas"
                        }
                    ],
                    "height": 0
                }
            },
            "_hint": "node-info-v0.0.1",
            "network_id": "bWl0dW0=",
            "last_manifest": {
                "proposal": "9sMie7cmFpDca3291pjFcfApYePxWgBptQ9bhx9RQFsC",
                "operations_tree": null,
                "suffrage": "kUmz18jsu3fPWc3gYdRhnqPKTJj6LbP528e6VqULhft",
                "_hint": "manifest-v0.0.1",
                "height": 694656,
                "states_tree": null,
                "hash": "6QBJd4zxfNdSzPgkKdag2L53TBGYY5oLNnVghABansNU",
                "previous": "ATo8qDkhquGEghzUiMEyLCLhhSEJTv8TV1c4VLdeHbWy",
                "proposed_at": "2023-11-01T04:49:48.682416022Z"
            },
            "network_policy": {
                "max_suffrage_size": 3,
                "suffrage_withdraw_lifespan": 0,
                "suffrage_candidate_limiter": {
                    "_hint": "currency-fixed-suffrage-candidate-limiter-rule-v0.0.1",
                    "limit": 1
                },
                "_hint": "currency-network-policy-v0.0.1",
                "max_operations_in_proposal": 99,
                "suffrage_candidate_lifespan": 333333333
            },
            "local": {
                "address": "no0sas",
                "publickey": "28diDScgSoStgj2Goket5wC7xTeo2E2w5q2shZiy98yFEmpu",
                "parameters": {
                    "interval_broadcast_ballot": "1s",
                    "wait_preparing_init_ballot": "1.5s",
                    "ballot_stuck_wait": "33s",
                    "ballot_stuck_resolve_after": "1m6s",
                    "max_try_handover_y_broker_sync_data": 33,
                    "_hint": "isaac-params-v0.0.1",
                    "threshold": "100.0"
                },
                "conn_info": "127.0.0.1:4320#tls_insecure",
                "uptime": "169798.151",
                "version": "v0.0.1"
            }
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

{% tab title="500" %}
```json
"Internal Server Error"
```
{% endtab %}
{% endtabs %}

