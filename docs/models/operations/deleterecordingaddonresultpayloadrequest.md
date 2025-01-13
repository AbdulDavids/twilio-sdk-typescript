# DeleteRecordingAddOnResultPayloadRequest

## Example Usage

```typescript
import { DeleteRecordingAddOnResultPayloadRequest } from "twilio-sdk/models/operations";

let value: DeleteRecordingAddOnResultPayloadRequest = {
  accountSid: "<id>",
  referenceSid: "<id>",
  addOnResultSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                                                     | Type                                                                                                                                      | Required                                                                                                                                  | Description                                                                                                                               |
| ----------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                                                              | *string*                                                                                                                                  | :heavy_check_mark:                                                                                                                        | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the Recording AddOnResult Payload resources to delete. |
| `referenceSid`                                                                                                                            | *string*                                                                                                                                  | :heavy_check_mark:                                                                                                                        | The SID of the recording to which the AddOnResult resource that contains the payloads to delete belongs.                                  |
| `addOnResultSid`                                                                                                                          | *string*                                                                                                                                  | :heavy_check_mark:                                                                                                                        | The SID of the AddOnResult to which the payloads to delete belongs.                                                                       |
| `sid`                                                                                                                                     | *string*                                                                                                                                  | :heavy_check_mark:                                                                                                                        | The Twilio-provided string that uniquely identifies the Recording AddOnResult Payload resource to delete.                                 |