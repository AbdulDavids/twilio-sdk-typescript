# CreateNewKeyRequest

## Example Usage

```typescript
import { CreateNewKeyRequest } from "twilio-sdk/models/operations";

let value: CreateNewKeyRequest = {
  accountSid: "<id>",
};
```

## Fields

| Field                                                                                                                    | Type                                                                                                                     | Required                                                                                                                 | Description                                                                                                              |
| ------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------ |
| `accountSid`                                                                                                             | *string*                                                                                                                 | :heavy_check_mark:                                                                                                       | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that will be responsible for the new Key resource. |
| `requestBody`                                                                                                            | [operations.CreateNewKeyCreateNewKeyRequest](../../models/operations/createnewkeycreatenewkeyrequest.md)                 | :heavy_minus_sign:                                                                                                       | N/A                                                                                                                      |