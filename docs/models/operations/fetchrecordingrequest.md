# FetchRecordingRequest

## Example Usage

```typescript
import { FetchRecordingRequest } from "twilio-sdk/models/operations";

let value: FetchRecordingRequest = {
  accountSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                                                                             | Type                                                                                                                                                              | Required                                                                                                                                                          | Description                                                                                                                                                       |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                                                                                      | *string*                                                                                                                                                          | :heavy_check_mark:                                                                                                                                                | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the Recording resource to fetch.                                               |
| `sid`                                                                                                                                                             | *string*                                                                                                                                                          | :heavy_check_mark:                                                                                                                                                | The Twilio-provided string that uniquely identifies the Recording resource to fetch.                                                                              |
| `includeSoftDeleted`                                                                                                                                              | *boolean*                                                                                                                                                         | :heavy_minus_sign:                                                                                                                                                | A boolean parameter indicating whether to retrieve soft deleted recordings or not. Recordings metadata are kept after deletion for a retention period of 40 days. |