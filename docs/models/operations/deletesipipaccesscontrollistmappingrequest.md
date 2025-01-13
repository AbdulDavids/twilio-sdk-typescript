# DeleteSipIpAccessControlListMappingRequest

## Example Usage

```typescript
import { DeleteSipIpAccessControlListMappingRequest } from "twilio-sdk/models/operations";

let value: DeleteSipIpAccessControlListMappingRequest = {
  accountSid: "<id>",
  domainSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                  | Type                                                                   | Required                                                               | Description                                                            |
| ---------------------------------------------------------------------- | ---------------------------------------------------------------------- | ---------------------------------------------------------------------- | ---------------------------------------------------------------------- |
| `accountSid`                                                           | *string*                                                               | :heavy_check_mark:                                                     | The unique id of the Account that is responsible for this resource.    |
| `domainSid`                                                            | *string*                                                               | :heavy_check_mark:                                                     | A 34 character string that uniquely identifies the SIP domain.         |
| `sid`                                                                  | *string*                                                               | :heavy_check_mark:                                                     | A 34 character string that uniquely identifies the resource to delete. |