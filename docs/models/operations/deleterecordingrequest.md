# DeleteRecordingRequest

## Example Usage

```typescript
import { DeleteRecordingRequest } from "twilio-sdk/models/operations";

let value: DeleteRecordingRequest = {
  accountSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                                 | Type                                                                                                                  | Required                                                                                                              | Description                                                                                                           |
| --------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                                          | *string*                                                                                                              | :heavy_check_mark:                                                                                                    | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the Recording resources to delete. |
| `sid`                                                                                                                 | *string*                                                                                                              | :heavy_check_mark:                                                                                                    | The Twilio-provided string that uniquely identifies the Recording resource to delete.                                 |