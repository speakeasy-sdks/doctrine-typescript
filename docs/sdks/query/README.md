# Query
(*query*)

### Available Operations

* [askQuestionSetNumberOfContextDocs](#askquestionsetnumberofcontextdocs) - Ask Question set number of context docs

## askQuestionSetNumberOfContextDocs

Ask Question set number of context docs

### Example Usage

```typescript
import { Doctrine } from "Doctrine";

async function run() {
  const sdk = new Doctrine();

  const res = await sdk.query.askQuestionSetNumberOfContextDocs({
    numberOfDocumentsInContext: 3,
    query: "How long should I let coffee grounds bloom?",
  });

  if (res.statusCode == 200) {
    // handle response
  }
}

run();
```

### Parameters

| Parameter                                                                                                                              | Type                                                                                                                                   | Required                                                                                                                               | Description                                                                                                                            |
| -------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                              | [operations.AskQuestionSetNumberOfContextDocsRequestBody](../../sdk/models/operations/askquestionsetnumberofcontextdocsrequestbody.md) | :heavy_check_mark:                                                                                                                     | The request object to use for the request.                                                                                             |
| `config`                                                                                                                               | [AxiosRequestConfig](https://axios-http.com/docs/req_config)                                                                           | :heavy_minus_sign:                                                                                                                     | Available config options for making requests.                                                                                          |


### Response

**Promise<[operations.AskQuestionSetNumberOfContextDocsResponse](../../sdk/models/operations/askquestionsetnumberofcontextdocsresponse.md)>**
### Errors

| Error Object    | Status Code     | Content Type    |
| --------------- | --------------- | --------------- |
| errors.SDKError | 4xx-5xx         | */*             |
