# DeleteCallRecordingRequest

## Example Usage

```typescript
import { DeleteCallRecordingRequest } from "twilio-sdk/models/operations";

let value: DeleteCallRecordingRequest = {
  accountSid: "<id>",
  callSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                                 | Type                                                                                                                  | Required                                                                                                              | Description                                                                                                           |
| --------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                                          | *string*                                                                                                              | :heavy_check_mark:                                                                                                    | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the Recording resources to delete. |
| `callSid`                                                                                                             | *string*                                                                                                              | :heavy_check_mark:                                                                                                    | The [Call](https://www.twilio.com/docs/voice/api/call-resource) SID of the resources to delete.                       |
| `sid`                                                                                                                 | *string*                                                                                                              | :heavy_check_mark:                                                                                                    | The Twilio-provided string that uniquely identifies the Recording resource to delete.                                 |