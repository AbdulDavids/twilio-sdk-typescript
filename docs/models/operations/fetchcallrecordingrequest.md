# FetchCallRecordingRequest

## Example Usage

```typescript
import { FetchCallRecordingRequest } from "twilio-sdk/models/operations";

let value: FetchCallRecordingRequest = {
  accountSid: "<id>",
  callSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                               | Type                                                                                                                | Required                                                                                                            | Description                                                                                                         |
| ------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                                        | *string*                                                                                                            | :heavy_check_mark:                                                                                                  | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the Recording resource to fetch. |
| `callSid`                                                                                                           | *string*                                                                                                            | :heavy_check_mark:                                                                                                  | The [Call](https://www.twilio.com/docs/voice/api/call-resource) SID of the resource to fetch.                       |
| `sid`                                                                                                               | *string*                                                                                                            | :heavy_check_mark:                                                                                                  | The Twilio-provided string that uniquely identifies the Recording resource to fetch.                                |