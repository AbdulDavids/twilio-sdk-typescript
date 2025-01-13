# ListSipCredentialRequest

## Example Usage

```typescript
import { ListSipCredentialRequest } from "twilio-sdk/models/operations";

let value: ListSipCredentialRequest = {
  accountSid: "<id>",
  credentialListSid: "<id>",
};
```

## Fields

| Field                                                                                       | Type                                                                                        | Required                                                                                    | Description                                                                                 |
| ------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                | *string*                                                                                    | :heavy_check_mark:                                                                          | The unique id of the Account that is responsible for this resource.                         |
| `credentialListSid`                                                                         | *string*                                                                                    | :heavy_check_mark:                                                                          | The unique id that identifies the credential list that contains the desired credentials.    |
| `pageSize`                                                                                  | *number*                                                                                    | :heavy_minus_sign:                                                                          | How many resources to return in each list page. The default is 50, and the maximum is 1000. |
| `page`                                                                                      | *number*                                                                                    | :heavy_minus_sign:                                                                          | The page index. This value is simply for client state.                                      |
| `pageToken`                                                                                 | *string*                                                                                    | :heavy_minus_sign:                                                                          | The page token. This is provided by the API.                                                |