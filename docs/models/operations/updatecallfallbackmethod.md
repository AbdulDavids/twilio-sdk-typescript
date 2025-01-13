# UpdateCallFallbackMethod

The HTTP method that we should use to request the `fallback_url`. Can be: `GET` or `POST` and the default is `POST`. If an `application_sid` parameter is present, this parameter is ignored.

## Example Usage

```typescript
import { UpdateCallFallbackMethod } from "twilio-sdk/models/operations";

let value: UpdateCallFallbackMethod = "POST";
```

## Values

```typescript
"GET" | "POST"
```