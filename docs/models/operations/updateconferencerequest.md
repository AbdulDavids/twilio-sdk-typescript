# UpdateConferenceRequest

## Example Usage

```typescript
import { UpdateConferenceRequest } from "twilio-sdk/models/operations";

let value: UpdateConferenceRequest = {
  accountSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                                    | Type                                                                                                                     | Required                                                                                                                 | Description                                                                                                              |
| ------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------ |
| `accountSid`                                                                                                             | *string*                                                                                                                 | :heavy_check_mark:                                                                                                       | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the Conference resource(s) to update. |
| `sid`                                                                                                                    | *string*                                                                                                                 | :heavy_check_mark:                                                                                                       | The Twilio-provided string that uniquely identifies the Conference resource to update                                    |
| `requestBody`                                                                                                            | [operations.UpdateConferenceUpdateConferenceRequest](../../models/operations/updateconferenceupdateconferencerequest.md) | :heavy_minus_sign:                                                                                                       | N/A                                                                                                                      |