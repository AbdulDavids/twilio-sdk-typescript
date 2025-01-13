# Api20100401Stream
(*api20100401Stream*)

## Overview

### Available Operations

* [createStream](#createstream) - Create a Stream
* [updateStream](#updatestream) - Stop a Stream using either the SID of the Stream resource or the `name` used when creating the resource

## createStream

Create a Stream

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
  const result = await twilioSDK.api20100401Stream.createStream({
    accountSid: "<id>",
    callSid: "<id>",
    requestBody: {
      url: "myUrl",
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
import { api20100401StreamCreateStream } from "twilio-sdk/funcs/api20100401StreamCreateStream.js";

// Use `TwilioSDKCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const twilioSDK = new TwilioSDKCore({
  security: {
    username: "",
    password: "",
  },
});

async function run() {
  const res = await api20100401StreamCreateStream(twilioSDK, {
    accountSid: "<id>",
    callSid: "<id>",
    requestBody: {
      url: "myUrl",
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
| `request`                                                                                                                                                                      | [operations.CreateStreamRequest](../../models/operations/createstreamrequest.md)                                                                                               | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |
| `options.serverURL`                                                                                                                                                            | *string*                                                                                                                                                                       | :heavy_minus_sign:                                                                                                                                                             | An optional server URL to use.                                                                                                                                                 |

### Response

**Promise\<[operations.CreateStreamResponse](../../models/operations/createstreamresponse.md)\>**

### Errors

| Error Type      | Status Code     | Content Type    |
| --------------- | --------------- | --------------- |
| errors.APIError | 4XX, 5XX        | \*/\*           |

## updateStream

Stop a Stream using either the SID of the Stream resource or the `name` used when creating the resource

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
  const result = await twilioSDK.api20100401Stream.updateStream({
    accountSid: "<id>",
    callSid: "<id>",
    sid: "<id>",
    requestBody: {
      status: "stopped",
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
import { api20100401StreamUpdateStream } from "twilio-sdk/funcs/api20100401StreamUpdateStream.js";

// Use `TwilioSDKCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const twilioSDK = new TwilioSDKCore({
  security: {
    username: "",
    password: "",
  },
});

async function run() {
  const res = await api20100401StreamUpdateStream(twilioSDK, {
    accountSid: "<id>",
    callSid: "<id>",
    sid: "<id>",
    requestBody: {
      status: "stopped",
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
| `request`                                                                                                                                                                      | [operations.UpdateStreamRequest](../../models/operations/updatestreamrequest.md)                                                                                               | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |
| `options.serverURL`                                                                                                                                                            | *string*                                                                                                                                                                       | :heavy_minus_sign:                                                                                                                                                             | An optional server URL to use.                                                                                                                                                 |

### Response

**Promise\<[operations.UpdateStreamResponse](../../models/operations/updatestreamresponse.md)\>**

### Errors

| Error Type      | Status Code     | Content Type    |
| --------------- | --------------- | --------------- |
| errors.APIError | 4XX, 5XX        | \*/\*           |