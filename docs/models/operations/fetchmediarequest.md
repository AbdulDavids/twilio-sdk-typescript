# FetchMediaRequest

## Example Usage

```typescript
import { FetchMediaRequest } from "twilio-sdk/models/operations";

let value: FetchMediaRequest = {
  accountSid: "<id>",
  messageSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                     | Type                                                                                                      | Required                                                                                                  | Description                                                                                               |
| --------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                              | *string*                                                                                                  | :heavy_check_mark:                                                                                        | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) associated with the Media resource. |
| `messageSid`                                                                                              | *string*                                                                                                  | :heavy_check_mark:                                                                                        | The SID of the Message resource that is associated with the Media resource.                               |
| `sid`                                                                                                     | *string*                                                                                                  | :heavy_check_mark:                                                                                        | The Twilio-provided string that uniquely identifies the Media resource to fetch.                          |