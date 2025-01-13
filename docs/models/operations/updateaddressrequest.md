# UpdateAddressRequest

## Example Usage

```typescript
import { UpdateAddressRequest } from "twilio-sdk/models/operations";

let value: UpdateAddressRequest = {
  accountSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                                         | Type                                                                                                                          | Required                                                                                                                      | Description                                                                                                                   |
| ----------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                                                  | *string*                                                                                                                      | :heavy_check_mark:                                                                                                            | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that is responsible for the Address resource to update. |
| `sid`                                                                                                                         | *string*                                                                                                                      | :heavy_check_mark:                                                                                                            | The Twilio-provided string that uniquely identifies the Address resource to update.                                           |
| `requestBody`                                                                                                                 | [operations.UpdateAddressUpdateAddressRequest](../../models/operations/updateaddressupdateaddressrequest.md)                  | :heavy_minus_sign:                                                                                                            | N/A                                                                                                                           |