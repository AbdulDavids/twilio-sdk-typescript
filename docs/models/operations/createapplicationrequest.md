# CreateApplicationRequest

## Example Usage

```typescript
import { CreateApplicationRequest } from "twilio-sdk/models/operations";

let value: CreateApplicationRequest = {
  accountSid: "<id>",
};
```

## Fields

| Field                                                                                                                        | Type                                                                                                                         | Required                                                                                                                     | Description                                                                                                                  |
| ---------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                                                 | *string*                                                                                                                     | :heavy_check_mark:                                                                                                           | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that will create the resource.                         |
| `requestBody`                                                                                                                | [operations.CreateApplicationCreateApplicationRequest](../../models/operations/createapplicationcreateapplicationrequest.md) | :heavy_minus_sign:                                                                                                           | N/A                                                                                                                          |