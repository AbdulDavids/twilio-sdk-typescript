# FetchAddressRequest

## Example Usage

```typescript
import { FetchAddressRequest } from "twilio-sdk/models/operations";

let value: FetchAddressRequest = {
  accountSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                                        | Type                                                                                                                         | Required                                                                                                                     | Description                                                                                                                  |
| ---------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                                                 | *string*                                                                                                                     | :heavy_check_mark:                                                                                                           | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that is responsible for the Address resource to fetch. |
| `sid`                                                                                                                        | *string*                                                                                                                     | :heavy_check_mark:                                                                                                           | The Twilio-provided string that uniquely identifies the Address resource to fetch.                                           |