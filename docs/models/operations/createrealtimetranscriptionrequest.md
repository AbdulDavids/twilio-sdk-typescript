# CreateRealtimeTranscriptionRequest

## Example Usage

```typescript
import { CreateRealtimeTranscriptionRequest } from "twilio-sdk/models/operations";

let value: CreateRealtimeTranscriptionRequest = {
  accountSid: "<id>",
  callSid: "<id>",
};
```

## Fields

| Field                                                                                                                                                                | Type                                                                                                                                                                 | Required                                                                                                                                                             | Description                                                                                                                                                          |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                                                                                         | *string*                                                                                                                                                             | :heavy_check_mark:                                                                                                                                                   | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created this Transcription resource.                                                      |
| `callSid`                                                                                                                                                            | *string*                                                                                                                                                             | :heavy_check_mark:                                                                                                                                                   | The SID of the [Call](https://www.twilio.com/docs/voice/api/call-resource) the Transcription resource is associated with.                                            |
| `requestBody`                                                                                                                                                        | [operations.CreateRealtimeTranscriptionCreateRealtimeTranscriptionRequest](../../models/operations/createrealtimetranscriptioncreaterealtimetranscriptionrequest.md) | :heavy_minus_sign:                                                                                                                                                   | N/A                                                                                                                                                                  |