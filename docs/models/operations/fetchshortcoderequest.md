# FetchShortCodeRequest

## Example Usage

```typescript
import { FetchShortCodeRequest } from "twilio-sdk/models/operations";

let value: FetchShortCodeRequest = {
  accountSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                                  | Type                                                                                                                   | Required                                                                                                               | Description                                                                                                            |
| ---------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                                           | *string*                                                                                                               | :heavy_check_mark:                                                                                                     | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the ShortCode resource(s) to fetch. |
| `sid`                                                                                                                  | *string*                                                                                                               | :heavy_check_mark:                                                                                                     | The Twilio-provided string that uniquely identifies the ShortCode resource to fetch                                    |