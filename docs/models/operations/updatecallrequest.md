# UpdateCallRequest

## Example Usage

```typescript
import { UpdateCallRequest } from "twilio-sdk/models/operations";

let value: UpdateCallRequest = {
  accountSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                              | Type                                                                                                               | Required                                                                                                           | Description                                                                                                        |
| ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------ |
| `accountSid`                                                                                                       | *string*                                                                                                           | :heavy_check_mark:                                                                                                 | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the Call resource(s) to update. |
| `sid`                                                                                                              | *string*                                                                                                           | :heavy_check_mark:                                                                                                 | The Twilio-provided string that uniquely identifies the Call resource to update                                    |
| `requestBody`                                                                                                      | [operations.UpdateCallUpdateCallRequest](../../models/operations/updatecallupdatecallrequest.md)                   | :heavy_minus_sign:                                                                                                 | N/A                                                                                                                |