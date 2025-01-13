# CreatePaymentsRequest

## Example Usage

```typescript
import { CreatePaymentsRequest } from "twilio-sdk/models/operations";

let value: CreatePaymentsRequest = {
  accountSid: "<id>",
  callSid: "<id>",
};
```

## Fields

| Field                                                                                                                                      | Type                                                                                                                                       | Required                                                                                                                                   | Description                                                                                                                                |
| ------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------ |
| `accountSid`                                                                                                                               | *string*                                                                                                                                   | :heavy_check_mark:                                                                                                                         | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that will create the resource.                                       |
| `callSid`                                                                                                                                  | *string*                                                                                                                                   | :heavy_check_mark:                                                                                                                         | The SID of the call that will create the resource. Call leg associated with this sid is expected to provide payment information thru DTMF. |
| `requestBody`                                                                                                                              | [operations.CreatePaymentsCreatePaymentsRequest](../../models/operations/createpaymentscreatepaymentsrequest.md)                           | :heavy_minus_sign:                                                                                                                         | N/A                                                                                                                                        |