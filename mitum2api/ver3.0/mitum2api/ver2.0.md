# Requests

Any tool that is fluent in HTTP can communicate with the API simply by requesting the correct URI.

Requests should be made using the HTTPS protocol so that traffic is encrypted.

The interface responds to different methods depending on the action required.



<table><thead><tr><th width="132.33333333333331">Methods</th><th>Usage</th></tr></thead><tbody><tr><td>GET</td><td>For simple retrieval of information about your account, block and operation information, or network’s status, you should use the GET method.<br>The information you request will be returned to you as a JSON object.<br>The attributes defined by the JSON object can be used to form additional requests.<br>Any request using the GET method is read-only and will not affect any of the objects you are querying.</td></tr><tr><td>POST</td><td>To create a new account or change the network’s status, your request should specify the POST method.<br>The POST request includes all of the attributes necessary to create a new account or change the network’s status.<br>When you wish to work above, send a POST request to the target endpoint.</td></tr></tbody></table>

Mitum is an immutable blockchain network, so it does not support other methods (e.g. "PATCH", "DELETE") other than "GET" and "POST" methods.

