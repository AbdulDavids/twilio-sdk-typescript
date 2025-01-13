# DeleteIncomingPhoneNumberAssignedAddOnRequest

## Example Usage

```typescript
import { DeleteIncomingPhoneNumberAssignedAddOnRequest } from "twilio-sdk/models/operations";

let value: DeleteIncomingPhoneNumberAssignedAddOnRequest = {
  accountSid: "<id>",
  resourceSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                       | Type                                                                                                        | Required                                                                                                    | Description                                                                                                 |
| ----------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                                | *string*                                                                                                    | :heavy_check_mark:                                                                                          | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the resources to delete. |
| `resourceSid`                                                                                               | *string*                                                                                                    | :heavy_check_mark:                                                                                          | The SID of the Phone Number to which the Add-on is assigned.                                                |
| `sid`                                                                                                       | *string*                                                                                                    | :heavy_check_mark:                                                                                          | The Twilio-provided string that uniquely identifies the resource to delete.                                 |