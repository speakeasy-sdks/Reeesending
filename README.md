# Reeesending

<div align="left">
    <a href="https://speakeasyapi.dev/"><img src="https://custom-icon-badges.demolab.com/badge/-Built%20By%20Speakeasy-212015?style=for-the-badge&logoColor=FBE331&logo=speakeasy&labelColor=545454" /></a>
    <a href="https://github.com/speakeasy-sdks/Reeesending.git/actions"><img src="https://img.shields.io/github/actions/workflow/status/speakeasy-sdks/Reeesending/speakeasy_sdk_generation.yml?style=for-the-badge" /></a>
    
</div>

<!-- Start SDK Installation -->
## SDK Installation

### NPM

```bash
npm add https://github.com/speakeasy-sdks/Reeesending
```

### Yarn

```bash
yarn add https://github.com/speakeasy-sdks/Reeesending
```
<!-- End SDK Installation -->

## SDK Example Usage
<!-- Start SDK Example Usage -->
```typescript
import { Reeesending } from "Reeesending";

(async () => {
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
<!-- End SDK Example Usage -->

<!-- Start SDK Available Operations -->
## Available Resources and Operations


### [apiKeys](docs/sdks/apikeys/README.md)

* [deleteApiKeysApiKeyId](docs/sdks/apikeys/README.md#deleteapikeysapikeyid) - Remove an existing API key
* [getApiKeys](docs/sdks/apikeys/README.md#getapikeys) - Retrieve a list of API keys
* [postApiKeys](docs/sdks/apikeys/README.md#postapikeys) - Create a new API key
<!-- End SDK Available Operations -->

<!-- Start Dev Containers -->

<!-- End Dev Containers -->

<!-- Placeholder for Future Speakeasy SDK Sections -->

# Development

## Maturity

This SDK is in beta, and there may be breaking changes between versions without a major version update. Therefore, we recommend pinning usage
to a specific package version. This way, you can install the same version each time without breaking changes unless you are intentionally
looking for the latest version.

## Contributions

While we value open-source contributions to this SDK, this library is generated programmatically.
Feel free to open a PR or a Github issue as a proof of concept and we'll do our best to include it in a future release!

### SDK Created by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/client-sdks)
