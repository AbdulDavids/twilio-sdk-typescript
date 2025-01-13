# UpdateUsageTriggerRequest

## Example Usage

```typescript
import { UpdateUsageTriggerRequest } from "twilio-sdk/models/operations";

let value: UpdateUsageTriggerRequest = {
  accountSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                                            | Type                                                                                                                             | Required                                                                                                                         | Description                                                                                                                      |
| -------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                                                     | *string*                                                                                                                         | :heavy_check_mark:                                                                                                               | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the UsageTrigger resources to update.         |
| `sid`                                                                                                                            | *string*                                                                                                                         | :heavy_check_mark:                                                                                                               | The Twilio-provided string that uniquely identifies the UsageTrigger resource to update.                                         |
| `requestBody`                                                                                                                    | [operations.UpdateUsageTriggerUpdateUsageTriggerRequest](../../models/operations/updateusagetriggerupdateusagetriggerrequest.md) | :heavy_minus_sign:                                                                                                               | N/A                                                                                                                              |