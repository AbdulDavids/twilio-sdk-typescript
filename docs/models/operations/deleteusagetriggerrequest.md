# DeleteUsageTriggerRequest

## Example Usage

```typescript
import { DeleteUsageTriggerRequest } from "twilio-sdk/models/operations";

let value: DeleteUsageTriggerRequest = {
  accountSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                                    | Type                                                                                                                     | Required                                                                                                                 | Description                                                                                                              |
| ------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------ |
| `accountSid`                                                                                                             | *string*                                                                                                                 | :heavy_check_mark:                                                                                                       | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the UsageTrigger resources to delete. |
| `sid`                                                                                                                    | *string*                                                                                                                 | :heavy_check_mark:                                                                                                       | The Twilio-provided string that uniquely identifies the UsageTrigger resource to delete.                                 |