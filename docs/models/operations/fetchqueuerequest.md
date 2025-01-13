# FetchQueueRequest

## Example Usage

```typescript
import { FetchQueueRequest } from "twilio-sdk/models/operations";

let value: FetchQueueRequest = {
  accountSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                           | Type                                                                                                            | Required                                                                                                        | Description                                                                                                     |
| --------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                                    | *string*                                                                                                        | :heavy_check_mark:                                                                                              | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the Queue resource to fetch. |
| `sid`                                                                                                           | *string*                                                                                                        | :heavy_check_mark:                                                                                              | The Twilio-provided string that uniquely identifies the Queue resource to fetch                                 |