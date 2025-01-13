# DeleteIncomingPhoneNumberRequest

## Example Usage

```typescript
import { DeleteIncomingPhoneNumberRequest } from "twilio-sdk/models/operations";

let value: DeleteIncomingPhoneNumberRequest = {
  accountSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                                           | Type                                                                                                                            | Required                                                                                                                        | Description                                                                                                                     |
| ------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                                                    | *string*                                                                                                                        | :heavy_check_mark:                                                                                                              | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the IncomingPhoneNumber resources to delete. |
| `sid`                                                                                                                           | *string*                                                                                                                        | :heavy_check_mark:                                                                                                              | The Twilio-provided string that uniquely identifies the IncomingPhoneNumber resource to delete.                                 |