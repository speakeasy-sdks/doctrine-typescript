# Document
(*document*)

### Available Operations

* [deleteDocument](#deletedocument) - Delete Document
* [listDocuments](#listdocuments) - List Documents

## deleteDocument

Delete Document

### Example Usage

```typescript
import { Doctrine } from "Doctrine";
import { DeleteDocumentResponse } from "Doctrine/dist/sdk/models/operations";

const sdk = new Doctrine();

sdk.document.deleteDocument().then((res: DeleteDocumentResponse) => {
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

**Promise<[operations.DeleteDocumentResponse](../../models/operations/deletedocumentresponse.md)>**


## listDocuments

List Documents

### Example Usage

```typescript
import { Doctrine } from "Doctrine";
import { ListDocumentsResponse } from "Doctrine/dist/sdk/models/operations";

const sdk = new Doctrine();

sdk.document.listDocuments().then((res: ListDocumentsResponse) => {
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

**Promise<[operations.ListDocumentsResponse](../../models/operations/listdocumentsresponse.md)>**

