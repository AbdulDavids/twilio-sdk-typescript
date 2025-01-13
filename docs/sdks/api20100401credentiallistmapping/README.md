# Api20100401CredentialListMapping
(*api20100401CredentialListMapping*)

## Overview

### Available Operations

* [createSipCredentialListMapping](#createsipcredentiallistmapping) - Create a CredentialListMapping resource for an account.
* [listSipCredentialListMapping](#listsipcredentiallistmapping) - Read multiple CredentialListMapping resources from an account.
* [fetchSipCredentialListMapping](#fetchsipcredentiallistmapping) - Fetch a single CredentialListMapping resource from an account.
* [deleteSipCredentialListMapping](#deletesipcredentiallistmapping) - Delete a CredentialListMapping resource from an account.

## createSipCredentialListMapping

Create a CredentialListMapping resource for an account.

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
  const result = await twilioSDK.api20100401CredentialListMapping.createSipCredentialListMapping({
    accountSid: "<id>",
    domainSid: "<id>",
    requestBody: {
      credentialListSid: "CLaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa",
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
import { api20100401CredentialListMappingCreateSipCredentialListMapping } from "twilio-sdk/funcs/api20100401CredentialListMappingCreateSipCredentialListMapping.js";

// Use `TwilioSDKCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const twilioSDK = new TwilioSDKCore({
  security: {
    username: "",
    password: "",
  },
});

async function run() {
  const res = await api20100401CredentialListMappingCreateSipCredentialListMapping(twilioSDK, {
    accountSid: "<id>",
    domainSid: "<id>",
    requestBody: {
      credentialListSid: "CLaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa",
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
| `request`                                                                                                                                                                      | [operations.CreateSipCredentialListMappingRequest](../../models/operations/createsipcredentiallistmappingrequest.md)                                                           | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |
| `options.serverURL`                                                                                                                                                            | *string*                                                                                                                                                                       | :heavy_minus_sign:                                                                                                                                                             | An optional server URL to use.                                                                                                                                                 |

### Response

**Promise\<[operations.CreateSipCredentialListMappingResponse](../../models/operations/createsipcredentiallistmappingresponse.md)\>**

### Errors

| Error Type      | Status Code     | Content Type    |
| --------------- | --------------- | --------------- |
| errors.APIError | 4XX, 5XX        | \*/\*           |

## listSipCredentialListMapping

Read multiple CredentialListMapping resources from an account.

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
  const result = await twilioSDK.api20100401CredentialListMapping.listSipCredentialListMapping({
    accountSid: "<id>",
    domainSid: "<id>",
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
import { api20100401CredentialListMappingListSipCredentialListMapping } from "twilio-sdk/funcs/api20100401CredentialListMappingListSipCredentialListMapping.js";

// Use `TwilioSDKCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const twilioSDK = new TwilioSDKCore({
  security: {
    username: "",
    password: "",
  },
});

async function run() {
  const res = await api20100401CredentialListMappingListSipCredentialListMapping(twilioSDK, {
    accountSid: "<id>",
    domainSid: "<id>",
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
| `request`                                                                                                                                                                      | [operations.ListSipCredentialListMappingRequest](../../models/operations/listsipcredentiallistmappingrequest.md)                                                               | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |
| `options.serverURL`                                                                                                                                                            | *string*                                                                                                                                                                       | :heavy_minus_sign:                                                                                                                                                             | An optional server URL to use.                                                                                                                                                 |

### Response

**Promise\<[operations.ListSipCredentialListMappingResponse](../../models/operations/listsipcredentiallistmappingresponse.md)\>**

### Errors

| Error Type      | Status Code     | Content Type    |
| --------------- | --------------- | --------------- |
| errors.APIError | 4XX, 5XX        | \*/\*           |

## fetchSipCredentialListMapping

Fetch a single CredentialListMapping resource from an account.

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
  const result = await twilioSDK.api20100401CredentialListMapping.fetchSipCredentialListMapping({
    accountSid: "<id>",
    domainSid: "<id>",
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
import { api20100401CredentialListMappingFetchSipCredentialListMapping } from "twilio-sdk/funcs/api20100401CredentialListMappingFetchSipCredentialListMapping.js";

// Use `TwilioSDKCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const twilioSDK = new TwilioSDKCore({
  security: {
    username: "",
    password: "",
  },
});

async function run() {
  const res = await api20100401CredentialListMappingFetchSipCredentialListMapping(twilioSDK, {
    accountSid: "<id>",
    domainSid: "<id>",
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
| `request`                                                                                                                                                                      | [operations.FetchSipCredentialListMappingRequest](../../models/operations/fetchsipcredentiallistmappingrequest.md)                                                             | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |
| `options.serverURL`                                                                                                                                                            | *string*                                                                                                                                                                       | :heavy_minus_sign:                                                                                                                                                             | An optional server URL to use.                                                                                                                                                 |

### Response

**Promise\<[operations.FetchSipCredentialListMappingResponse](../../models/operations/fetchsipcredentiallistmappingresponse.md)\>**

### Errors

| Error Type      | Status Code     | Content Type    |
| --------------- | --------------- | --------------- |
| errors.APIError | 4XX, 5XX        | \*/\*           |

## deleteSipCredentialListMapping

Delete a CredentialListMapping resource from an account.

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
  await twilioSDK.api20100401CredentialListMapping.deleteSipCredentialListMapping({
    accountSid: "<id>",
    domainSid: "<id>",
    sid: "<id>",
  });


}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { TwilioSDKCore } from "twilio-sdk/core.js";
import { api20100401CredentialListMappingDeleteSipCredentialListMapping } from "twilio-sdk/funcs/api20100401CredentialListMappingDeleteSipCredentialListMapping.js";

// Use `TwilioSDKCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const twilioSDK = new TwilioSDKCore({
  security: {
    username: "",
    password: "",
  },
});

async function run() {
  const res = await api20100401CredentialListMappingDeleteSipCredentialListMapping(twilioSDK, {
    accountSid: "<id>",
    domainSid: "<id>",
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
| `request`                                                                                                                                                                      | [operations.DeleteSipCredentialListMappingRequest](../../models/operations/deletesipcredentiallistmappingrequest.md)                                                           | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
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