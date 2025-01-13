# FetchAuthorizedConnectAppRequest

## Example Usage

```typescript
import { FetchAuthorizedConnectAppRequest } from "twilio-sdk/models/operations";

let value: FetchAuthorizedConnectAppRequest = {
  accountSid: "<id>",
  connectAppSid: "<id>",
};
```

## Fields

| Field                                                                                                                          | Type                                                                                                                           | Required                                                                                                                       | Description                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------ |
| `accountSid`                                                                                                                   | *string*                                                                                                                       | :heavy_check_mark:                                                                                                             | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the AuthorizedConnectApp resource to fetch. |
| `connectAppSid`                                                                                                                | *string*                                                                                                                       | :heavy_check_mark:                                                                                                             | The SID of the Connect App to fetch.                                                                                           |