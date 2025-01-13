# ApiV2010AccountCallUserDefinedMessage

## Example Usage

```typescript
import { ApiV2010AccountCallUserDefinedMessage } from "twilio-sdk/models/components";

let value: ApiV2010AccountCallUserDefinedMessage = {};
```

## Fields

| Field                                                                                                                   | Type                                                                                                                    | Required                                                                                                                | Description                                                                                                             |
| ----------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                                            | *string*                                                                                                                | :heavy_minus_sign:                                                                                                      | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created User Defined Message.                |
| `callSid`                                                                                                               | *string*                                                                                                                | :heavy_minus_sign:                                                                                                      | The SID of the [Call](https://www.twilio.com/docs/voice/api/call-resource) the User Defined Message is associated with. |
| `sid`                                                                                                                   | *string*                                                                                                                | :heavy_minus_sign:                                                                                                      | The SID that uniquely identifies this User Defined Message.                                                             |
| `dateCreated`                                                                                                           | *string*                                                                                                                | :heavy_minus_sign:                                                                                                      | The date that this User Defined Message was created, given in RFC 2822 format.                                          |