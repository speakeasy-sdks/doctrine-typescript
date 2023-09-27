# Doctrine

<!-- Start SDK Installation -->
## SDK Installation

### NPM

```bash
npm add https://github.com/speakeasy-sdks/doctrine-typescript
```

### Yarn

```bash
yarn add https://github.com/speakeasy-sdks/doctrine-typescript
```
<!-- End SDK Installation -->

## SDK Example Usage
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

<!-- Start SDK Available Operations -->
## Available Resources and Operations

### [Doctrine SDK](docs/sdks/doctrine/README.md)

* [httpLocalhost3000ApiScanpagecontent](docs/sdks/doctrine/README.md#httplocalhost3000apiscanpagecontent) - http://localhost:3000/api/scanPageContent
* [httpLocalhost3000ApiScansitemap](docs/sdks/doctrine/README.md#httplocalhost3000apiscansitemap) - http://localhost:3000/api/scanSitemap

### [chat](docs/sdks/chat/README.md)

* [createPublicChat](docs/sdks/chat/README.md#createpublicchat) - Create Public Chat
* [deleteChat](docs/sdks/chat/README.md#deletechat) - Delete Chat
* [sendMessageToPublicChat](docs/sdks/chat/README.md#sendmessagetopublicchat) - Send message to Public Chat

### [document](docs/sdks/document/README.md)

* [deleteDocument](docs/sdks/document/README.md#deletedocument) - Delete Document
* [listDocuments](docs/sdks/document/README.md#listdocuments) - List Documents

### [ingest](docs/sdks/ingest/README.md)

* [ingestTextWithMetadata](docs/sdks/ingest/README.md#ingesttextwithmetadata) - Ingest Text with Metadata

### [partition](docs/sdks/partition/README.md)

* [createPartition](docs/sdks/partition/README.md#createpartition) - Create Partition
* [searchPartitions](docs/sdks/partition/README.md#searchpartitions) - Search Partitions

### [query](docs/sdks/query/README.md)

* [askQuestionSetNumberOfContextDocs](docs/sdks/query/README.md#askquestionsetnumberofcontextdocs) - Ask Question set number of context docs
<!-- End SDK Available Operations -->



<!-- Start Dev Containers -->

<!-- End Dev Containers -->



<!-- Start Pagination -->
# Pagination

Some of the endpoints in this SDK support pagination. To use pagination, you make your SDK calls as usual, but the
returned response object will have a `next` method that can be called to pull down the next group of results. If the
return value of `next` is `null`, then there are no more pages to be fetched.

Here's an example of one such pagination call:
<!-- End Pagination -->

<!-- Placeholder for Future Speakeasy SDK Sections -->



### Maturity

This SDK is in beta, and there may be breaking changes between versions without a major version update. Therefore, we recommend pinning usage
to a specific package version. This way, you can install the same version each time without breaking changes unless you are intentionally
looking for the latest version.

### Contributions

While we value open-source contributions to this SDK, this library is generated programmatically.
Feel free to open a PR or a Github issue as a proof of concept and we'll do our best to include it in a future release!

### SDK Created by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/client-sdks)
