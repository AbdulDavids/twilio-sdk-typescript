# Api20100401IncomingPhoneNumber
(*api20100401IncomingPhoneNumber*)

## Overview

### Available Operations

* [updateIncomingPhoneNumber](#updateincomingphonenumber) - Update an incoming-phone-number instance.
* [fetchIncomingPhoneNumber](#fetchincomingphonenumber) - Fetch an incoming-phone-number belonging to the account used to make the request.
* [deleteIncomingPhoneNumber](#deleteincomingphonenumber) - Delete a phone-numbers belonging to the account used to make the request.
* [listIncomingPhoneNumber](#listincomingphonenumber) - Retrieve a list of incoming-phone-numbers belonging to the account used to make the request.
* [createIncomingPhoneNumber](#createincomingphonenumber) - Purchase a phone-number for the account.

## updateIncomingPhoneNumber

Update an incoming-phone-number instance.

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
  const result = await twilioSDK.api20100401IncomingPhoneNumber.updateIncomingPhoneNumber({
    accountSid: "<id>",
    sid: "<id>",
    requestBody: {
      accountSid: "ACaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa",
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
      emergencyStatus: "Inactive",
      emergencyAddressSid: "ADaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa",
      voiceReceiveMode: "voice",
      identitySid: "RIaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa",
      addressSid: "ADaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa",
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
import { api20100401IncomingPhoneNumberUpdateIncomingPhoneNumber } from "twilio-sdk/funcs/api20100401IncomingPhoneNumberUpdateIncomingPhoneNumber.js";

// Use `TwilioSDKCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const twilioSDK = new TwilioSDKCore({
  security: {
    username: "",
    password: "",
  },
});

async function run() {
  const res = await api20100401IncomingPhoneNumberUpdateIncomingPhoneNumber(twilioSDK, {
    accountSid: "<id>",
    sid: "<id>",
    requestBody: {
      accountSid: "ACaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa",
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
      emergencyStatus: "Inactive",
      emergencyAddressSid: "ADaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa",
      voiceReceiveMode: "voice",
      identitySid: "RIaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa",
      addressSid: "ADaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa",
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
| `request`                                                                                                                                                                      | [operations.UpdateIncomingPhoneNumberRequest](../../models/operations/updateincomingphonenumberrequest.md)                                                                     | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |
| `options.serverURL`                                                                                                                                                            | *string*                                                                                                                                                                       | :heavy_minus_sign:                                                                                                                                                             | An optional server URL to use.                                                                                                                                                 |

### Response

**Promise\<[operations.UpdateIncomingPhoneNumberResponse](../../models/operations/updateincomingphonenumberresponse.md)\>**

### Errors

| Error Type      | Status Code     | Content Type    |
| --------------- | --------------- | --------------- |
| errors.APIError | 4XX, 5XX        | \*/\*           |

## fetchIncomingPhoneNumber

Fetch an incoming-phone-number belonging to the account used to make the request.

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
  const result = await twilioSDK.api20100401IncomingPhoneNumber.fetchIncomingPhoneNumber({
    accountSid: "<id>",
    sid: "<id>",
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
import { api20100401IncomingPhoneNumberFetchIncomingPhoneNumber } from "twilio-sdk/funcs/api20100401IncomingPhoneNumberFetchIncomingPhoneNumber.js";

// Use `TwilioSDKCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const twilioSDK = new TwilioSDKCore({
  security: {
    username: "",
    password: "",
  },
});

async function run() {
  const res = await api20100401IncomingPhoneNumberFetchIncomingPhoneNumber(twilioSDK, {
    accountSid: "<id>",
    sid: "<id>",
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
| `request`                                                                                                                                                                      | [operations.FetchIncomingPhoneNumberRequest](../../models/operations/fetchincomingphonenumberrequest.md)                                                                       | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |
| `options.serverURL`                                                                                                                                                            | *string*                                                                                                                                                                       | :heavy_minus_sign:                                                                                                                                                             | An optional server URL to use.                                                                                                                                                 |

### Response

**Promise\<[operations.FetchIncomingPhoneNumberResponse](../../models/operations/fetchincomingphonenumberresponse.md)\>**

### Errors

| Error Type      | Status Code     | Content Type    |
| --------------- | --------------- | --------------- |
| errors.APIError | 4XX, 5XX        | \*/\*           |

## deleteIncomingPhoneNumber

Delete a phone-numbers belonging to the account used to make the request.

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
  await twilioSDK.api20100401IncomingPhoneNumber.deleteIncomingPhoneNumber({
    accountSid: "<id>",
    sid: "<id>",
  });


}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { TwilioSDKCore } from "twilio-sdk/core.js";
import { api20100401IncomingPhoneNumberDeleteIncomingPhoneNumber } from "twilio-sdk/funcs/api20100401IncomingPhoneNumberDeleteIncomingPhoneNumber.js";

// Use `TwilioSDKCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const twilioSDK = new TwilioSDKCore({
  security: {
    username: "",
    password: "",
  },
});

async function run() {
  const res = await api20100401IncomingPhoneNumberDeleteIncomingPhoneNumber(twilioSDK, {
    accountSid: "<id>",
    sid: "<id>",
  });

  if (!res.ok) {
    throw res.error;
  }

  const { value: result } = res;

  
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.DeleteIncomingPhoneNumberRequest](../../models/operations/deleteincomingphonenumberrequest.md)                                                                     | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |
| `options.serverURL`                                                                                                                                                            | *string*                                                                                                                                                                       | :heavy_minus_sign:                                                                                                                                                             | An optional server URL to use.                                                                                                                                                 |

### Response

**Promise\<void\>**

### Errors

| Error Type      | Status Code     | Content Type    |
| --------------- | --------------- | --------------- |
| errors.APIError | 4XX, 5XX        | \*/\*           |

## listIncomingPhoneNumber

Retrieve a list of incoming-phone-numbers belonging to the account used to make the request.

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
  const result = await twilioSDK.api20100401IncomingPhoneNumber.listIncomingPhoneNumber({
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
import { api20100401IncomingPhoneNumberListIncomingPhoneNumber } from "twilio-sdk/funcs/api20100401IncomingPhoneNumberListIncomingPhoneNumber.js";

// Use `TwilioSDKCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const twilioSDK = new TwilioSDKCore({
  security: {
    username: "",
    password: "",
  },
});

async function run() {
  const res = await api20100401IncomingPhoneNumberListIncomingPhoneNumber(twilioSDK, {
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
| `request`                                                                                                                                                                      | [operations.ListIncomingPhoneNumberRequest](../../models/operations/listincomingphonenumberrequest.md)                                                                         | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |
| `options.serverURL`                                                                                                                                                            | *string*                                                                                                                                                                       | :heavy_minus_sign:                                                                                                                                                             | An optional server URL to use.                                                                                                                                                 |

### Response

**Promise\<[operations.ListIncomingPhoneNumberResponse](../../models/operations/listincomingphonenumberresponse.md)\>**

### Errors

| Error Type      | Status Code     | Content Type    |
| --------------- | --------------- | --------------- |
| errors.APIError | 4XX, 5XX        | \*/\*           |

## createIncomingPhoneNumber

Purchase a phone-number for the account.

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
  const result = await twilioSDK.api20100401IncomingPhoneNumber.createIncomingPhoneNumber({
    accountSid: "<id>",
    requestBody: {
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
      emergencyStatus: "Active",
      emergencyAddressSid: "ADaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa",
      identitySid: "RIaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa",
      addressSid: "ADaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa",
      bundleSid: "BUaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa",
      phoneNumber: "+18089255327",
      areaCode: "area_code",
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
import { api20100401IncomingPhoneNumberCreateIncomingPhoneNumber } from "twilio-sdk/funcs/api20100401IncomingPhoneNumberCreateIncomingPhoneNumber.js";

// Use `TwilioSDKCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const twilioSDK = new TwilioSDKCore({
  security: {
    username: "",
    password: "",
  },
});

async function run() {
  const res = await api20100401IncomingPhoneNumberCreateIncomingPhoneNumber(twilioSDK, {
    accountSid: "<id>",
    requestBody: {
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
      emergencyStatus: "Active",
      emergencyAddressSid: "ADaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa",
      identitySid: "RIaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa",
      addressSid: "ADaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa",
      bundleSid: "BUaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa",
      phoneNumber: "+18089255327",
      areaCode: "area_code",
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
| `request`                                                                                                                                                                      | [operations.CreateIncomingPhoneNumberRequest](../../models/operations/createincomingphonenumberrequest.md)                                                                     | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |
| `options.serverURL`                                                                                                                                                            | *string*                                                                                                                                                                       | :heavy_minus_sign:                                                                                                                                                             | An optional server URL to use.                                                                                                                                                 |

### Response

**Promise\<[operations.CreateIncomingPhoneNumberResponse](../../models/operations/createincomingphonenumberresponse.md)\>**

### Errors

| Error Type      | Status Code     | Content Type    |
| --------------- | --------------- | --------------- |
| errors.APIError | 4XX, 5XX        | \*/\*           |