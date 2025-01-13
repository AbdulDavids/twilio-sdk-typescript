# ApiV2010AccountAvailablePhoneNumberCountryAvailablePhoneNumberSharedCostCapabilities

The set of Boolean properties that indicate whether a phone number can receive calls or messages.  Capabilities are: `Voice`, `SMS`, and `MMS` and each capability can be: `true` or `false`.

## Example Usage

```typescript
import {
  ApiV2010AccountAvailablePhoneNumberCountryAvailablePhoneNumberSharedCostCapabilities,
} from "twilio-sdk/models/components";

let value:
  ApiV2010AccountAvailablePhoneNumberCountryAvailablePhoneNumberSharedCostCapabilities =
    {};
```

## Fields

| Field              | Type               | Required           | Description        |
| ------------------ | ------------------ | ------------------ | ------------------ |
| `mms`              | *boolean*          | :heavy_minus_sign: | N/A                |
| `sms`              | *boolean*          | :heavy_minus_sign: | N/A                |
| `voice`            | *boolean*          | :heavy_minus_sign: | N/A                |
| `fax`              | *boolean*          | :heavy_minus_sign: | N/A                |