# CreateSipIpAddressRequest

## Example Usage

```typescript
import { CreateSipIpAddressRequest } from "twilio-sdk/models/operations";

let value: CreateSipIpAddressRequest = {
  accountSid: "<id>",
  ipAccessControlListSid: "<id>",
};
```

## Fields

| Field                                                                                                                            | Type                                                                                                                             | Required                                                                                                                         | Description                                                                                                                      |
| -------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                                                     | *string*                                                                                                                         | :heavy_check_mark:                                                                                                               | The unique id of the [Account](https://www.twilio.com/docs/iam/api/account) responsible for this resource.                       |
| `ipAccessControlListSid`                                                                                                         | *string*                                                                                                                         | :heavy_check_mark:                                                                                                               | The IpAccessControlList Sid with which to associate the created IpAddress resource.                                              |
| `requestBody`                                                                                                                    | [operations.CreateSipIpAddressCreateSipIpAddressRequest](../../models/operations/createsipipaddresscreatesipipaddressrequest.md) | :heavy_minus_sign:                                                                                                               | N/A                                                                                                                              |