# Backend integration contract (not yet connected)

Implement a server-side `POST /api/analyze` endpoint that accepts multipart form data with `image`, `symbol`, and `timeframe`. The server should call the documented GPT 5.6 Terra vision endpoint using secrets stored only on the server. Validate model output and return JSON containing `bias`, `confidence`, `entryZone`, `stopLoss`, `takeProfits`, `support`, `resistance`, `trend`, and `indicators`.

Do not enable this endpoint until the provider's actual base URL, auth scheme, model identifier, and image-input format are verified. Never fabricate successful AI results when the provider call fails.
