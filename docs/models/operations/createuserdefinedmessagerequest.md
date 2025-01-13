# CreateUserDefinedMessageRequest

## Example Usage

```typescript
import { CreateUserDefinedMessageRequest } from "twilio-sdk/models/operations";

let value: CreateUserDefinedMessageRequest = {
  accountSid: "<id>",
  callSid: "<id>",
};
```

## Fields

| Field                                                                                                                                                    | Type                                                                                                                                                     | Required                                                                                                                                                 | Description                                                                                                                                              |
| -------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                                                                             | *string*                                                                                                                                                 | :heavy_check_mark:                                                                                                                                       | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created User Defined Message.                                                 |
| `callSid`                                                                                                                                                | *string*                                                                                                                                                 | :heavy_check_mark:                                                                                                                                       | The SID of the [Call](https://www.twilio.com/docs/voice/api/call-resource) the User Defined Message is associated with.                                  |
| `requestBody`                                                                                                                                            | [operations.CreateUserDefinedMessageCreateUserDefinedMessageRequest](../../models/operations/createuserdefinedmessagecreateuserdefinedmessagerequest.md) | :heavy_minus_sign:                                                                                                                                       | N/A                                                                                                                                                      |