# DeleteCallRequest

## Example Usage

```typescript
import { DeleteCallRequest } from "twilio-sdk/models/operations";

let value: DeleteCallRequest = {
  accountSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                              | Type                                                                                                               | Required                                                                                                           | Description                                                                                                        |
| ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------ |
| `accountSid`                                                                                                       | *string*                                                                                                           | :heavy_check_mark:                                                                                                 | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the Call resource(s) to delete. |
| `sid`                                                                                                              | *string*                                                                                                           | :heavy_check_mark:                                                                                                 | The Twilio-provided Call SID that uniquely identifies the Call resource to delete                                  |