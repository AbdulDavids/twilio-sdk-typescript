# FetchUsageTriggerRequest

## Example Usage

```typescript
import { FetchUsageTriggerRequest } from "twilio-sdk/models/operations";

let value: FetchUsageTriggerRequest = {
  accountSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                                  | Type                                                                                                                   | Required                                                                                                               | Description                                                                                                            |
| ---------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                                           | *string*                                                                                                               | :heavy_check_mark:                                                                                                     | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the UsageTrigger resource to fetch. |
| `sid`                                                                                                                  | *string*                                                                                                               | :heavy_check_mark:                                                                                                     | The Twilio-provided string that uniquely identifies the UsageTrigger resource to fetch.                                |