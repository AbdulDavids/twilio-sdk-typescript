# UpdateCallStatusCallbackMethod

The HTTP method we should use when requesting the `status_callback` URL. Can be: `GET` or `POST` and the default is `POST`. If an `application_sid` parameter is present, this parameter is ignored.

## Example Usage

```typescript
import { UpdateCallStatusCallbackMethod } from "twilio-sdk/models/operations";

let value: UpdateCallStatusCallbackMethod = "GET";
```

## Values

```typescript
"GET" | "POST"
```