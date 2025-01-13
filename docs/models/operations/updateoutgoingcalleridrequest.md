# UpdateOutgoingCallerIdRequest

## Example Usage

```typescript
import { UpdateOutgoingCallerIdRequest } from "twilio-sdk/models/operations";

let value: UpdateOutgoingCallerIdRequest = {
  accountSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                                                            | Type                                                                                                                                             | Required                                                                                                                                         | Description                                                                                                                                      |
| ------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------ |
| `accountSid`                                                                                                                                     | *string*                                                                                                                                         | :heavy_check_mark:                                                                                                                               | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the OutgoingCallerId resources to update.                     |
| `sid`                                                                                                                                            | *string*                                                                                                                                         | :heavy_check_mark:                                                                                                                               | The Twilio-provided string that uniquely identifies the OutgoingCallerId resource to update.                                                     |
| `requestBody`                                                                                                                                    | [operations.UpdateOutgoingCallerIdUpdateOutgoingCallerIdRequest](../../models/operations/updateoutgoingcalleridupdateoutgoingcalleridrequest.md) | :heavy_minus_sign:                                                                                                                               | N/A                                                                                                                                              |