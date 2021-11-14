# Flashfood API Spec
OpenAPI 3.0 spec for unofficial flashfood API

View this rendered interactive API docs here: https://editor.swagger.io/?url=https://raw.githubusercontent.com/patcon/flashfood-api-docs/main/openapi-3.yaml

This documentation was created using [`apk-mitm`](https://github.com/shroudedcode/apk-mitm) (to unpin the app's certificate and reinstall the modified apk) and [`mitmproxy`](https://mitmproxy.org/) to proxy the traffic from the modified app through your laptop for inspection. (Specific details about using these tools can be found elsewhere on the internet.)

## Getting the access token

```
cp payload.sample.json payload.json
# edit username (email) and password in your file copy
curl -X POST https://identity.flashfood.com/oauth/token -d @payload.json --header "Content-Type: application/json"
```

Note the long `access_token` string in the response (this will likely log you out of your app). You can use this in the top-right of the interactive API docs to explore the API.
