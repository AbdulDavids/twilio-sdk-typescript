# CreateSipAuthRegistrationsCredentialListMappingCreateSipAuthRegistrationsCredentialListMappingRequest

## Example Usage

```typescript
import {
  CreateSipAuthRegistrationsCredentialListMappingCreateSipAuthRegistrationsCredentialListMappingRequest,
} from "twilio-sdk/models/operations";

let value:
  CreateSipAuthRegistrationsCredentialListMappingCreateSipAuthRegistrationsCredentialListMappingRequest =
    {
      credentialListSid: "<id>",
    };
```

## Fields

| Field                                                            | Type                                                             | Required                                                         | Description                                                      |
| ---------------------------------------------------------------- | ---------------------------------------------------------------- | ---------------------------------------------------------------- | ---------------------------------------------------------------- |
| `credentialListSid`                                              | *string*                                                         | :heavy_check_mark:                                               | The SID of the CredentialList resource to map to the SIP domain. |