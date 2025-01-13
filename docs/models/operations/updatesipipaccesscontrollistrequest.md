# UpdateSipIpAccessControlListRequest

## Example Usage

```typescript
import { UpdateSipIpAccessControlListRequest } from "twilio-sdk/models/operations";

let value: UpdateSipIpAccessControlListRequest = {
  accountSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                                                                                    | Type                                                                                                                                                                     | Required                                                                                                                                                                 | Description                                                                                                                                                              |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `accountSid`                                                                                                                                                             | *string*                                                                                                                                                                 | :heavy_check_mark:                                                                                                                                                       | The unique id of the [Account](https://www.twilio.com/docs/iam/api/account) responsible for this resource.                                                               |
| `sid`                                                                                                                                                                    | *string*                                                                                                                                                                 | :heavy_check_mark:                                                                                                                                                       | A 34 character string that uniquely identifies the resource to udpate.                                                                                                   |
| `requestBody`                                                                                                                                                            | [operations.UpdateSipIpAccessControlListUpdateSipIpAccessControlListRequest](../../models/operations/updatesipipaccesscontrollistupdatesipipaccesscontrollistrequest.md) | :heavy_minus_sign:                                                                                                                                                       | N/A                                                                                                                                                                      |