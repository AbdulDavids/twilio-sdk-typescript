# UpdateSipDomainRequest

## Example Usage

```typescript
import { UpdateSipDomainRequest } from "twilio-sdk/models/operations";

let value: UpdateSipDomainRequest = {
  accountSid: "<id>",
  sid: "<id>",
};
```

## Fields

| Field                                                                                                                | Type                                                                                                                 | Required                                                                                                             | Description                                                                                                          |
| -------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                                         | *string*                                                                                                             | :heavy_check_mark:                                                                                                   | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the SipDomain resource to update. |
| `sid`                                                                                                                | *string*                                                                                                             | :heavy_check_mark:                                                                                                   | The Twilio-provided string that uniquely identifies the SipDomain resource to update.                                |
| `requestBody`                                                                                                        | [operations.UpdateSipDomainUpdateSipDomainRequest](../../models/operations/updatesipdomainupdatesipdomainrequest.md) | :heavy_minus_sign:                                                                                                   | N/A                                                                                                                  |