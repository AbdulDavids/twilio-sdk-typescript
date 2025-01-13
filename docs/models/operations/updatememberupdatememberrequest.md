# UpdateMemberUpdateMemberRequest

## Example Usage

```typescript
import { UpdateMemberUpdateMemberRequest } from "twilio-sdk/models/operations";

let value: UpdateMemberUpdateMemberRequest = {
  url: "https://querulous-chap.biz/",
};
```

## Fields

| Field                                                                                                                                                                           | Type                                                                                                                                                                            | Required                                                                                                                                                                        | Description                                                                                                                                                                     |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `url`                                                                                                                                                                           | *string*                                                                                                                                                                        | :heavy_check_mark:                                                                                                                                                              | The absolute URL of the Queue resource.                                                                                                                                         |
| `method`                                                                                                                                                                        | [operations.UpdateMemberMethod](../../models/operations/updatemembermethod.md)                                                                                                  | :heavy_minus_sign:                                                                                                                                                              | How to pass the update request data. Can be `GET` or `POST` and the default is `POST`. `POST` sends the data as encoded form data and `GET` sends the data as query parameters. |