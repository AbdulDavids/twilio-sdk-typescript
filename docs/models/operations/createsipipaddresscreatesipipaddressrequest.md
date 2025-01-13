# CreateSipIpAddressCreateSipIpAddressRequest

## Example Usage

```typescript
import { CreateSipIpAddressCreateSipIpAddressRequest } from "twilio-sdk/models/operations";

let value: CreateSipIpAddressCreateSipIpAddressRequest = {
  friendlyName: "<value>",
  ipAddress: "155.4.77.169",
};
```

## Fields

| Field                                                                                                                                                                       | Type                                                                                                                                                                        | Required                                                                                                                                                                    | Description                                                                                                                                                                 |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `friendlyName`                                                                                                                                                              | *string*                                                                                                                                                                    | :heavy_check_mark:                                                                                                                                                          | A human readable descriptive text for this resource, up to 255 characters long.                                                                                             |
| `ipAddress`                                                                                                                                                                 | *string*                                                                                                                                                                    | :heavy_check_mark:                                                                                                                                                          | An IP address in dotted decimal notation from which you want to accept traffic. Any SIP requests from this IP address will be allowed by Twilio. IPv4 only supported today. |
| `cidrPrefixLength`                                                                                                                                                          | *number*                                                                                                                                                                    | :heavy_minus_sign:                                                                                                                                                          | An integer representing the length of the CIDR prefix to use with this IP address when accepting traffic. By default the entire IP address is used.                         |