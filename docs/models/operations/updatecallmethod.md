# UpdateCallMethod

The HTTP method we should use when calling the `url`. Can be: `GET` or `POST` and the default is `POST`. If an `application_sid` parameter is present, this parameter is ignored.

## Example Usage

```typescript
import { UpdateCallMethod } from "twilio-sdk/models/operations";

let value: UpdateCallMethod = "POST";
```

## Values

```typescript
"GET" | "POST"
```