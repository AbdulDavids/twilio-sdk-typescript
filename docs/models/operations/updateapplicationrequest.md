# UpdateApplicationRequest

## Example Usage

```typescript
import { UpdateApplicationRequest } from "twilio-sdk/models/operations";

let value: UpdateApplicationRequest = {
  accountSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                                        | Type                                                                                                                         | Required                                                                                                                     | Description                                                                                                                  |
| ---------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                                                 | *string*                                                                                                                     | :heavy_check_mark:                                                                                                           | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the Application resources to update.      |
| `sid`                                                                                                                        | *string*                                                                                                                     | :heavy_check_mark:                                                                                                           | The Twilio-provided string that uniquely identifies the Application resource to update.                                      |
| `requestBody`                                                                                                                | [operations.UpdateApplicationUpdateApplicationRequest](../../models/operations/updateapplicationupdateapplicationrequest.md) | :heavy_minus_sign:                                                                                                           | N/A                                                                                                                          |