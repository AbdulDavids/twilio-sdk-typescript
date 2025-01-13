# DeleteRecordingTranscriptionRequest

## Example Usage

```typescript
import { DeleteRecordingTranscriptionRequest } from "twilio-sdk/models/operations";

let value: DeleteRecordingTranscriptionRequest = {
  accountSid: "<id>",
  recordingSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                                     | Type                                                                                                                      | Required                                                                                                                  | Description                                                                                                               |
| ------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                                              | *string*                                                                                                                  | :heavy_check_mark:                                                                                                        | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the Transcription resources to delete. |
| `recordingSid`                                                                                                            | *string*                                                                                                                  | :heavy_check_mark:                                                                                                        | The SID of the [Recording](https://www.twilio.com/docs/voice/api/recording) that created the transcription to delete.     |
| `sid`                                                                                                                     | *string*                                                                                                                  | :heavy_check_mark:                                                                                                        | The Twilio-provided string that uniquely identifies the Transcription resource to delete.                                 |