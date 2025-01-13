# CreateSipAuthCallsIpAccessControlListMappingCreateSipAuthCallsIpAccessControlListMappingRequest

## Example Usage

```typescript
import {
  CreateSipAuthCallsIpAccessControlListMappingCreateSipAuthCallsIpAccessControlListMappingRequest,
} from "twilio-sdk/models/operations";

let value:
  CreateSipAuthCallsIpAccessControlListMappingCreateSipAuthCallsIpAccessControlListMappingRequest =
    {
      ipAccessControlListSid: "<id>",
    };
```

## Fields

| Field                                                                 | Type                                                                  | Required                                                              | Description                                                           |
| --------------------------------------------------------------------- | --------------------------------------------------------------------- | --------------------------------------------------------------------- | --------------------------------------------------------------------- |
| `ipAccessControlListSid`                                              | *string*                                                              | :heavy_check_mark:                                                    | The SID of the IpAccessControlList resource to map to the SIP domain. |