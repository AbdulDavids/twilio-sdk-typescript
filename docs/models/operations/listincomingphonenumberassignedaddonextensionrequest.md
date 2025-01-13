# ListIncomingPhoneNumberAssignedAddOnExtensionRequest

## Example Usage

```typescript
import { ListIncomingPhoneNumberAssignedAddOnExtensionRequest } from "twilio-sdk/models/operations";

let value: ListIncomingPhoneNumberAssignedAddOnExtensionRequest = {
  accountSid: "<id>",
  resourceSid: "<id>",
  assignedAddOnSid: "<id>",
};
```

## Fields

| Field                                                                                                     | Type                                                                                                      | Required                                                                                                  | Description                                                                                               |
| --------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                              | *string*                                                                                                  | :heavy_check_mark:                                                                                        | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the resources to read. |
| `resourceSid`                                                                                             | *string*                                                                                                  | :heavy_check_mark:                                                                                        | The SID of the Phone Number to which the Add-on is assigned.                                              |
| `assignedAddOnSid`                                                                                        | *string*                                                                                                  | :heavy_check_mark:                                                                                        | The SID that uniquely identifies the assigned Add-on installation.                                        |
| `pageSize`                                                                                                | *number*                                                                                                  | :heavy_minus_sign:                                                                                        | How many resources to return in each list page. The default is 50, and the maximum is 1000.               |
| `page`                                                                                                    | *number*                                                                                                  | :heavy_minus_sign:                                                                                        | The page index. This value is simply for client state.                                                    |
| `pageToken`                                                                                               | *string*                                                                                                  | :heavy_minus_sign:                                                                                        | The page token. This is provided by the API.                                                              |