# flashfood-api-docs
OpenAPI 3.0 spec for unofficial flashfood API

View this rendered API spec here: https://editor.swagger.io/?url=https://raw.githubusercontent.com/patcon/flashfood-api-docs/main/openapi-3.yaml

To use the API (and interactive docs), you'll need to retrieve the Bearer token from app traffic. You can do this with [`apk-mitm`](https://github.com/shroudedcode/apk-mitm) (to unpin the app's certificate and reinstall the modified apk) and [`mitmproxy`](https://mitmproxy.org/) to proxy the traffic from the modified app through your laptop for inspection. (Specific details about using these tools can be found elsewhere on the internet.)
