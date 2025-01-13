# FetchRecordingAddOnResultRequest

## Example Usage

```typescript
import { FetchRecordingAddOnResultRequest } from "twilio-sdk/models/operations";

let value: FetchRecordingAddOnResultRequest = {
  accountSid: "<id>",
  referenceSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                                           | Type                                                                                                                            | Required                                                                                                                        | Description                                                                                                                     |
| ------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                                                    | *string*                                                                                                                        | :heavy_check_mark:                                                                                                              | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the Recording AddOnResult resource to fetch. |
| `referenceSid`                                                                                                                  | *string*                                                                                                                        | :heavy_check_mark:                                                                                                              | The SID of the recording to which the result to fetch belongs.                                                                  |
| `sid`                                                                                                                           | *string*                                                                                                                        | :heavy_check_mark:                                                                                                              | The Twilio-provided string that uniquely identifies the Recording AddOnResult resource to fetch.                                |