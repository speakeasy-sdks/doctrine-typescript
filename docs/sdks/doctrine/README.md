# Doctrine SDK


## Overview

### Available Operations

* [httpLocalhost3000ApiScanpagecontent](#httplocalhost3000apiscanpagecontent) - http://localhost:3000/api/scanPageContent
* [httpLocalhost3000ApiScansitemap](#httplocalhost3000apiscansitemap) - http://localhost:3000/api/scanSitemap

## httpLocalhost3000ApiScanpagecontent

http://localhost:3000/api/scanPageContent

### Example Usage

```typescript
import { Doctrine } from "Doctrine";

async function run() {
  const sdk = new Doctrine();

  const res = await sdk.httpLocalhost3000ApiScanpagecontent({
    url: "https://sardelkitchen.com/products/chili-infused-olive-oil",
  });

  if (res.statusCode == 200) {
    // handle response
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                  | Type                                                                                                                                       | Required                                                                                                                                   | Description                                                                                                                                |
| ------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                  | [operations.HttpLocalhost3000ApiScanpagecontentRequestBody](../../sdk/models/operations/httplocalhost3000apiscanpagecontentrequestbody.md) | :heavy_check_mark:                                                                                                                         | The request object to use for the request.                                                                                                 |
| `config`                                                                                                                                   | [AxiosRequestConfig](https://axios-http.com/docs/req_config)                                                                               | :heavy_minus_sign:                                                                                                                         | Available config options for making requests.                                                                                              |


### Response

**Promise<[operations.HttpLocalhost3000ApiScanpagecontentResponse](../../sdk/models/operations/httplocalhost3000apiscanpagecontentresponse.md)>**
### Errors

| Error Object    | Status Code     | Content Type    |
| --------------- | --------------- | --------------- |
| errors.SDKError | 4xx-5xx         | */*             |

## httpLocalhost3000ApiScansitemap

http://localhost:3000/api/scanSitemap

### Example Usage

```typescript
import { Doctrine } from "Doctrine";

async function run() {
  const sdk = new Doctrine();

  const res = await sdk.httpLocalhost3000ApiScansitemap({
    rootDomain: "sardelkitchen.com",
  });

  if (res.statusCode == 200) {
    // handle response
  }
}

run();
```

### Parameters

| Parameter                                                                                                                          | Type                                                                                                                               | Required                                                                                                                           | Description                                                                                                                        |
| ---------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                          | [operations.HttpLocalhost3000ApiScansitemapRequestBody](../../sdk/models/operations/httplocalhost3000apiscansitemaprequestbody.md) | :heavy_check_mark:                                                                                                                 | The request object to use for the request.                                                                                         |
| `config`                                                                                                                           | [AxiosRequestConfig](https://axios-http.com/docs/req_config)                                                                       | :heavy_minus_sign:                                                                                                                 | Available config options for making requests.                                                                                      |


### Response

**Promise<[operations.HttpLocalhost3000ApiScansitemapResponse](../../sdk/models/operations/httplocalhost3000apiscansitemapresponse.md)>**
### Errors

| Error Object    | Status Code     | Content Type    |
| --------------- | --------------- | --------------- |
| errors.SDKError | 4xx-5xx         | */*             |
