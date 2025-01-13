# CreateIncomingPhoneNumberSmsFallbackMethod

The HTTP method that we should use to call `sms_fallback_url`. Can be: `GET` or `POST` and defaults to `POST`.

## Example Usage

```typescript
import { CreateIncomingPhoneNumberSmsFallbackMethod } from "twilio-sdk/models/operations";

let value: CreateIncomingPhoneNumberSmsFallbackMethod = "GET";
```

## Values

```typescript
"GET" | "POST"
```