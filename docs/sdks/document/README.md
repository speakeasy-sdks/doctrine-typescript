# Document
(*.document*)

### Available Operations

* [deleteDocument](#deletedocument) - Delete Document
* [listDocuments](#listdocuments) - List Documents

## deleteDocument

Delete Document

### Example Usage

```typescript
import { Doctrine } from "Doctrine";

(async() => {
  const sdk = new Doctrine();

  const res = await sdk.document.deleteDocument();


  if (res.statusCode == 200) {
    // handle response
  }
})();
```

### Parameters

| Parameter                                                    | Type                                                         | Required                                                     | Description                                                  |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| `config`                                                     | [AxiosRequestConfig](https://axios-http.com/docs/req_config) | :heavy_minus_sign:                                           | Available config options for making requests.                |


### Response

**Promise<[operations.DeleteDocumentResponse](../../models/operations/deletedocumentresponse.md)>**


## listDocuments

List Documents

### Example Usage

```typescript
import { Doctrine } from "Doctrine";

(async() => {
  const sdk = new Doctrine();

  const res = await sdk.document.listDocuments();


  if (res.statusCode == 200) {
    // handle response
  }
})();
```

### Parameters

| Parameter                                                    | Type                                                         | Required                                                     | Description                                                  |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| `config`                                                     | [AxiosRequestConfig](https://axios-http.com/docs/req_config) | :heavy_minus_sign:                                           | Available config options for making requests.                |


### Response

**Promise<[operations.ListDocumentsResponse](../../models/operations/listdocumentsresponse.md)>**

