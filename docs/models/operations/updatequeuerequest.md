# UpdateQueueRequest

## Example Usage

```typescript
import { UpdateQueueRequest } from "twilio-sdk/models/operations";

let value: UpdateQueueRequest = {
  accountSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                            | Type                                                                                                             | Required                                                                                                         | Description                                                                                                      |
| ---------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                                     | *string*                                                                                                         | :heavy_check_mark:                                                                                               | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the Queue resource to update. |
| `sid`                                                                                                            | *string*                                                                                                         | :heavy_check_mark:                                                                                               | The Twilio-provided string that uniquely identifies the Queue resource to update                                 |
| `requestBody`                                                                                                    | [operations.UpdateQueueUpdateQueueRequest](../../models/operations/updatequeueupdatequeuerequest.md)             | :heavy_minus_sign:                                                                                               | N/A                                                                                                              |