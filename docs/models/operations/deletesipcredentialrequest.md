# DeleteSipCredentialRequest

## Example Usage

```typescript
import { DeleteSipCredentialRequest } from "twilio-sdk/models/operations";

let value: DeleteSipCredentialRequest = {
  accountSid: "<id>",
  credentialListSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                    | Type                                                                                     | Required                                                                                 | Description                                                                              |
| ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- |
| `accountSid`                                                                             | *string*                                                                                 | :heavy_check_mark:                                                                       | The unique id of the Account that is responsible for this resource.                      |
| `credentialListSid`                                                                      | *string*                                                                                 | :heavy_check_mark:                                                                       | The unique id that identifies the credential list that contains the desired credentials. |
| `sid`                                                                                    | *string*                                                                                 | :heavy_check_mark:                                                                       | The unique id that identifies the resource to delete.                                    |