# UpdateSipCredentialUpdateSipCredentialRequest

## Example Usage

```typescript
import { UpdateSipCredentialUpdateSipCredentialRequest } from "twilio-sdk/models/operations";

let value: UpdateSipCredentialUpdateSipCredentialRequest = {};
```

## Fields

| Field                                                                                                                                                                                             | Type                                                                                                                                                                                              | Required                                                                                                                                                                                          | Description                                                                                                                                                                                       |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `password`                                                                                                                                                                                        | *string*                                                                                                                                                                                          | :heavy_minus_sign:                                                                                                                                                                                | The password that the username will use when authenticating SIP requests. The password must be a minimum of 12 characters, contain at least 1 digit, and have mixed case. (eg `IWasAtSignal2018`) |