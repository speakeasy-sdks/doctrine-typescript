<!-- Start SDK Example Usage -->


```typescript
import { Doctrine } from "Doctrine";

(async () => {
    const sdk = new Doctrine();

    const res = await sdk.httpLocalhost3000ApiScanpagecontent({
        url: "https://sardelkitchen.com/products/chili-infused-olive-oil",
    });

    if (res.statusCode == 200) {
        // handle response
    }
})();

```
<!-- End SDK Example Usage -->