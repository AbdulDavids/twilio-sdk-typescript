# CreateAddressRequest

## Example Usage

```typescript
import { CreateAddressRequest } from "twilio-sdk/models/operations";

let value: CreateAddressRequest = {
  accountSid: "<id>",
};
```

## Fields

| Field                                                                                                                        | Type                                                                                                                         | Required                                                                                                                     | Description                                                                                                                  |
| ---------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                                                 | *string*                                                                                                                     | :heavy_check_mark:                                                                                                           | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that will be responsible for the new Address resource. |
| `requestBody`                                                                                                                | [operations.CreateAddressCreateAddressRequest](../../models/operations/createaddresscreateaddressrequest.md)                 | :heavy_minus_sign:                                                                                                           | N/A                                                                                                                          |