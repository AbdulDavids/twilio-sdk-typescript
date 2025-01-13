# CreateNewSigningKeyRequest

## Example Usage

```typescript
import { CreateNewSigningKeyRequest } from "twilio-sdk/models/operations";

let value: CreateNewSigningKeyRequest = {
  accountSid: "<id>",
};
```

## Fields

| Field                                                                                                                                | Type                                                                                                                                 | Required                                                                                                                             | Description                                                                                                                          |
| ------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------ |
| `accountSid`                                                                                                                         | *string*                                                                                                                             | :heavy_check_mark:                                                                                                                   | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that will be responsible for the new Key resource.             |
| `requestBody`                                                                                                                        | [operations.CreateNewSigningKeyCreateNewSigningKeyRequest](../../models/operations/createnewsigningkeycreatenewsigningkeyrequest.md) | :heavy_minus_sign:                                                                                                                   | N/A                                                                                                                                  |