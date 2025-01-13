# UpdateMessageRequest

## Example Usage

```typescript
import { UpdateMessageRequest } from "twilio-sdk/models/operations";

let value: UpdateMessageRequest = {
  accountSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                               | Type                                                                                                                | Required                                                                                                            | Description                                                                                                         |
| ------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                                        | *string*                                                                                                            | :heavy_check_mark:                                                                                                  | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the Message resources to update. |
| `sid`                                                                                                               | *string*                                                                                                            | :heavy_check_mark:                                                                                                  | The SID of the Message resource to be updated                                                                       |
| `requestBody`                                                                                                       | [operations.UpdateMessageUpdateMessageRequest](../../models/operations/updatemessageupdatemessagerequest.md)        | :heavy_minus_sign:                                                                                                  | N/A                                                                                                                 |