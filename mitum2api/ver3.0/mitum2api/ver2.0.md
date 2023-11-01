# Requests

Any HTTP-compliant tool can easily interact with the API by sending requests to the appropriate URI. \
\
For security, it's important to use the HTTPS protocol to ensure that the traffic is encrypted. \
\
The API interface responds to various methods based on the specific action needed.



<table><thead><tr><th width="132.33333333333331">Methods</th><th>Usage</th></tr></thead><tbody><tr><td>GET</td><td>For straightforward retrieval of account, block, and operation information or network status, consider utilizing the GET method. The requested information will be returned in the form of a JSON object. Attributes specified in the JSON object can then be utilized to create further requests. Any request made using the GET method is of a read-only nature and will not impact the queried objects.</td></tr><tr><td>POST</td><td>For the creation of a new account or modification of the network's status, utilize the POST method in your request. The POST request should contain all the required attributes for creating a new account or altering the network's status. To perform these actions, submit a POST request to the designated endpoint</td></tr></tbody></table>



Mitum operates as an immutable blockchain network, exclusively supporting the 'GET' and 'POST' methods, and it does not accommodate other methods like 'PATCH' or 'DELETE'

