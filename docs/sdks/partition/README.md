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
import { CreatePartitionResponse } from "Doctrine/dist/sdk/models/operations";

const sdk = new Doctrine();

sdk.partition.createPartition({
  name: "Sample part",
}).then((res: CreatePartitionResponse) => {
  if (res.statusCode == 200) {
    // handle response
  }
});
```

### Parameters

| Parameter                                                                                      | Type                                                                                           | Required                                                                                       | Description                                                                                    |
| ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- |
| `request`                                                                                      | [operations.CreatePartitionRequestBody](../../models/operations/createpartitionrequestbody.md) | :heavy_check_mark:                                                                             | The request object to use for the request.                                                     |
| `config`                                                                                       | [AxiosRequestConfig](https://axios-http.com/docs/req_config)                                   | :heavy_minus_sign:                                                                             | Available config options for making requests.                                                  |


### Response

**Promise<[operations.CreatePartitionResponse](../../models/operations/createpartitionresponse.md)>**


## searchPartitions

Search Partitions

### Example Usage

```typescript
import { Doctrine } from "Doctrine";
import { SearchPartitionsResponse } from "Doctrine/dist/sdk/models/operations";

const sdk = new Doctrine();

sdk.partition.searchPartitions({
  searchValue: "metadata",
}).then((res: SearchPartitionsResponse) => {
  if (res.statusCode == 200) {
    // handle response
  }
});
```

### Parameters

| Parameter                                                                                | Type                                                                                     | Required                                                                                 | Description                                                                              |
| ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- |
| `request`                                                                                | [operations.SearchPartitionsRequest](../../models/operations/searchpartitionsrequest.md) | :heavy_check_mark:                                                                       | The request object to use for the request.                                               |
| `config`                                                                                 | [AxiosRequestConfig](https://axios-http.com/docs/req_config)                             | :heavy_minus_sign:                                                                       | Available config options for making requests.                                            |


### Response

**Promise<[operations.SearchPartitionsResponse](../../models/operations/searchpartitionsresponse.md)>**

