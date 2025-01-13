# FetchIncomingPhoneNumberAssignedAddOnRequest

## Example Usage

```typescript
import { FetchIncomingPhoneNumberAssignedAddOnRequest } from "twilio-sdk/models/operations";

let value: FetchIncomingPhoneNumberAssignedAddOnRequest = {
  accountSid: "<id>",
  resourceSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                     | Type                                                                                                      | Required                                                                                                  | Description                                                                                               |
| --------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                              | *string*                                                                                                  | :heavy_check_mark:                                                                                        | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the resource to fetch. |
| `resourceSid`                                                                                             | *string*                                                                                                  | :heavy_check_mark:                                                                                        | The SID of the Phone Number to which the Add-on is assigned.                                              |
| `sid`                                                                                                     | *string*                                                                                                  | :heavy_check_mark:                                                                                        | The Twilio-provided string that uniquely identifies the resource to fetch.                                |