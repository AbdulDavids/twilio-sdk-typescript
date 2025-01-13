# FetchCallRequest

## Example Usage

```typescript
import { FetchCallRequest } from "twilio-sdk/models/operations";

let value: FetchCallRequest = {
  accountSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                             | Type                                                                                                              | Required                                                                                                          | Description                                                                                                       |
| ----------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                                      | *string*                                                                                                          | :heavy_check_mark:                                                                                                | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the Call resource(s) to fetch. |
| `sid`                                                                                                             | *string*                                                                                                          | :heavy_check_mark:                                                                                                | The SID of the Call resource to fetch.                                                                            |