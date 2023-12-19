# APIKeys
(*apiKeys*)

## Overview

Create and manage API Keys through the Reeesending Test API.

### Available Operations

* [deleteApiKeysApiKeyId](#deleteapikeysapikeyid) - Remove an existing API key
* [getApiKeys](#getapikeys) - Retrieve a list of API keys
* [postApiKeys](#postapikeys) - Create a new API key

## deleteApiKeysApiKeyId

Remove an existing API key

### Example Usage

```typescript
import { Reeesending } from "Reeesending";

async function run() {
  const sdk = new Reeesending({
    bearerAuth: "<YOUR_BEARER_TOKEN_HERE>",
  });

  const res = await sdk.apiKeys.deleteApiKeysApiKeyId({
    apiKeyId: "string",
  });

  if (res.statusCode == 200) {
    // handle response
  }
}

run();
```

### Parameters

| Parameter                                                                                              | Type                                                                                                   | Required                                                                                               | Description                                                                                            |
| ------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------ |
| `request`                                                                                              | [operations.DeleteApiKeysApiKeyIdRequest](../../sdk/models/operations/deleteapikeysapikeyidrequest.md) | :heavy_check_mark:                                                                                     | The request object to use for the request.                                                             |
| `config`                                                                                               | [AxiosRequestConfig](https://axios-http.com/docs/req_config)                                           | :heavy_minus_sign:                                                                                     | Available config options for making requests.                                                          |


### Response

**Promise<[operations.DeleteApiKeysApiKeyIdResponse](../../sdk/models/operations/deleteapikeysapikeyidresponse.md)>**
### Errors

| Error Object    | Status Code     | Content Type    |
| --------------- | --------------- | --------------- |
| errors.SDKError | 4xx-5xx         | */*             |

## getApiKeys

Retrieve a list of API keys

### Example Usage

```typescript
import { Reeesending } from "Reeesending";

async function run() {
  const sdk = new Reeesending({
    bearerAuth: "<YOUR_BEARER_TOKEN_HERE>",
  });

  const res = await sdk.apiKeys.getApiKeys();

  if (res.statusCode == 200) {
    // handle response
  }
}

run();
```

### Parameters

| Parameter                                                    | Type                                                         | Required                                                     | Description                                                  |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| `config`                                                     | [AxiosRequestConfig](https://axios-http.com/docs/req_config) | :heavy_minus_sign:                                           | Available config options for making requests.                |


### Response

**Promise<[operations.GetApiKeysResponse](../../sdk/models/operations/getapikeysresponse.md)>**
### Errors

| Error Object    | Status Code     | Content Type    |
| --------------- | --------------- | --------------- |
| errors.SDKError | 4xx-5xx         | */*             |

## postApiKeys

Create a new API key

### Example Usage

```typescript
import { Reeesending } from "Reeesending";
import { Permission } from "Reeesending/dist/sdk/models/shared";

async function run() {
  const sdk = new Reeesending({
    bearerAuth: "<YOUR_BEARER_TOKEN_HERE>",
  });

  const res = await sdk.apiKeys.postApiKeys({
    name: "string",
  });

  if (res.statusCode == 200) {
    // handle response
  }
}

run();
```

### Parameters

| Parameter                                                                    | Type                                                                         | Required                                                                     | Description                                                                  |
| ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- |
| `request`                                                                    | [shared.CreateApiKeyRequest](../../sdk/models/shared/createapikeyrequest.md) | :heavy_check_mark:                                                           | The request object to use for the request.                                   |
| `config`                                                                     | [AxiosRequestConfig](https://axios-http.com/docs/req_config)                 | :heavy_minus_sign:                                                           | Available config options for making requests.                                |


### Response

**Promise<[operations.PostApiKeysResponse](../../sdk/models/operations/postapikeysresponse.md)>**
### Errors

| Error Object    | Status Code     | Content Type    |
| --------------- | --------------- | --------------- |
| errors.SDKError | 4xx-5xx         | */*             |
