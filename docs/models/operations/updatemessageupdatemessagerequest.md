# UpdateMessageUpdateMessageRequest

## Example Usage

```typescript
import { UpdateMessageUpdateMessageRequest } from "twilio-sdk/models/operations";

let value: UpdateMessageUpdateMessageRequest = {};
```

## Fields

| Field                                                                                                                           | Type                                                                                                                            | Required                                                                                                                        | Description                                                                                                                     |
| ------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------- |
| `body`                                                                                                                          | *string*                                                                                                                        | :heavy_minus_sign:                                                                                                              | The new `body` of the Message resource. To redact the text content of a Message, this parameter's value must be an empty string |
| `status`                                                                                                                        | [components.MessageEnumUpdateStatus](../../models/components/messageenumupdatestatus.md)                                        | :heavy_minus_sign:                                                                                                              | N/A                                                                                                                             |