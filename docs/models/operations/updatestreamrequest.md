# UpdateStreamRequest

## Example Usage

```typescript
import { UpdateStreamRequest } from "twilio-sdk/models/operations";

let value: UpdateStreamRequest = {
  accountSid: "<id>",
  callSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                              | Type                                                                                                               | Required                                                                                                           | Description                                                                                                        |
| ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------ |
| `accountSid`                                                                                                       | *string*                                                                                                           | :heavy_check_mark:                                                                                                 | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created this Stream resource.           |
| `callSid`                                                                                                          | *string*                                                                                                           | :heavy_check_mark:                                                                                                 | The SID of the [Call](https://www.twilio.com/docs/voice/api/call-resource) the Stream resource is associated with. |
| `sid`                                                                                                              | *string*                                                                                                           | :heavy_check_mark:                                                                                                 | The SID or the `name` of the Stream resource to be stopped                                                         |
| `requestBody`                                                                                                      | [operations.UpdateStreamUpdateStreamRequest](../../models/operations/updatestreamupdatestreamrequest.md)           | :heavy_minus_sign:                                                                                                 | N/A                                                                                                                |