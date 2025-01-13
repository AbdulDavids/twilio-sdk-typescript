# FetchConferenceRequest

## Example Usage

```typescript
import { FetchConferenceRequest } from "twilio-sdk/models/operations";

let value: FetchConferenceRequest = {
  accountSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                                   | Type                                                                                                                    | Required                                                                                                                | Description                                                                                                             |
| ----------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                                            | *string*                                                                                                                | :heavy_check_mark:                                                                                                      | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the Conference resource(s) to fetch. |
| `sid`                                                                                                                   | *string*                                                                                                                | :heavy_check_mark:                                                                                                      | The Twilio-provided string that uniquely identifies the Conference resource to fetch                                    |