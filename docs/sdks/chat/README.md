# Chat
(*chat*)

### Available Operations

* [createPublicChat](#createpublicchat) - Create Public Chat
* [deleteChat](#deletechat) - Delete Chat
* [sendMessageToPublicChat](#sendmessagetopublicchat) - Send message to Public Chat

## createPublicChat

Create Public Chat

### Example Usage

```typescript
import { Doctrine } from "Doctrine";
import { CreatePublicChatResponse } from "Doctrine/dist/sdk/models/operations";

const sdk = new Doctrine();

sdk.chat.createPublicChat({
  name: "Public Chat",
  partitionId: "cli3wrtkt000c33d1yzc9acqj",
  public: true,
}).then((res: CreatePublicChatResponse) => {
  if (res.statusCode == 200) {
    // handle response
  }
});
```

### Parameters

| Parameter                                                                                        | Type                                                                                             | Required                                                                                         | Description                                                                                      |
| ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ |
| `request`                                                                                        | [operations.CreatePublicChatRequestBody](../../models/operations/createpublicchatrequestbody.md) | :heavy_check_mark:                                                                               | The request object to use for the request.                                                       |
| `config`                                                                                         | [AxiosRequestConfig](https://axios-http.com/docs/req_config)                                     | :heavy_minus_sign:                                                                               | Available config options for making requests.                                                    |


### Response

**Promise<[operations.CreatePublicChatResponse](../../models/operations/createpublicchatresponse.md)>**


## deleteChat

Delete Chat

### Example Usage

```typescript
import { Doctrine } from "Doctrine";
import { DeleteChatResponse } from "Doctrine/dist/sdk/models/operations";

const sdk = new Doctrine();

sdk.chat.deleteChat().then((res: DeleteChatResponse) => {
  if (res.statusCode == 200) {
    // handle response
  }
});
```

### Parameters

| Parameter                                                    | Type                                                         | Required                                                     | Description                                                  |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| `config`                                                     | [AxiosRequestConfig](https://axios-http.com/docs/req_config) | :heavy_minus_sign:                                           | Available config options for making requests.                |


### Response

**Promise<[operations.DeleteChatResponse](../../models/operations/deletechatresponse.md)>**


## sendMessageToPublicChat

Send message to Public Chat

### Example Usage

```typescript
import { Doctrine } from "Doctrine";
import { SendMessageToPublicChatResponse } from "Doctrine/dist/sdk/models/operations";

const sdk = new Doctrine();

sdk.chat.sendMessageToPublicChat({
  message: "How hot should water be?",
  userId: "cookiecookie",
}).then((res: SendMessageToPublicChatResponse) => {
  if (res.statusCode == 200) {
    // handle response
  }
});
```

### Parameters

| Parameter                                                                                                      | Type                                                                                                           | Required                                                                                                       | Description                                                                                                    |
| -------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                      | [operations.SendMessageToPublicChatRequestBody](../../models/operations/sendmessagetopublicchatrequestbody.md) | :heavy_check_mark:                                                                                             | The request object to use for the request.                                                                     |
| `config`                                                                                                       | [AxiosRequestConfig](https://axios-http.com/docs/req_config)                                                   | :heavy_minus_sign:                                                                                             | Available config options for making requests.                                                                  |


### Response

**Promise<[operations.SendMessageToPublicChatResponse](../../models/operations/sendmessagetopublicchatresponse.md)>**

