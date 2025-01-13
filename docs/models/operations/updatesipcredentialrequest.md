# UpdateSipCredentialRequest

## Example Usage

```typescript
import { UpdateSipCredentialRequest } from "twilio-sdk/models/operations";

let value: UpdateSipCredentialRequest = {
  accountSid: "<id>",
  credentialListSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                                                | Type                                                                                                                                 | Required                                                                                                                             | Description                                                                                                                          |
| ------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------ |
| `accountSid`                                                                                                                         | *string*                                                                                                                             | :heavy_check_mark:                                                                                                                   | The unique id of the Account that is responsible for this resource.                                                                  |
| `credentialListSid`                                                                                                                  | *string*                                                                                                                             | :heavy_check_mark:                                                                                                                   | The unique id that identifies the credential list that includes this credential.                                                     |
| `sid`                                                                                                                                | *string*                                                                                                                             | :heavy_check_mark:                                                                                                                   | The unique id that identifies the resource to update.                                                                                |
| `requestBody`                                                                                                                        | [operations.UpdateSipCredentialUpdateSipCredentialRequest](../../models/operations/updatesipcredentialupdatesipcredentialrequest.md) | :heavy_minus_sign:                                                                                                                   | N/A                                                                                                                                  |