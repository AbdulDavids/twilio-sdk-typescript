# CreateTokenRequest

## Example Usage

```typescript
import { CreateTokenRequest } from "twilio-sdk/models/operations";

let value: CreateTokenRequest = {
  accountSid: "<id>",
};
```

## Fields

| Field                                                                                                | Type                                                                                                 | Required                                                                                             | Description                                                                                          |
| ---------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                         | *string*                                                                                             | :heavy_check_mark:                                                                                   | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that will create the resource. |
| `requestBody`                                                                                        | [operations.CreateTokenCreateTokenRequest](../../models/operations/createtokencreatetokenrequest.md) | :heavy_minus_sign:                                                                                   | N/A                                                                                                  |