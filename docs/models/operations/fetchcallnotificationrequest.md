# FetchCallNotificationRequest

## Example Usage

```typescript
import { FetchCallNotificationRequest } from "twilio-sdk/models/operations";

let value: FetchCallNotificationRequest = {
  accountSid: "<id>",
  callSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                                       | Type                                                                                                                        | Required                                                                                                                    | Description                                                                                                                 |
| --------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                                                | *string*                                                                                                                    | :heavy_check_mark:                                                                                                          | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the Call Notification resource to fetch. |
| `callSid`                                                                                                                   | *string*                                                                                                                    | :heavy_check_mark:                                                                                                          | The [Call](https://www.twilio.com/docs/voice/api/call-resource) SID of the Call Notification resource to fetch.             |
| `sid`                                                                                                                       | *string*                                                                                                                    | :heavy_check_mark:                                                                                                          | The Twilio-provided string that uniquely identifies the Call Notification resource to fetch.                                |