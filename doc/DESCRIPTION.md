The secret is encrypted with a symmetric 256bit AES encryption in the browser before being sent to the server. Afterwards an URL containing the ID of the secret and the password is generated. The password is never sent to the server so the server will never be able to decrypt the secrets it delivers with a reasonable effort. Also the secret is immediately deleted on the first read.

## Features

- Secrets are encrypted with AES 256bit encryption in browser
- Server never receives the plain text secret
- Secret is deleted on first read

**Secrets are stored in memory and will be lost on restart, upgrade, or restore.**