# Ingest
(*ingest*)

### Available Operations

* [ingestTextWithMetadata](#ingesttextwithmetadata) - Ingest Text with Metadata

## ingestTextWithMetadata

Ingest Text with Metadata

### Example Usage

```typescript
import { Doctrine } from "Doctrine";

async function run() {
  const sdk = new Doctrine();

  const res = await sdk.ingest.ingestTextWithMetadata({
    metadata: {
      externalId: "12356abc",
      source: "Chemex creator",
    },
    name: "Sample doc",
    partition: "Metadata test",
    text: "Brewing coffee using a Chemex can result in a clean, pure, and flavorful cup of coffee. Here is a simple guide to brewing coffee using a Chemex:\n\nWhat you'll need:\n\nChemex\nChemex filters\n42 grams of coffee beans\nGrinder\n700 grams (or ml) of water, plus additional for rinsing\nKettle\nScale\nTimer\nSteps:\n\nBoil your water: Start by bringing your water to a boil. The ideal brewing temperature is between 1195 to 2005 degrees Fahrenheit, so let the water cool down a bit after boiling.\nGrind your coffee: While your water is boiling, grind your coffee beans to a medium-coarse grind. You want the consistency to be similar to sea salt.\nPrepare the filter: Place the Chemex filter in the brewer with the thicker (multi-layered) side against the pouring spout. Rinse the filter with hot water to get rid of any paper taste and to preheat the Chemex. Then, discard the rinse water.\nAdd coffee: Place your Chemex on the scale, tare it to zero, and add your ground coffee.\nBloom the coffee: Start your timer and pour enough water (about 70-100 grams) over the coffee grounds to wet them evenly. Let it sit and \"bloom\" for 30-45 seconds. This allows the coffee to de-gas, enabling the water to yield the full potential of the coffee.\nContinue pouring: After the bloom, continue pouring the water in a slow, steady spiral from the middle of the grounds outwards, pausing as needed to let it drip through. Try to avoid pouring directly on the filter. Continue until you've reached 700 grams (or ml) of water.\nWait: Allow the rest of the water to drip through the grounds. This should take around 4 to 5 minutes. If it's dripping too fast, you may need a finer grind. If it's too slow, try a coarser grind.\nEnjoy: Once the dripping slows to a stop, remove and discard the filter. Swirl the brewed coffee in the Chemex a bit to mix it evenly, then pour and enjoy!\nRemember, these are just guidelines. The best cup of coffee is one that tastes right to you, so feel free to adjust the amount of coffee, the grind size, the water temperature, and the brew time to suit your tastes. The Chemex is a forgiving brewing method, so don't be afraid to experiment a bit to find your perfect brew.",
  });

  if (res.statusCode == 200) {
    // handle response
  }
}

run();
```

### Parameters

| Parameter                                                                                                        | Type                                                                                                             | Required                                                                                                         | Description                                                                                                      |
| ---------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                        | [operations.IngestTextWithMetadataRequestBody](../../sdk/models/operations/ingesttextwithmetadatarequestbody.md) | :heavy_check_mark:                                                                                               | The request object to use for the request.                                                                       |
| `config`                                                                                                         | [AxiosRequestConfig](https://axios-http.com/docs/req_config)                                                     | :heavy_minus_sign:                                                                                               | Available config options for making requests.                                                                    |


### Response

**Promise<[operations.IngestTextWithMetadataResponse](../../sdk/models/operations/ingesttextwithmetadataresponse.md)>**
### Errors

| Error Object    | Status Code     | Content Type    |
| --------------- | --------------- | --------------- |
| errors.SDKError | 4xx-5xx         | */*             |
