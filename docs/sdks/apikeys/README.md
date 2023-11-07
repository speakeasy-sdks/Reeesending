# APIKeys
(*.apiKeys*)

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

(async() => {
  const sdk = new Reeesending({
    bearerAuth: "",
  });

  const res = await sdk.apiKeys.deleteApiKeysApiKeyId({
    apiKeyId: "string",
  });


  if (res.statusCode == 200) {
    // handle response
  }
})();
```

### Parameters

| Parameter                                                                                          | Type                                                                                               | Required                                                                                           | Description                                                                                        |
| -------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- |
| `request`                                                                                          | [operations.DeleteApiKeysApiKeyIdRequest](../../models/operations/deleteapikeysapikeyidrequest.md) | :heavy_check_mark:                                                                                 | The request object to use for the request.                                                         |
| `config`                                                                                           | [AxiosRequestConfig](https://axios-http.com/docs/req_config)                                       | :heavy_minus_sign:                                                                                 | Available config options for making requests.                                                      |


### Response

**Promise<[operations.DeleteApiKeysApiKeyIdResponse](../../models/operations/deleteapikeysapikeyidresponse.md)>**


## getApiKeys

Retrieve a list of API keys

### Example Usage

```typescript
import { Reeesending } from "Reeesending";

(async() => {
  const sdk = new Reeesending({
    bearerAuth: "",
  });

  const res = await sdk.apiKeys.getApiKeys();


  if (res.statusCode == 200) {
    // handle response
  }
})();
```

### Parameters

| Parameter                                                    | Type                                                         | Required                                                     | Description                                                  |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| `config`                                                     | [AxiosRequestConfig](https://axios-http.com/docs/req_config) | :heavy_minus_sign:                                           | Available config options for making requests.                |


### Response

**Promise<[operations.GetApiKeysResponse](../../models/operations/getapikeysresponse.md)>**


## postApiKeys

Create a new API key

### Example Usage

```typescript
import { Reeesending } from "Reeesending";
import { Permission } from "Reeesending/dist/sdk/models/shared";

(async() => {
  const sdk = new Reeesending({
    bearerAuth: "",
  });

  const res = await sdk.apiKeys.postApiKeys({
    name: "string",
  });


  if (res.statusCode == 200) {
    // handle response
  }
})();
```

### Parameters

| Parameter                                                                | Type                                                                     | Required                                                                 | Description                                                              |
| ------------------------------------------------------------------------ | ------------------------------------------------------------------------ | ------------------------------------------------------------------------ | ------------------------------------------------------------------------ |
| `request`                                                                | [shared.CreateApiKeyRequest](../../models/shared/createapikeyrequest.md) | :heavy_check_mark:                                                       | The request object to use for the request.                               |
| `config`                                                                 | [AxiosRequestConfig](https://axios-http.com/docs/req_config)             | :heavy_minus_sign:                                                       | Available config options for making requests.                            |


### Response

**Promise<[operations.PostApiKeysResponse](../../models/operations/postapikeysresponse.md)>**

