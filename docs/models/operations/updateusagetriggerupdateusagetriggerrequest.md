# UpdateUsageTriggerUpdateUsageTriggerRequest

## Example Usage

```typescript
import { UpdateUsageTriggerUpdateUsageTriggerRequest } from "twilio-sdk/models/operations";

let value: UpdateUsageTriggerUpdateUsageTriggerRequest = {};
```

## Fields

| Field                                                                                                    | Type                                                                                                     | Required                                                                                                 | Description                                                                                              |
| -------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------- |
| `callbackMethod`                                                                                         | [operations.CallbackMethod](../../models/operations/callbackmethod.md)                                   | :heavy_minus_sign:                                                                                       | The HTTP method we should use to call `callback_url`. Can be: `GET` or `POST` and the default is `POST`. |
| `callbackUrl`                                                                                            | *string*                                                                                                 | :heavy_minus_sign:                                                                                       | The URL we should call using `callback_method` when the trigger fires.                                   |
| `friendlyName`                                                                                           | *string*                                                                                                 | :heavy_minus_sign:                                                                                       | A descriptive string that you create to describe the resource. It can be up to 64 characters long.       |