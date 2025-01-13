# FetchSipIpAddressRequest

## Example Usage

```typescript
import { FetchSipIpAddressRequest } from "twilio-sdk/models/operations";

let value: FetchSipIpAddressRequest = {
  accountSid: "<id>",
  ipAccessControlListSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                      | Type                                                                                                       | Required                                                                                                   | Description                                                                                                |
| ---------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                               | *string*                                                                                                   | :heavy_check_mark:                                                                                         | The unique id of the [Account](https://www.twilio.com/docs/iam/api/account) responsible for this resource. |
| `ipAccessControlListSid`                                                                                   | *string*                                                                                                   | :heavy_check_mark:                                                                                         | The IpAccessControlList Sid that identifies the IpAddress resources to fetch.                              |
| `sid`                                                                                                      | *string*                                                                                                   | :heavy_check_mark:                                                                                         | A 34 character string that uniquely identifies the IpAddress resource to fetch.                            |