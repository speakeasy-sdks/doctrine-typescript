# Partition
(*partition*)

### Available Operations

* [createPartition](#createpartition) - Create Partition
* [searchPartitions](#searchpartitions) - Search Partitions

## createPartition

Create Partition

### Example Usage

```typescript
import { Doctrine } from "Doctrine";

async function run() {
  const sdk = new Doctrine();

  const res = await sdk.partition.createPartition({
    name: "Sample part",
  });

  if (res.statusCode == 200) {
    // handle response
  }
}

run();
```

### Parameters

| Parameter                                                                                          | Type                                                                                               | Required                                                                                           | Description                                                                                        |
| -------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- |
| `request`                                                                                          | [operations.CreatePartitionRequestBody](../../sdk/models/operations/createpartitionrequestbody.md) | :heavy_check_mark:                                                                                 | The request object to use for the request.                                                         |
| `config`                                                                                           | [AxiosRequestConfig](https://axios-http.com/docs/req_config)                                       | :heavy_minus_sign:                                                                                 | Available config options for making requests.                                                      |


### Response

**Promise<[operations.CreatePartitionResponse](../../sdk/models/operations/createpartitionresponse.md)>**
### Errors

| Error Object    | Status Code     | Content Type    |
| --------------- | --------------- | --------------- |
| errors.SDKError | 4xx-5xx         | */*             |

## searchPartitions

Search Partitions

### Example Usage

```typescript
import { Doctrine } from "Doctrine";

async function run() {
  const sdk = new Doctrine();

  const res = await sdk.partition.searchPartitions({
    searchValue: "metadata",
  });

  if (res.statusCode == 200) {
    // handle response
  }
}

run();
```

### Parameters

| Parameter                                                                                    | Type                                                                                         | Required                                                                                     | Description                                                                                  |
| -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
| `request`                                                                                    | [operations.SearchPartitionsRequest](../../sdk/models/operations/searchpartitionsrequest.md) | :heavy_check_mark:                                                                           | The request object to use for the request.                                                   |
| `config`                                                                                     | [AxiosRequestConfig](https://axios-http.com/docs/req_config)                                 | :heavy_minus_sign:                                                                           | Available config options for making requests.                                                |


### Response

**Promise<[operations.SearchPartitionsResponse](../../sdk/models/operations/searchpartitionsresponse.md)>**
### Errors

| Error Object    | Status Code     | Content Type    |
| --------------- | --------------- | --------------- |
| errors.SDKError | 4xx-5xx         | */*             |
