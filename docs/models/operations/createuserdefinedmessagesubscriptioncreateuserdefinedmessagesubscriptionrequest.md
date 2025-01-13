# CreateUserDefinedMessageSubscriptionCreateUserDefinedMessageSubscriptionRequest

## Example Usage

```typescript
import { CreateUserDefinedMessageSubscriptionCreateUserDefinedMessageSubscriptionRequest } from "twilio-sdk/models/operations";

let value:
  CreateUserDefinedMessageSubscriptionCreateUserDefinedMessageSubscriptionRequest =
    {
      callback: "https://strict-pressure.com",
    };
```

## Fields

| Field                                                                                                                                                          | Type                                                                                                                                                           | Required                                                                                                                                                       | Description                                                                                                                                                    |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `callback`                                                                                                                                                     | *string*                                                                                                                                                       | :heavy_check_mark:                                                                                                                                             | The URL we should call using the `method` to send user defined events to your application. URLs must contain a valid hostname (underscores are not permitted). |
| `idempotencyKey`                                                                                                                                               | *string*                                                                                                                                                       | :heavy_minus_sign:                                                                                                                                             | A unique string value to identify API call. This should be a unique string value per API call and can be a randomly generated.                                 |
| `method`                                                                                                                                                       | [operations.CreateUserDefinedMessageSubscriptionMethod](../../models/operations/createuserdefinedmessagesubscriptionmethod.md)                                 | :heavy_minus_sign:                                                                                                                                             | The HTTP method Twilio will use when requesting the above `Url`. Either `GET` or `POST`. Default is `POST`.                                                    |