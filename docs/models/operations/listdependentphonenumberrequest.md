# ListDependentPhoneNumberRequest

## Example Usage

```typescript
import { ListDependentPhoneNumberRequest } from "twilio-sdk/models/operations";

let value: ListDependentPhoneNumberRequest = {
  accountSid: "<id>",
  addressSid: "<id>",
};
```

## Fields

| Field                                                                                                                          | Type                                                                                                                           | Required                                                                                                                       | Description                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------ |
| `accountSid`                                                                                                                   | *string*                                                                                                                       | :heavy_check_mark:                                                                                                             | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the DependentPhoneNumber resources to read. |
| `addressSid`                                                                                                                   | *string*                                                                                                                       | :heavy_check_mark:                                                                                                             | The SID of the Address resource associated with the phone number.                                                              |
| `pageSize`                                                                                                                     | *number*                                                                                                                       | :heavy_minus_sign:                                                                                                             | How many resources to return in each list page. The default is 50, and the maximum is 1000.                                    |
| `page`                                                                                                                         | *number*                                                                                                                       | :heavy_minus_sign:                                                                                                             | The page index. This value is simply for client state.                                                                         |
| `pageToken`                                                                                                                    | *string*                                                                                                                       | :heavy_minus_sign:                                                                                                             | The page token. This is provided by the API.                                                                                   |