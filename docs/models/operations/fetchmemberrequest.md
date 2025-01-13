# FetchMemberRequest

## Example Usage

```typescript
import { FetchMemberRequest } from "twilio-sdk/models/operations";

let value: FetchMemberRequest = {
  accountSid: "<id>",
  queueSid: "<id>",
  callSid: "<id>",
};
```

## Fields

| Field                                                                                                               | Type                                                                                                                | Required                                                                                                            | Description                                                                                                         |
| ------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                                        | *string*                                                                                                            | :heavy_check_mark:                                                                                                  | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the Member resource(s) to fetch. |
| `queueSid`                                                                                                          | *string*                                                                                                            | :heavy_check_mark:                                                                                                  | The SID of the Queue in which to find the members to fetch.                                                         |
| `callSid`                                                                                                           | *string*                                                                                                            | :heavy_check_mark:                                                                                                  | The [Call](https://www.twilio.com/docs/voice/api/call-resource) SID of the resource(s) to fetch.                    |