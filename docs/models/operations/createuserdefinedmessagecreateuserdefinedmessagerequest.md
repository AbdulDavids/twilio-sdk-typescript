# CreateUserDefinedMessageCreateUserDefinedMessageRequest

## Example Usage

```typescript
import { CreateUserDefinedMessageCreateUserDefinedMessageRequest } from "twilio-sdk/models/operations";

let value: CreateUserDefinedMessageCreateUserDefinedMessageRequest = {
  content: "<value>",
};
```

## Fields

| Field                                                                                                                          | Type                                                                                                                           | Required                                                                                                                       | Description                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------ |
| `content`                                                                                                                      | *string*                                                                                                                       | :heavy_check_mark:                                                                                                             | The User Defined Message in the form of URL-encoded JSON string.                                                               |
| `idempotencyKey`                                                                                                               | *string*                                                                                                                       | :heavy_minus_sign:                                                                                                             | A unique string value to identify API call. This should be a unique string value per API call and can be a randomly generated. |