# ListCallEventRequest

## Example Usage

```typescript
import { ListCallEventRequest } from "twilio-sdk/models/operations";

let value: ListCallEventRequest = {
  accountSid: "<id>",
  callSid: "<id>",
};
```

## Fields

| Field                                                                                       | Type                                                                                        | Required                                                                                    | Description                                                                                 |
| ------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                | *string*                                                                                    | :heavy_check_mark:                                                                          | The unique SID identifier of the Account.                                                   |
| `callSid`                                                                                   | *string*                                                                                    | :heavy_check_mark:                                                                          | The unique SID identifier of the Call.                                                      |
| `pageSize`                                                                                  | *number*                                                                                    | :heavy_minus_sign:                                                                          | How many resources to return in each list page. The default is 50, and the maximum is 1000. |
| `page`                                                                                      | *number*                                                                                    | :heavy_minus_sign:                                                                          | The page index. This value is simply for client state.                                      |
| `pageToken`                                                                                 | *string*                                                                                    | :heavy_minus_sign:                                                                          | The page token. This is provided by the API.                                                |