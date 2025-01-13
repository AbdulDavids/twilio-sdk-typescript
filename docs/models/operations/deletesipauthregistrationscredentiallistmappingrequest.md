# DeleteSipAuthRegistrationsCredentialListMappingRequest

## Example Usage

```typescript
import { DeleteSipAuthRegistrationsCredentialListMappingRequest } from "twilio-sdk/models/operations";

let value: DeleteSipAuthRegistrationsCredentialListMappingRequest = {
  accountSid: "<id>",
  domainSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                                             | Type                                                                                                                              | Required                                                                                                                          | Description                                                                                                                       |
| --------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                                                      | *string*                                                                                                                          | :heavy_check_mark:                                                                                                                | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the CredentialListMapping resources to delete. |
| `domainSid`                                                                                                                       | *string*                                                                                                                          | :heavy_check_mark:                                                                                                                | The SID of the SIP domain that contains the resources to delete.                                                                  |
| `sid`                                                                                                                             | *string*                                                                                                                          | :heavy_check_mark:                                                                                                                | The Twilio-provided string that uniquely identifies the CredentialListMapping resource to delete.                                 |