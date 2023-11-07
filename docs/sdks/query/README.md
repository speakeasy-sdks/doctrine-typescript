# Query
(*.query*)

### Available Operations

* [askQuestionSetNumberOfContextDocs](#askquestionsetnumberofcontextdocs) - Ask Question set number of context docs

## askQuestionSetNumberOfContextDocs

Ask Question set number of context docs

### Example Usage

```typescript
import { Doctrine } from "Doctrine";

(async() => {
  const sdk = new Doctrine();

  const res = await sdk.query.askQuestionSetNumberOfContextDocs({
    numberOfDocumentsInContext: 3,
    query: "How long should I let coffee grounds bloom?",
  });


  if (res.statusCode == 200) {
    // handle response
  }
})();
```

### Parameters

| Parameter                                                                                                                          | Type                                                                                                                               | Required                                                                                                                           | Description                                                                                                                        |
| ---------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                          | [operations.AskQuestionSetNumberOfContextDocsRequestBody](../../models/operations/askquestionsetnumberofcontextdocsrequestbody.md) | :heavy_check_mark:                                                                                                                 | The request object to use for the request.                                                                                         |
| `config`                                                                                                                           | [AxiosRequestConfig](https://axios-http.com/docs/req_config)                                                                       | :heavy_minus_sign:                                                                                                                 | Available config options for making requests.                                                                                      |


### Response

**Promise<[operations.AskQuestionSetNumberOfContextDocsResponse](../../models/operations/askquestionsetnumberofcontextdocsresponse.md)>**

