# DeleteRecordingAddOnResultRequest

## Example Usage

```typescript
import { DeleteRecordingAddOnResultRequest } from "twilio-sdk/models/operations";

let value: DeleteRecordingAddOnResultRequest = {
  accountSid: "<id>",
  referenceSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                                             | Type                                                                                                                              | Required                                                                                                                          | Description                                                                                                                       |
| --------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                                                      | *string*                                                                                                                          | :heavy_check_mark:                                                                                                                | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the Recording AddOnResult resources to delete. |
| `referenceSid`                                                                                                                    | *string*                                                                                                                          | :heavy_check_mark:                                                                                                                | The SID of the recording to which the result to delete belongs.                                                                   |
| `sid`                                                                                                                             | *string*                                                                                                                          | :heavy_check_mark:                                                                                                                | The Twilio-provided string that uniquely identifies the Recording AddOnResult resource to delete.                                 |