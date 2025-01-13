# UpdateKeyRequest

## Example Usage

```typescript
import { UpdateKeyRequest } from "twilio-sdk/models/operations";

let value: UpdateKeyRequest = {
  accountSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                           | Type                                                                                                            | Required                                                                                                        | Description                                                                                                     |
| --------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                                    | *string*                                                                                                        | :heavy_check_mark:                                                                                              | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the Key resources to update. |
| `sid`                                                                                                           | *string*                                                                                                        | :heavy_check_mark:                                                                                              | The Twilio-provided string that uniquely identifies the Key resource to update.                                 |
| `requestBody`                                                                                                   | [operations.UpdateKeyUpdateKeyRequest](../../models/operations/updatekeyupdatekeyrequest.md)                    | :heavy_minus_sign:                                                                                              | N/A                                                                                                             |