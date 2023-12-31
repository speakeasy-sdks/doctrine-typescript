# Doctrine

<!-- Start SDK Installation [installation] -->
## SDK Installation

### NPM

```bash
npm add https://github.com/speakeasy-sdks/doctrine-typescript
```

### Yarn

```bash
yarn add https://github.com/speakeasy-sdks/doctrine-typescript
```
<!-- End SDK Installation [installation] -->

<!-- Start SDK Example Usage [usage] -->
## SDK Example Usage

### Example

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

<!-- Start Available Resources and Operations [operations] -->
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
<!-- End Available Resources and Operations [operations] -->







<!-- Start Error Handling [errors] -->
## Error Handling

Handling errors in this SDK should largely match your expectations.  All operations return a response object or throw an error.  If Error objects are specified in your OpenAPI Spec, the SDK will throw the appropriate Error type.

| Error Object    | Status Code     | Content Type    |
| --------------- | --------------- | --------------- |
| errors.SDKError | 4xx-5xx         | */*             |

Example

```typescript
import { Doctrine } from "Doctrine";

async function run() {
    const sdk = new Doctrine();

    let res;
    try {
        res = await sdk.httpLocalhost3000ApiScanpagecontent({
            url: "https://sardelkitchen.com/products/chili-infused-olive-oil",
        });
    } catch (err) {
        if (err instanceof errors.SDKError) {
            console.error(err); // handle exception
            throw err;
        }
    }

    if (res.statusCode == 200) {
        // handle response
    }
}

run();

```
<!-- End Error Handling [errors] -->



<!-- Start Server Selection [server] -->
## Server Selection

### Select Server by Index

You can override the default server globally by passing a server index to the `serverIdx: number` optional parameter when initializing the SDK client instance. The selected server will then be used as the default on the operations that use it. This table lists the indexes associated with the available servers:

| # | Server | Variables |
| - | ------ | --------- |
| 0 | `http://localhost` | None |

#### Example

```typescript
import { Doctrine } from "Doctrine";

async function run() {
    const sdk = new Doctrine({
        serverIdx: 0,
    });

    const res = await sdk.httpLocalhost3000ApiScanpagecontent({
        url: "https://sardelkitchen.com/products/chili-infused-olive-oil",
    });

    if (res.statusCode == 200) {
        // handle response
    }
}

run();

```


### Override Server URL Per-Client

The default server can also be overridden globally by passing a URL to the `serverURL: str` optional parameter when initializing the SDK client instance. For example:
```typescript
import { Doctrine } from "Doctrine";

async function run() {
    const sdk = new Doctrine({
        serverURL: "http://localhost",
    });

    const res = await sdk.httpLocalhost3000ApiScanpagecontent({
        url: "https://sardelkitchen.com/products/chili-infused-olive-oil",
    });

    if (res.statusCode == 200) {
        // handle response
    }
}

run();

```
<!-- End Server Selection [server] -->



<!-- Start Custom HTTP Client [http-client] -->
## Custom HTTP Client

The Typescript SDK makes API calls using the [axios](https://axios-http.com/docs/intro) HTTP library.  In order to provide a convenient way to configure timeouts, cookies, proxies, custom headers, and other low-level configuration, you can initialize the SDK client with a custom `AxiosInstance` object.

For example, you could specify a header for every request that your sdk makes as follows:

```typescript
import { Doctrine } from "Doctrine";
import axios from "axios";

const httpClient = axios.create({
    headers: {'x-custom-header': 'someValue'}
})

const sdk = new Doctrine({defaultClient: httpClient});
```
<!-- End Custom HTTP Client [http-client] -->

<!-- Placeholder for Future Speakeasy SDK Sections -->



### Maturity

This SDK is in beta, and there may be breaking changes between versions without a major version update. Therefore, we recommend pinning usage
to a specific package version. This way, you can install the same version each time without breaking changes unless you are intentionally
looking for the latest version.

### Contributions

While we value open-source contributions to this SDK, this library is generated programmatically.
Feel free to open a PR or a Github issue as a proof of concept and we'll do our best to include it in a future release!

### SDK Created by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/client-sdks)
