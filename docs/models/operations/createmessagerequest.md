# CreateMessageRequest

## Example Usage

```typescript
import { CreateMessageRequest } from "twilio-sdk/models/operations";

let value: CreateMessageRequest = {
  accountSid: "<id>",
};
```

## Fields

| Field                                                                                                        | Type                                                                                                         | Required                                                                                                     | Description                                                                                                  |
| ------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------ |
| `accountSid`                                                                                                 | *string*                                                                                                     | :heavy_check_mark:                                                                                           | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) creating the Message resource.         |
| `requestBody`                                                                                                | [operations.CreateMessageCreateMessageRequest](../../models/operations/createmessagecreatemessagerequest.md) | :heavy_minus_sign:                                                                                           | N/A                                                                                                          |