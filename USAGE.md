<!-- Start SDK Example Usage [usage] -->
```typescript
import { Reeesending } from "Reeesending";

async function run() {
    const sdk = new Reeesending({
        bearerAuth: "<YOUR_BEARER_TOKEN_HERE>",
    });

    const res = await sdk.apiKeys.deleteApiKeysApiKeyId({
        apiKeyId: "<value>",
    });

    if (res.statusCode == 200) {
        // handle response
    }
}

run();

```
<!-- End SDK Example Usage [usage] -->