# FetchSipIpAccessControlListMappingRequest

## Example Usage

```typescript
import { FetchSipIpAccessControlListMappingRequest } from "twilio-sdk/models/operations";

let value: FetchSipIpAccessControlListMappingRequest = {
  accountSid: "<id>",
  domainSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                 | Type                                                                  | Required                                                              | Description                                                           |
| --------------------------------------------------------------------- | --------------------------------------------------------------------- | --------------------------------------------------------------------- | --------------------------------------------------------------------- |
| `accountSid`                                                          | *string*                                                              | :heavy_check_mark:                                                    | The unique id of the Account that is responsible for this resource.   |
| `domainSid`                                                           | *string*                                                              | :heavy_check_mark:                                                    | A 34 character string that uniquely identifies the SIP domain.        |
| `sid`                                                                 | *string*                                                              | :heavy_check_mark:                                                    | A 34 character string that uniquely identifies the resource to fetch. |