# CreateStreamRequest

## Example Usage

```typescript
import { CreateStreamRequest } from "twilio-sdk/models/operations";

let value: CreateStreamRequest = {
  accountSid: "<id>",
  callSid: "<id>",
};
```

## Fields

| Field                                                                                                              | Type                                                                                                               | Required                                                                                                           | Description                                                                                                        |
| ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------ |
| `accountSid`                                                                                                       | *string*                                                                                                           | :heavy_check_mark:                                                                                                 | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created this Stream resource.           |
| `callSid`                                                                                                          | *string*                                                                                                           | :heavy_check_mark:                                                                                                 | The SID of the [Call](https://www.twilio.com/docs/voice/api/call-resource) the Stream resource is associated with. |
| `requestBody`                                                                                                      | [operations.CreateStreamCreateStreamRequest](../../models/operations/createstreamcreatestreamrequest.md)           | :heavy_minus_sign:                                                                                                 | N/A                                                                                                                |