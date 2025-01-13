# UpdateMemberMethod

How to pass the update request data. Can be `GET` or `POST` and the default is `POST`. `POST` sends the data as encoded form data and `GET` sends the data as query parameters.

## Example Usage

```typescript
import { UpdateMemberMethod } from "twilio-sdk/models/operations";

let value: UpdateMemberMethod = "GET";
```

## Values

```typescript
"GET" | "POST"
```