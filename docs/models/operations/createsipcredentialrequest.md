# CreateSipCredentialRequest

## Example Usage

```typescript
import { CreateSipCredentialRequest } from "twilio-sdk/models/operations";

let value: CreateSipCredentialRequest = {
  accountSid: "<id>",
  credentialListSid: "<id>",
};
```

## Fields

| Field                                                                                                                                | Type                                                                                                                                 | Required                                                                                                                             | Description                                                                                                                          |
| ------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------ |
| `accountSid`                                                                                                                         | *string*                                                                                                                             | :heavy_check_mark:                                                                                                                   | The unique id of the Account that is responsible for this resource.                                                                  |
| `credentialListSid`                                                                                                                  | *string*                                                                                                                             | :heavy_check_mark:                                                                                                                   | The unique id that identifies the credential list to include the created credential.                                                 |
| `requestBody`                                                                                                                        | [operations.CreateSipCredentialCreateSipCredentialRequest](../../models/operations/createsipcredentialcreatesipcredentialrequest.md) | :heavy_minus_sign:                                                                                                                   | N/A                                                                                                                                  |