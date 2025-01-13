# DeleteMessageRequest

## Example Usage

```typescript
import { DeleteMessageRequest } from "twilio-sdk/models/operations";

let value: DeleteMessageRequest = {
  accountSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                      | Type                                                                                                       | Required                                                                                                   | Description                                                                                                |
| ---------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                               | *string*                                                                                                   | :heavy_check_mark:                                                                                         | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) associated with the Message resource |
| `sid`                                                                                                      | *string*                                                                                                   | :heavy_check_mark:                                                                                         | The SID of the Message resource you wish to delete                                                         |