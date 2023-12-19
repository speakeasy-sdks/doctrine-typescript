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

async function run() {
  const sdk = new Doctrine();

  const res = await sdk.chat.createPublicChat({
    name: "Public Chat",
    partitionId: "cli3wrtkt000c33d1yzc9acqj",
    public: true,
  });

  if (res.statusCode == 200) {
    // handle response
  }
}

run();
```

### Parameters

| Parameter                                                                                            | Type                                                                                                 | Required                                                                                             | Description                                                                                          |
| ---------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- |
| `request`                                                                                            | [operations.CreatePublicChatRequestBody](../../sdk/models/operations/createpublicchatrequestbody.md) | :heavy_check_mark:                                                                                   | The request object to use for the request.                                                           |
| `config`                                                                                             | [AxiosRequestConfig](https://axios-http.com/docs/req_config)                                         | :heavy_minus_sign:                                                                                   | Available config options for making requests.                                                        |


### Response

**Promise<[operations.CreatePublicChatResponse](../../sdk/models/operations/createpublicchatresponse.md)>**
### Errors

| Error Object    | Status Code     | Content Type    |
| --------------- | --------------- | --------------- |
| errors.SDKError | 4xx-5xx         | */*             |

## deleteChat

Delete Chat

### Example Usage

```typescript
import { Doctrine } from "Doctrine";

async function run() {
  const sdk = new Doctrine();

  const res = await sdk.chat.deleteChat();

  if (res.statusCode == 200) {
    // handle response
  }
}

run();
```

### Parameters

| Parameter                                                    | Type                                                         | Required                                                     | Description                                                  |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| `config`                                                     | [AxiosRequestConfig](https://axios-http.com/docs/req_config) | :heavy_minus_sign:                                           | Available config options for making requests.                |


### Response

**Promise<[operations.DeleteChatResponse](../../sdk/models/operations/deletechatresponse.md)>**
### Errors

| Error Object    | Status Code     | Content Type    |
| --------------- | --------------- | --------------- |
| errors.SDKError | 4xx-5xx         | */*             |

## sendMessageToPublicChat

Send message to Public Chat

### Example Usage

```typescript
import { Doctrine } from "Doctrine";

async function run() {
  const sdk = new Doctrine();

  const res = await sdk.chat.sendMessageToPublicChat({
    message: "How hot should water be?",
    userId: "cookiecookie",
  });

  if (res.statusCode == 200) {
    // handle response
  }
}

run();
```

### Parameters

| Parameter                                                                                                          | Type                                                                                                               | Required                                                                                                           | Description                                                                                                        |
| ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                          | [operations.SendMessageToPublicChatRequestBody](../../sdk/models/operations/sendmessagetopublicchatrequestbody.md) | :heavy_check_mark:                                                                                                 | The request object to use for the request.                                                                         |
| `config`                                                                                                           | [AxiosRequestConfig](https://axios-http.com/docs/req_config)                                                       | :heavy_minus_sign:                                                                                                 | Available config options for making requests.                                                                      |


### Response

**Promise<[operations.SendMessageToPublicChatResponse](../../sdk/models/operations/sendmessagetopublicchatresponse.md)>**
### Errors

| Error Object    | Status Code     | Content Type    |
| --------------- | --------------- | --------------- |
| errors.SDKError | 4xx-5xx         | */*             |
