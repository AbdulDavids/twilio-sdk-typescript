<!-- Start SDK Example Usage [usage] -->
```typescript
import { TwilioSDK } from "twilio-sdk";

const twilioSDK = new TwilioSDK({
  security: {
    username: "",
    password: "",
  },
});

async function run() {
  const result = await twilioSDK.api20100401Account.createAccount({
    friendlyName: "friendly_name",
  });

  // Handle the result
  console.log(result);
}

run();

```
<!-- End SDK Example Usage [usage] -->