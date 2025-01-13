# CreateSipCredentialListMappingCreateSipCredentialListMappingRequest

## Example Usage

```typescript
import { CreateSipCredentialListMappingCreateSipCredentialListMappingRequest } from "twilio-sdk/models/operations";

let value: CreateSipCredentialListMappingCreateSipCredentialListMappingRequest =
  {
    credentialListSid: "<id>",
  };
```

## Fields

| Field                                                                                                | Type                                                                                                 | Required                                                                                             | Description                                                                                          |
| ---------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- |
| `credentialListSid`                                                                                  | *string*                                                                                             | :heavy_check_mark:                                                                                   | A 34 character string that uniquely identifies the CredentialList resource to map to the SIP domain. |