# UpdateCallRecordingRequest

## Example Usage

```typescript
import { UpdateCallRecordingRequest } from "twilio-sdk/models/operations";

let value: UpdateCallRecordingRequest = {
  accountSid: "<id>",
  callSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                                                | Type                                                                                                                                 | Required                                                                                                                             | Description                                                                                                                          |
| ------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------ |
| `accountSid`                                                                                                                         | *string*                                                                                                                             | :heavy_check_mark:                                                                                                                   | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the Recording resource to update.                 |
| `callSid`                                                                                                                            | *string*                                                                                                                             | :heavy_check_mark:                                                                                                                   | The [Call](https://www.twilio.com/docs/voice/api/call-resource) SID of the resource to update.                                       |
| `sid`                                                                                                                                | *string*                                                                                                                             | :heavy_check_mark:                                                                                                                   | The Twilio-provided string that uniquely identifies the Recording resource to update.                                                |
| `requestBody`                                                                                                                        | [operations.UpdateCallRecordingUpdateCallRecordingRequest](../../models/operations/updatecallrecordingupdatecallrecordingrequest.md) | :heavy_minus_sign:                                                                                                                   | N/A                                                                                                                                  |