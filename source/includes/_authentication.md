# Authentication

> To authorize, use this code:

```shell
# With shell, you can just pass the correct header with each request
curl "https://api.edvisor.io/graphql"
  -H "Authorization: Bearer <your_edvisor_api_key>"
```

> Make sure to replace `your_edvisor_api_key` with your API key.

Edvisor.io uses API keys to allow access to the API. To access our API, please contact us at <a href='mailto:support@edvisor.io'>support@edvisor.io</a>.

Edvisor.io expects for the API key to be included in all API requests to the server in a header that looks like the following:

`Authorization: Bearer <your_edvisor_api_key>`

<aside class="notice">
You must replace <code>your_edvisor_api_key</code> with your API key.
</aside>
<aside class="warning">
It is your responsibility to not expose your Edvisor.io API key to the public. All requests to the Edvisor API should be made from your server and not a customer-facing front end.
</aside>