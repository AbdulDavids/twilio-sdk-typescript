# ListSipAuthCallsCredentialListMappingRequest

## Example Usage

```typescript
import { ListSipAuthCallsCredentialListMappingRequest } from "twilio-sdk/models/operations";

let value: ListSipAuthCallsCredentialListMappingRequest = {
  accountSid: "<id>",
  domainSid: "<id>",
};
```

## Fields

| Field                                                                                                                           | Type                                                                                                                            | Required                                                                                                                        | Description                                                                                                                     |
| ------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                                                    | *string*                                                                                                                        | :heavy_check_mark:                                                                                                              | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the CredentialListMapping resources to read. |
| `domainSid`                                                                                                                     | *string*                                                                                                                        | :heavy_check_mark:                                                                                                              | The SID of the SIP domain that contains the resources to read.                                                                  |
| `pageSize`                                                                                                                      | *number*                                                                                                                        | :heavy_minus_sign:                                                                                                              | How many resources to return in each list page. The default is 50, and the maximum is 1000.                                     |
| `page`                                                                                                                          | *number*                                                                                                                        | :heavy_minus_sign:                                                                                                              | The page index. This value is simply for client state.                                                                          |
| `pageToken`                                                                                                                     | *string*                                                                                                                        | :heavy_minus_sign:                                                                                                              | The page token. This is provided by the API.                                                                                    |