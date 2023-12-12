<!-- Start SDK Example Usage [usage] -->
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
<!-- End SDK Example Usage [usage] -->