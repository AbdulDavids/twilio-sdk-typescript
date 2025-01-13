# FetchApplicationRequest

## Example Usage

```typescript
import { FetchApplicationRequest } from "twilio-sdk/models/operations";

let value: FetchApplicationRequest = {
  accountSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                                 | Type                                                                                                                  | Required                                                                                                              | Description                                                                                                           |
| --------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                                          | *string*                                                                                                              | :heavy_check_mark:                                                                                                    | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the Application resource to fetch. |
| `sid`                                                                                                                 | *string*                                                                                                              | :heavy_check_mark:                                                                                                    | The Twilio-provided string that uniquely identifies the Application resource to fetch.                                |