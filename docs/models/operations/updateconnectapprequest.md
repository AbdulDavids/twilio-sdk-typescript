# UpdateConnectAppRequest

## Example Usage

```typescript
import { UpdateConnectAppRequest } from "twilio-sdk/models/operations";

let value: UpdateConnectAppRequest = {
  accountSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                                    | Type                                                                                                                     | Required                                                                                                                 | Description                                                                                                              |
| ------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------ |
| `accountSid`                                                                                                             | *string*                                                                                                                 | :heavy_check_mark:                                                                                                       | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the ConnectApp resources to update.   |
| `sid`                                                                                                                    | *string*                                                                                                                 | :heavy_check_mark:                                                                                                       | The Twilio-provided string that uniquely identifies the ConnectApp resource to update.                                   |
| `requestBody`                                                                                                            | [operations.UpdateConnectAppUpdateConnectAppRequest](../../models/operations/updateconnectappupdateconnectapprequest.md) | :heavy_minus_sign:                                                                                                       | N/A                                                                                                                      |