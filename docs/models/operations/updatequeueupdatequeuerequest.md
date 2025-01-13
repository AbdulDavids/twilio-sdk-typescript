# UpdateQueueUpdateQueueRequest

## Example Usage

```typescript
import { UpdateQueueUpdateQueueRequest } from "twilio-sdk/models/operations";

let value: UpdateQueueUpdateQueueRequest = {};
```

## Fields

| Field                                                                                                | Type                                                                                                 | Required                                                                                             | Description                                                                                          |
| ---------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- |
| `friendlyName`                                                                                       | *string*                                                                                             | :heavy_minus_sign:                                                                                   | A descriptive string that you created to describe this resource. It can be up to 64 characters long. |
| `maxSize`                                                                                            | *number*                                                                                             | :heavy_minus_sign:                                                                                   | The maximum number of calls allowed to be in the queue. The default is 1000. The maximum is 5000.    |