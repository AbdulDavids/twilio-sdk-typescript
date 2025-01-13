# FetchAvailablePhoneNumberCountryRequest

## Example Usage

```typescript
import { FetchAvailablePhoneNumberCountryRequest } from "twilio-sdk/models/operations";

let value: FetchAvailablePhoneNumberCountryRequest = {
  accountSid: "<id>",
  countryCode: "<value>",
};
```

## Fields

| Field                                                                                                                                             | Type                                                                                                                                              | Required                                                                                                                                          | Description                                                                                                                                       |
| ------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------- |
| `accountSid`                                                                                                                                      | *string*                                                                                                                                          | :heavy_check_mark:                                                                                                                                | The SID of the [Account](https://www.twilio.com/docs/iam/api/account) requesting the available phone number Country resource.                     |
| `countryCode`                                                                                                                                     | *string*                                                                                                                                          | :heavy_check_mark:                                                                                                                                | The [ISO-3166-1](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2) country code of the country to fetch available phone number information about. |