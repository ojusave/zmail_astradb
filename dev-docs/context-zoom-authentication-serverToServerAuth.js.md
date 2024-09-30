

---
# High Level Context
## context
**Last Updated at:** 9/30/2024, 8:04:16 PM

Summary:
This code file implements a server-to-server OAuth authentication mechanism for Zoom API. It manages token generation, caching, and automatic renewal when the token expires.

Main object: Module exports

Methods:

1. getToken()

Description: Retrieves an access token for Zoom API authentication. It caches the token and returns the cached version if it's still valid.

Example usage:
```javascript
const { getToken } = require('./serverToServerAuth');

async function makeZoomApiCall() {
  try {
    const token = await getToken();
    // Use the token for Zoom API requests
    // ...
  } catch (error) {
    console.error('Failed to get token:', error);
  }
}
```

Note: This is the only public method exported by the module.

Internal variables:

- cachedToken: Stores the current access token
- tokenExpiration: Stores the expiration date of the current token

The module uses environment variables for sensitive information:
- OAuth_Client_ID
- OAuth_Client_Secret
- ZOOM_ACCOUNT_ID

These should be set in a .env file or in the server's environment.
