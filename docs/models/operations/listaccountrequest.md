# ListAccountRequest

## Example Usage

```typescript
import { ListAccountRequest } from "twilio-sdk/models/operations";

let value: ListAccountRequest = {};
```

## Fields

| Field                                                                                          | Type                                                                                           | Required                                                                                       | Description                                                                                    |
| ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- |
| `friendlyName`                                                                                 | *string*                                                                                       | :heavy_minus_sign:                                                                             | Only return the Account resources with friendly names that exactly match this name.            |
| `status`                                                                                       | [components.AccountEnumStatus](../../models/components/accountenumstatus.md)                   | :heavy_minus_sign:                                                                             | Only return Account resources with the given status. Can be `closed`, `suspended` or `active`. |
| `pageSize`                                                                                     | *number*                                                                                       | :heavy_minus_sign:                                                                             | How many resources to return in each list page. The default is 50, and the maximum is 1000.    |
| `page`                                                                                         | *number*                                                                                       | :heavy_minus_sign:                                                                             | The page index. This value is simply for client state.                                         |
| `pageToken`                                                                                    | *string*                                                                                       | :heavy_minus_sign:                                                                             | The page token. This is provided by the API.                                                   |