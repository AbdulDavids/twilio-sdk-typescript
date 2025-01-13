# FetchSipCredentialListMappingRequest

## Example Usage

```typescript
import { FetchSipCredentialListMappingRequest } from "twilio-sdk/models/operations";

let value: FetchSipCredentialListMappingRequest = {
  accountSid: "<id>",
  domainSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                      | Type                                                                                                       | Required                                                                                                   | Description                                                                                                |
| ---------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                               | *string*                                                                                                   | :heavy_check_mark:                                                                                         | The unique id of the [Account](https://www.twilio.com/docs/iam/api/account) responsible for this resource. |
| `domainSid`                                                                                                | *string*                                                                                                   | :heavy_check_mark:                                                                                         | A 34 character string that uniquely identifies the SIP Domain that includes the resource to fetch.         |
| `sid`                                                                                                      | *string*                                                                                                   | :heavy_check_mark:                                                                                         | A 34 character string that uniquely identifies the resource to fetch.                                      |