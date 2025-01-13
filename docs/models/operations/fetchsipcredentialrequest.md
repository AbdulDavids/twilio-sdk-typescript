# FetchSipCredentialRequest

## Example Usage

```typescript
import { FetchSipCredentialRequest } from "twilio-sdk/models/operations";

let value: FetchSipCredentialRequest = {
  accountSid: "<id>",
  credentialListSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                   | Type                                                                                    | Required                                                                                | Description                                                                             |
| --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- |
| `accountSid`                                                                            | *string*                                                                                | :heavy_check_mark:                                                                      | The unique id of the Account that is responsible for this resource.                     |
| `credentialListSid`                                                                     | *string*                                                                                | :heavy_check_mark:                                                                      | The unique id that identifies the credential list that contains the desired credential. |
| `sid`                                                                                   | *string*                                                                                | :heavy_check_mark:                                                                      | The unique id that identifies the resource to fetch.                                    |