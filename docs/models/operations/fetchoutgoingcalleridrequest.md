# FetchOutgoingCallerIdRequest

## Example Usage

```typescript
import { FetchOutgoingCallerIdRequest } from "twilio-sdk/models/operations";

let value: FetchOutgoingCallerIdRequest = {
  accountSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                                      | Type                                                                                                                       | Required                                                                                                                   | Description                                                                                                                |
| -------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                                               | *string*                                                                                                                   | :heavy_check_mark:                                                                                                         | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the OutgoingCallerId resource to fetch. |
| `sid`                                                                                                                      | *string*                                                                                                                   | :heavy_check_mark:                                                                                                         | The Twilio-provided string that uniquely identifies the OutgoingCallerId resource to fetch.                                |