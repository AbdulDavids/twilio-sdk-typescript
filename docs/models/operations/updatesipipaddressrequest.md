# UpdateSipIpAddressRequest

## Example Usage

```typescript
import { UpdateSipIpAddressRequest } from "twilio-sdk/models/operations";

let value: UpdateSipIpAddressRequest = {
  accountSid: "<id>",
  ipAccessControlListSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                                            | Type                                                                                                                             | Required                                                                                                                         | Description                                                                                                                      |
| -------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                                                     | *string*                                                                                                                         | :heavy_check_mark:                                                                                                               | The unique id of the [Account](https://www.twilio.com/docs/iam/api/account) responsible for this resource.                       |
| `ipAccessControlListSid`                                                                                                         | *string*                                                                                                                         | :heavy_check_mark:                                                                                                               | The IpAccessControlList Sid that identifies the IpAddress resources to update.                                                   |
| `sid`                                                                                                                            | *string*                                                                                                                         | :heavy_check_mark:                                                                                                               | A 34 character string that identifies the IpAddress resource to update.                                                          |
| `requestBody`                                                                                                                    | [operations.UpdateSipIpAddressUpdateSipIpAddressRequest](../../models/operations/updatesipipaddressupdatesipipaddressrequest.md) | :heavy_minus_sign:                                                                                                               | N/A                                                                                                                              |