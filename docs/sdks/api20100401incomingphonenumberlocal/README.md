# Api20100401IncomingPhoneNumberLocal
(*api20100401IncomingPhoneNumberLocal*)

## Overview

### Available Operations

* [listIncomingPhoneNumberLocal](#listincomingphonenumberlocal)
* [createIncomingPhoneNumberLocal](#createincomingphonenumberlocal)

## listIncomingPhoneNumberLocal

### Example Usage

```typescript
import { TwilioSDK } from "twilio-sdk";

const twilioSDK = new TwilioSDK({
  security: {
    username: "",
    password: "",
  },
});

async function run() {
  const result = await twilioSDK.api20100401IncomingPhoneNumberLocal.listIncomingPhoneNumberLocal({
    accountSid: "<id>",
    beta: true,
    friendlyName: "friendly_name",
    phoneNumber: "+19876543210",
  });

  // Handle the result
  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { TwilioSDKCore } from "twilio-sdk/core.js";
import { api20100401IncomingPhoneNumberLocalListIncomingPhoneNumberLocal } from "twilio-sdk/funcs/api20100401IncomingPhoneNumberLocalListIncomingPhoneNumberLocal.js";

// Use `TwilioSDKCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const twilioSDK = new TwilioSDKCore({
  security: {
    username: "",
    password: "",
  },
});

async function run() {
  const res = await api20100401IncomingPhoneNumberLocalListIncomingPhoneNumberLocal(twilioSDK, {
    accountSid: "<id>",
    beta: true,
    friendlyName: "friendly_name",
    phoneNumber: "+19876543210",
  });

  if (!res.ok) {
    throw res.error;
  }

  const { value: result } = res;

  // Handle the result
  console.log(result);
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ListIncomingPhoneNumberLocalRequest](../../models/operations/listincomingphonenumberlocalrequest.md)                                                               | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |
| `options.serverURL`                                                                                                                                                            | *string*                                                                                                                                                                       | :heavy_minus_sign:                                                                                                                                                             | An optional server URL to use.                                                                                                                                                 |

### Response

**Promise\<[operations.ListIncomingPhoneNumberLocalResponse](../../models/operations/listincomingphonenumberlocalresponse.md)\>**

### Errors

| Error Type      | Status Code     | Content Type    |
| --------------- | --------------- | --------------- |
| errors.APIError | 4XX, 5XX        | \*/\*           |

## createIncomingPhoneNumberLocal

### Example Usage

```typescript
import { TwilioSDK } from "twilio-sdk";

const twilioSDK = new TwilioSDK({
  security: {
    username: "",
    password: "",
  },
});

async function run() {
  const result = await twilioSDK.api20100401IncomingPhoneNumberLocal.createIncomingPhoneNumberLocal({
    accountSid: "<id>",
    requestBody: {
      phoneNumber: "+18089255327",
      apiVersion: "api_version",
      friendlyName: "friendly_name",
      smsApplicationSid: "APaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa",
      smsFallbackMethod: "GET",
      smsFallbackUrl: "https://example.com",
      smsMethod: "GET",
      smsUrl: "https://example.com",
      statusCallback: "https://example.com",
      statusCallbackMethod: "GET",
      voiceApplicationSid: "APaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa",
      voiceCallerIdLookup: true,
      voiceFallbackMethod: "GET",
      voiceFallbackUrl: "https://example.com",
      voiceMethod: "GET",
      voiceUrl: "https://example.com",
      identitySid: "RIaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa",
      addressSid: "ADaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa",
      emergencyStatus: "Active",
      emergencyAddressSid: "ADaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa",
      bundleSid: "BUaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa",
    },
  });

  // Handle the result
  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { TwilioSDKCore } from "twilio-sdk/core.js";
import { api20100401IncomingPhoneNumberLocalCreateIncomingPhoneNumberLocal } from "twilio-sdk/funcs/api20100401IncomingPhoneNumberLocalCreateIncomingPhoneNumberLocal.js";

// Use `TwilioSDKCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const twilioSDK = new TwilioSDKCore({
  security: {
    username: "",
    password: "",
  },
});

async function run() {
  const res = await api20100401IncomingPhoneNumberLocalCreateIncomingPhoneNumberLocal(twilioSDK, {
    accountSid: "<id>",
    requestBody: {
      phoneNumber: "+18089255327",
      apiVersion: "api_version",
      friendlyName: "friendly_name",
      smsApplicationSid: "APaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa",
      smsFallbackMethod: "GET",
      smsFallbackUrl: "https://example.com",
      smsMethod: "GET",
      smsUrl: "https://example.com",
      statusCallback: "https://example.com",
      statusCallbackMethod: "GET",
      voiceApplicationSid: "APaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa",
      voiceCallerIdLookup: true,
      voiceFallbackMethod: "GET",
      voiceFallbackUrl: "https://example.com",
      voiceMethod: "GET",
      voiceUrl: "https://example.com",
      identitySid: "RIaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa",
      addressSid: "ADaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa",
      emergencyStatus: "Active",
      emergencyAddressSid: "ADaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa",
      bundleSid: "BUaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa",
    },
  });

  if (!res.ok) {
    throw res.error;
  }

  const { value: result } = res;

  // Handle the result
  console.log(result);
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.CreateIncomingPhoneNumberLocalRequest](../../models/operations/createincomingphonenumberlocalrequest.md)                                                           | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |
| `options.serverURL`                                                                                                                                                            | *string*                                                                                                                                                                       | :heavy_minus_sign:                                                                                                                                                             | An optional server URL to use.                                                                                                                                                 |

### Response

**Promise\<[operations.CreateIncomingPhoneNumberLocalResponse](../../models/operations/createincomingphonenumberlocalresponse.md)\>**

### Errors

| Error Type      | Status Code     | Content Type    |
| --------------- | --------------- | --------------- |
| errors.APIError | 4XX, 5XX        | \*/\*           |