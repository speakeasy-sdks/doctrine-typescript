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
import { HttpLocalhost3000ApiScanpagecontentResponse } from "Doctrine/dist/sdk/models/operations";

const sdk = new Doctrine();

sdk.doctrine.httpLocalhost3000ApiScanpagecontent({
  url: "https://sardelkitchen.com/products/chili-infused-olive-oil",
}).then((res: HttpLocalhost3000ApiScanpagecontentResponse) => {
  if (res.statusCode == 200) {
    // handle response
  }
});
```

### Parameters

| Parameter                                                                                                                              | Type                                                                                                                                   | Required                                                                                                                               | Description                                                                                                                            |
| -------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                              | [operations.HttpLocalhost3000ApiScanpagecontentRequestBody](../../models/operations/httplocalhost3000apiscanpagecontentrequestbody.md) | :heavy_check_mark:                                                                                                                     | The request object to use for the request.                                                                                             |
| `config`                                                                                                                               | [AxiosRequestConfig](https://axios-http.com/docs/req_config)                                                                           | :heavy_minus_sign:                                                                                                                     | Available config options for making requests.                                                                                          |


### Response

**Promise<[operations.HttpLocalhost3000ApiScanpagecontentResponse](../../models/operations/httplocalhost3000apiscanpagecontentresponse.md)>**


## httpLocalhost3000ApiScansitemap

http://localhost:3000/api/scanSitemap

### Example Usage

```typescript
import { Doctrine } from "Doctrine";
import { HttpLocalhost3000ApiScansitemapResponse } from "Doctrine/dist/sdk/models/operations";

const sdk = new Doctrine();

sdk.doctrine.httpLocalhost3000ApiScansitemap({
  rootDomain: "sardelkitchen.com",
}).then((res: HttpLocalhost3000ApiScansitemapResponse) => {
  if (res.statusCode == 200) {
    // handle response
  }
});
```

### Parameters

| Parameter                                                                                                                      | Type                                                                                                                           | Required                                                                                                                       | Description                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                      | [operations.HttpLocalhost3000ApiScansitemapRequestBody](../../models/operations/httplocalhost3000apiscansitemaprequestbody.md) | :heavy_check_mark:                                                                                                             | The request object to use for the request.                                                                                     |
| `config`                                                                                                                       | [AxiosRequestConfig](https://axios-http.com/docs/req_config)                                                                   | :heavy_minus_sign:                                                                                                             | Available config options for making requests.                                                                                  |


### Response

**Promise<[operations.HttpLocalhost3000ApiScansitemapResponse](../../models/operations/httplocalhost3000apiscansitemapresponse.md)>**
