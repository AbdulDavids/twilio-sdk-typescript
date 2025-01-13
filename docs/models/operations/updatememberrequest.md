# UpdateMemberRequest

## Example Usage

```typescript
import { UpdateMemberRequest } from "twilio-sdk/models/operations";

let value: UpdateMemberRequest = {
  accountSid: "<id>",
  queueSid: "<id>",
  callSid: "<id>",
};
```

## Fields

| Field                                                                                                                | Type                                                                                                                 | Required                                                                                                             | Description                                                                                                          |
| -------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                                         | *string*                                                                                                             | :heavy_check_mark:                                                                                                   | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the Member resource(s) to update. |
| `queueSid`                                                                                                           | *string*                                                                                                             | :heavy_check_mark:                                                                                                   | The SID of the Queue in which to find the members to update.                                                         |
| `callSid`                                                                                                            | *string*                                                                                                             | :heavy_check_mark:                                                                                                   | The [Call](https://www.twilio.com/docs/voice/api/call-resource) SID of the resource(s) to update.                    |
| `requestBody`                                                                                                        | [operations.UpdateMemberUpdateMemberRequest](../../models/operations/updatememberupdatememberrequest.md)             | :heavy_minus_sign:                                                                                                   | N/A                                                                                                                  |