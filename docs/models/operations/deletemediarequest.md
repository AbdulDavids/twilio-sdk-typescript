# DeleteMediaRequest

## Example Usage

```typescript
import { DeleteMediaRequest } from "twilio-sdk/models/operations";

let value: DeleteMediaRequest = {
  accountSid: "<id>",
  messageSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                             | Type                                                                                                              | Required                                                                                                          | Description                                                                                                       |
| ----------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                                      | *string*                                                                                                          | :heavy_check_mark:                                                                                                | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that is associated with the Media resource. |
| `messageSid`                                                                                                      | *string*                                                                                                          | :heavy_check_mark:                                                                                                | The SID of the Message resource that is associated with the Media resource.                                       |
| `sid`                                                                                                             | *string*                                                                                                          | :heavy_check_mark:                                                                                                | The unique identifier of the to-be-deleted Media resource.                                                        |