# FetchSipDomainRequest

## Example Usage

```typescript
import { FetchSipDomainRequest } from "twilio-sdk/models/operations";

let value: FetchSipDomainRequest = {
  accountSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                               | Type                                                                                                                | Required                                                                                                            | Description                                                                                                         |
| ------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                                        | *string*                                                                                                            | :heavy_check_mark:                                                                                                  | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the SipDomain resource to fetch. |
| `sid`                                                                                                               | *string*                                                                                                            | :heavy_check_mark:                                                                                                  | The Twilio-provided string that uniquely identifies the SipDomain resource to fetch.                                |