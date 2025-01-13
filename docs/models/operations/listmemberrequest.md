# ListMemberRequest

## Example Usage

```typescript
import { ListMemberRequest } from "twilio-sdk/models/operations";

let value: ListMemberRequest = {
  accountSid: "<id>",
  queueSid: "<id>",
};
```

## Fields

| Field                                                                                                              | Type                                                                                                               | Required                                                                                                           | Description                                                                                                        |
| ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------ |
| `accountSid`                                                                                                       | *string*                                                                                                           | :heavy_check_mark:                                                                                                 | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the Member resource(s) to read. |
| `queueSid`                                                                                                         | *string*                                                                                                           | :heavy_check_mark:                                                                                                 | The SID of the Queue in which to find the members                                                                  |
| `pageSize`                                                                                                         | *number*                                                                                                           | :heavy_minus_sign:                                                                                                 | How many resources to return in each list page. The default is 50, and the maximum is 1000.                        |
| `page`                                                                                                             | *number*                                                                                                           | :heavy_minus_sign:                                                                                                 | The page index. This value is simply for client state.                                                             |
| `pageToken`                                                                                                        | *string*                                                                                                           | :heavy_minus_sign:                                                                                                 | The page token. This is provided by the API.                                                                       |