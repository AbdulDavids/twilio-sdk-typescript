# CreateParticipantWaitMethod

The HTTP method we should use to call `wait_url`. Can be `GET` or `POST` and the default is `POST`. When using a static audio file, this should be `GET` so that we can cache the file.

## Example Usage

```typescript
import { CreateParticipantWaitMethod } from "twilio-sdk/models/operations";

let value: CreateParticipantWaitMethod = "POST";
```

## Values

```typescript
"GET" | "POST"
```