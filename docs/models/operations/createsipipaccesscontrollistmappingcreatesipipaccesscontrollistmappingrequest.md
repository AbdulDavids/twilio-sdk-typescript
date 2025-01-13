# CreateSipIpAccessControlListMappingCreateSipIpAccessControlListMappingRequest

## Example Usage

```typescript
import { CreateSipIpAccessControlListMappingCreateSipIpAccessControlListMappingRequest } from "twilio-sdk/models/operations";

let value:
  CreateSipIpAccessControlListMappingCreateSipIpAccessControlListMappingRequest =
    {
      ipAccessControlListSid: "<id>",
    };
```

## Fields

| Field                                                                 | Type                                                                  | Required                                                              | Description                                                           |
| --------------------------------------------------------------------- | --------------------------------------------------------------------- | --------------------------------------------------------------------- | --------------------------------------------------------------------- |
| `ipAccessControlListSid`                                              | *string*                                                              | :heavy_check_mark:                                                    | The unique id of the IP access control list to map to the SIP domain. |