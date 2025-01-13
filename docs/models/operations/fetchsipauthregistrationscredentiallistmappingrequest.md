# FetchSipAuthRegistrationsCredentialListMappingRequest

## Example Usage

```typescript
import { FetchSipAuthRegistrationsCredentialListMappingRequest } from "twilio-sdk/models/operations";

let value: FetchSipAuthRegistrationsCredentialListMappingRequest = {
  accountSid: "<id>",
  domainSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                                           | Type                                                                                                                            | Required                                                                                                                        | Description                                                                                                                     |
| ------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                                                    | *string*                                                                                                                        | :heavy_check_mark:                                                                                                              | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the CredentialListMapping resource to fetch. |
| `domainSid`                                                                                                                     | *string*                                                                                                                        | :heavy_check_mark:                                                                                                              | The SID of the SIP domain that contains the resource to fetch.                                                                  |
| `sid`                                                                                                                           | *string*                                                                                                                        | :heavy_check_mark:                                                                                                              | The Twilio-provided string that uniquely identifies the CredentialListMapping resource to fetch.                                |