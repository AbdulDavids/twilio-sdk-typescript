# FetchIncomingPhoneNumberAssignedAddOnExtensionRequest

## Example Usage

```typescript
import { FetchIncomingPhoneNumberAssignedAddOnExtensionRequest } from "twilio-sdk/models/operations";

let value: FetchIncomingPhoneNumberAssignedAddOnExtensionRequest = {
  accountSid: "<id>",
  resourceSid: "<id>",
  assignedAddOnSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                     | Type                                                                                                      | Required                                                                                                  | Description                                                                                               |
| --------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                              | *string*                                                                                                  | :heavy_check_mark:                                                                                        | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the resource to fetch. |
| `resourceSid`                                                                                             | *string*                                                                                                  | :heavy_check_mark:                                                                                        | The SID of the Phone Number to which the Add-on is assigned.                                              |
| `assignedAddOnSid`                                                                                        | *string*                                                                                                  | :heavy_check_mark:                                                                                        | The SID that uniquely identifies the assigned Add-on installation.                                        |
| `sid`                                                                                                     | *string*                                                                                                  | :heavy_check_mark:                                                                                        | The Twilio-provided string that uniquely identifies the resource to fetch.                                |