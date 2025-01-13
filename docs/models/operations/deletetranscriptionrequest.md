# DeleteTranscriptionRequest

## Example Usage

```typescript
import { DeleteTranscriptionRequest } from "twilio-sdk/models/operations";

let value: DeleteTranscriptionRequest = {
  accountSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                                     | Type                                                                                                                      | Required                                                                                                                  | Description                                                                                                               |
| ------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                                              | *string*                                                                                                                  | :heavy_check_mark:                                                                                                        | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the Transcription resources to delete. |
| `sid`                                                                                                                     | *string*                                                                                                                  | :heavy_check_mark:                                                                                                        | The Twilio-provided string that uniquely identifies the Transcription resource to delete.                                 |