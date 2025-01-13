# CreateSiprecRequest

## Example Usage

```typescript
import { CreateSiprecRequest } from "twilio-sdk/models/operations";

let value: CreateSiprecRequest = {
  accountSid: "<id>",
  callSid: "<id>",
};
```

## Fields

| Field                                                                                                              | Type                                                                                                               | Required                                                                                                           | Description                                                                                                        |
| ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------ |
| `accountSid`                                                                                                       | *string*                                                                                                           | :heavy_check_mark:                                                                                                 | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created this Siprec resource.           |
| `callSid`                                                                                                          | *string*                                                                                                           | :heavy_check_mark:                                                                                                 | The SID of the [Call](https://www.twilio.com/docs/voice/api/call-resource) the Siprec resource is associated with. |
| `requestBody`                                                                                                      | [operations.CreateSiprecCreateSiprecRequest](../../models/operations/createsipreccreatesiprecrequest.md)           | :heavy_minus_sign:                                                                                                 | N/A                                                                                                                |