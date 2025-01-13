# CreateParticipantRequest

## Example Usage

```typescript
import { CreateParticipantRequest } from "twilio-sdk/models/operations";

let value: CreateParticipantRequest = {
  accountSid: "<id>",
  conferenceSid: "<id>",
};
```

## Fields

| Field                                                                                                                        | Type                                                                                                                         | Required                                                                                                                     | Description                                                                                                                  |
| ---------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                                                 | *string*                                                                                                                     | :heavy_check_mark:                                                                                                           | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that will create the resource.                         |
| `conferenceSid`                                                                                                              | *string*                                                                                                                     | :heavy_check_mark:                                                                                                           | The SID of the participant's conference.                                                                                     |
| `requestBody`                                                                                                                | [operations.CreateParticipantCreateParticipantRequest](../../models/operations/createparticipantcreateparticipantrequest.md) | :heavy_minus_sign:                                                                                                           | N/A                                                                                                                          |