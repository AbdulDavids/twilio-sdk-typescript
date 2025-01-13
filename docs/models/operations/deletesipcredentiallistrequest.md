# DeleteSipCredentialListRequest

## Example Usage

```typescript
import { DeleteSipCredentialListRequest } from "twilio-sdk/models/operations";

let value: DeleteSipCredentialListRequest = {
  accountSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                               | Type                                                                | Required                                                            | Description                                                         |
| ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- |
| `accountSid`                                                        | *string*                                                            | :heavy_check_mark:                                                  | The unique id of the Account that is responsible for this resource. |
| `sid`                                                               | *string*                                                            | :heavy_check_mark:                                                  | The credential list Sid that uniquely identifies this resource      |