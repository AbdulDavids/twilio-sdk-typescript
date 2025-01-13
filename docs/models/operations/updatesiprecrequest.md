# UpdateSiprecRequest

## Example Usage

```typescript
import { UpdateSiprecRequest } from "twilio-sdk/models/operations";

let value: UpdateSiprecRequest = {
  accountSid: "<id>",
  callSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                              | Type                                                                                                               | Required                                                                                                           | Description                                                                                                        |
| ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------ |
| `accountSid`                                                                                                       | *string*                                                                                                           | :heavy_check_mark:                                                                                                 | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created this Siprec resource.           |
| `callSid`                                                                                                          | *string*                                                                                                           | :heavy_check_mark:                                                                                                 | The SID of the [Call](https://www.twilio.com/docs/voice/api/call-resource) the Siprec resource is associated with. |
| `sid`                                                                                                              | *string*                                                                                                           | :heavy_check_mark:                                                                                                 | The SID of the Siprec resource, or the `name` used when creating the resource                                      |
| `requestBody`                                                                                                      | [operations.UpdateSiprecUpdateSiprecRequest](../../models/operations/updatesiprecupdatesiprecrequest.md)           | :heavy_minus_sign:                                                                                                 | N/A                                                                                                                |