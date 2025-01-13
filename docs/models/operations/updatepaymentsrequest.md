# UpdatePaymentsRequest

## Example Usage

```typescript
import { UpdatePaymentsRequest } from "twilio-sdk/models/operations";

let value: UpdatePaymentsRequest = {
  accountSid: "<id>",
  callSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                                          | Type                                                                                                                           | Required                                                                                                                       | Description                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------ |
| `accountSid`                                                                                                                   | *string*                                                                                                                       | :heavy_check_mark:                                                                                                             | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that will update the resource.                           |
| `callSid`                                                                                                                      | *string*                                                                                                                       | :heavy_check_mark:                                                                                                             | The SID of the call that will update the resource. This should be the same call sid that was used to create payments resource. |
| `sid`                                                                                                                          | *string*                                                                                                                       | :heavy_check_mark:                                                                                                             | The SID of Payments session that needs to be updated.                                                                          |
| `requestBody`                                                                                                                  | [operations.UpdatePaymentsUpdatePaymentsRequest](../../models/operations/updatepaymentsupdatepaymentsrequest.md)               | :heavy_minus_sign:                                                                                                             | N/A                                                                                                                            |