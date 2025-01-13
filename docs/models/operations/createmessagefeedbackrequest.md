# CreateMessageFeedbackRequest

## Example Usage

```typescript
import { CreateMessageFeedbackRequest } from "twilio-sdk/models/operations";

let value: CreateMessageFeedbackRequest = {
  accountSid: "<id>",
  messageSid: "<id>",
};
```

## Fields

| Field                                                                                                                                           | Type                                                                                                                                            | Required                                                                                                                                        | Description                                                                                                                                     |
| ----------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                                                                    | *string*                                                                                                                                        | :heavy_check_mark:                                                                                                                              | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) associated with the Message resource for which to create MessageFeedback. |
| `messageSid`                                                                                                                                    | *string*                                                                                                                                        | :heavy_check_mark:                                                                                                                              | The SID of the Message resource for which to create MessageFeedback.                                                                            |
| `requestBody`                                                                                                                                   | [operations.CreateMessageFeedbackCreateMessageFeedbackRequest](../../models/operations/createmessagefeedbackcreatemessagefeedbackrequest.md)    | :heavy_minus_sign:                                                                                                                              | N/A                                                                                                                                             |