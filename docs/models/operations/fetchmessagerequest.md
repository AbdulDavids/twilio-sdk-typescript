# FetchMessageRequest

## Example Usage

```typescript
import { FetchMessageRequest } from "twilio-sdk/models/operations";

let value: FetchMessageRequest = {
  accountSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                      | Type                                                                                                       | Required                                                                                                   | Description                                                                                                |
| ---------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                               | *string*                                                                                                   | :heavy_check_mark:                                                                                         | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) associated with the Message resource |
| `sid`                                                                                                      | *string*                                                                                                   | :heavy_check_mark:                                                                                         | The SID of the Message resource to be fetched                                                              |