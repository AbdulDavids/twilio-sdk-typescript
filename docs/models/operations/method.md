# Method

The HTTP method we should use when calling the `url` parameter's value. Can be: `GET` or `POST` and the default is `POST`. If an `application_sid` parameter is present, this parameter is ignored.

## Example Usage

```typescript
import { Method } from "twilio-sdk/models/operations";

let value: Method = "GET";
```

## Values

```typescript
"GET" | "POST"
```