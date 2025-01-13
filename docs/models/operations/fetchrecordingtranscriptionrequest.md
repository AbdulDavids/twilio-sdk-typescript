# FetchRecordingTranscriptionRequest

## Example Usage

```typescript
import { FetchRecordingTranscriptionRequest } from "twilio-sdk/models/operations";

let value: FetchRecordingTranscriptionRequest = {
  accountSid: "<id>",
  recordingSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                                   | Type                                                                                                                    | Required                                                                                                                | Description                                                                                                             |
| ----------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                                            | *string*                                                                                                                | :heavy_check_mark:                                                                                                      | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the Transcription resource to fetch. |
| `recordingSid`                                                                                                          | *string*                                                                                                                | :heavy_check_mark:                                                                                                      | The SID of the [Recording](https://www.twilio.com/docs/voice/api/recording) that created the transcription to fetch.    |
| `sid`                                                                                                                   | *string*                                                                                                                | :heavy_check_mark:                                                                                                      | The Twilio-provided string that uniquely identifies the Transcription resource to fetch.                                |