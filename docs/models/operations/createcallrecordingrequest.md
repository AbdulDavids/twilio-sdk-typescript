# CreateCallRecordingRequest

## Example Usage

```typescript
import { CreateCallRecordingRequest } from "twilio-sdk/models/operations";

let value: CreateCallRecordingRequest = {
  accountSid: "<id>",
  callSid: "<id>",
};
```

## Fields

| Field                                                                                                                                | Type                                                                                                                                 | Required                                                                                                                             | Description                                                                                                                          |
| ------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------ |
| `accountSid`                                                                                                                         | *string*                                                                                                                             | :heavy_check_mark:                                                                                                                   | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that will create the resource.                                 |
| `callSid`                                                                                                                            | *string*                                                                                                                             | :heavy_check_mark:                                                                                                                   | The SID of the [Call](https://www.twilio.com/docs/voice/api/call-resource) to associate the resource with.                           |
| `requestBody`                                                                                                                        | [operations.CreateCallRecordingCreateCallRecordingRequest](../../models/operations/createcallrecordingcreatecallrecordingrequest.md) | :heavy_minus_sign:                                                                                                                   | N/A                                                                                                                                  |