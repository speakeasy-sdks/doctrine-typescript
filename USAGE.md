<!-- Start SDK Example Usage -->


```typescript
import { Doctrine } from "Doctrine";
import { HttpLocalhost3000ApiScanpagecontentResponse } from "Doctrine/dist/sdk/models/operations";

const sdk = new Doctrine();

sdk.httpLocalhost3000ApiScanpagecontent({
  url: "https://sardelkitchen.com/products/chili-infused-olive-oil",
}).then((res: HttpLocalhost3000ApiScanpagecontentResponse) => {
  if (res.statusCode == 200) {
    // handle response
  }
});
```
<!-- End SDK Example Usage -->