# DeleteApplicationRequest

## Example Usage

```typescript
import { DeleteApplicationRequest } from "twilio-sdk/models/operations";

let value: DeleteApplicationRequest = {
  accountSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                                   | Type                                                                                                                    | Required                                                                                                                | Description                                                                                                             |
| ----------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                                            | *string*                                                                                                                | :heavy_check_mark:                                                                                                      | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the Application resources to delete. |
| `sid`                                                                                                                   | *string*                                                                                                                | :heavy_check_mark:                                                                                                      | The Twilio-provided string that uniquely identifies the Application resource to delete.                                 |