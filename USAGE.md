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