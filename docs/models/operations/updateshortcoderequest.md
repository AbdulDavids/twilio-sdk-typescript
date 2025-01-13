# UpdateShortCodeRequest

## Example Usage

```typescript
import { UpdateShortCodeRequest } from "twilio-sdk/models/operations";

let value: UpdateShortCodeRequest = {
  accountSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                                   | Type                                                                                                                    | Required                                                                                                                | Description                                                                                                             |
| ----------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                                            | *string*                                                                                                                | :heavy_check_mark:                                                                                                      | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the ShortCode resource(s) to update. |
| `sid`                                                                                                                   | *string*                                                                                                                | :heavy_check_mark:                                                                                                      | The Twilio-provided string that uniquely identifies the ShortCode resource to update                                    |
| `requestBody`                                                                                                           | [operations.UpdateShortCodeUpdateShortCodeRequest](../../models/operations/updateshortcodeupdateshortcoderequest.md)    | :heavy_minus_sign:                                                                                                      | N/A                                                                                                                     |