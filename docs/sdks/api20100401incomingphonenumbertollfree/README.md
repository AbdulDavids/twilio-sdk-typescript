# Api20100401IncomingPhoneNumberTollFree
(*api20100401IncomingPhoneNumberTollFree*)

## Overview

### Available Operations

* [listIncomingPhoneNumberTollFree](#listincomingphonenumbertollfree)
* [createIncomingPhoneNumberTollFree](#createincomingphonenumbertollfree)

## listIncomingPhoneNumberTollFree

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
  const result = await twilioSDK.api20100401IncomingPhoneNumberTollFree.listIncomingPhoneNumberTollFree({
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
import { api20100401IncomingPhoneNumberTollFreeListIncomingPhoneNumberTollFree } from "twilio-sdk/funcs/api20100401IncomingPhoneNumberTollFreeListIncomingPhoneNumberTollFree.js";

// Use `TwilioSDKCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const twilioSDK = new TwilioSDKCore({
  security: {
    username: "",
    password: "",
  },
});

async function run() {
  const res = await api20100401IncomingPhoneNumberTollFreeListIncomingPhoneNumberTollFree(twilioSDK, {
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
| `request`                                                                                                                                                                      | [operations.ListIncomingPhoneNumberTollFreeRequest](../../models/operations/listincomingphonenumbertollfreerequest.md)                                                         | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |
| `options.serverURL`                                                                                                                                                            | *string*                                                                                                                                                                       | :heavy_minus_sign:                                                                                                                                                             | An optional server URL to use.                                                                                                                                                 |

### Response

**Promise\<[operations.ListIncomingPhoneNumberTollFreeResponse](../../models/operations/listincomingphonenumbertollfreeresponse.md)\>**

### Errors

| Error Type      | Status Code     | Content Type    |
| --------------- | --------------- | --------------- |
| errors.APIError | 4XX, 5XX        | \*/\*           |

## createIncomingPhoneNumberTollFree

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
  const result = await twilioSDK.api20100401IncomingPhoneNumberTollFree.createIncomingPhoneNumberTollFree({
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
import { api20100401IncomingPhoneNumberTollFreeCreateIncomingPhoneNumberTollFree } from "twilio-sdk/funcs/api20100401IncomingPhoneNumberTollFreeCreateIncomingPhoneNumberTollFree.js";

// Use `TwilioSDKCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const twilioSDK = new TwilioSDKCore({
  security: {
    username: "",
    password: "",
  },
});

async function run() {
  const res = await api20100401IncomingPhoneNumberTollFreeCreateIncomingPhoneNumberTollFree(twilioSDK, {
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
| `request`                                                                                                                                                                      | [operations.CreateIncomingPhoneNumberTollFreeRequest](../../models/operations/createincomingphonenumbertollfreerequest.md)                                                     | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |
| `options.serverURL`                                                                                                                                                            | *string*                                                                                                                                                                       | :heavy_minus_sign:                                                                                                                                                             | An optional server URL to use.                                                                                                                                                 |

### Response

**Promise\<[operations.CreateIncomingPhoneNumberTollFreeResponse](../../models/operations/createincomingphonenumbertollfreeresponse.md)\>**

### Errors

| Error Type      | Status Code     | Content Type    |
| --------------- | --------------- | --------------- |
| errors.APIError | 4XX, 5XX        | \*/\*           |