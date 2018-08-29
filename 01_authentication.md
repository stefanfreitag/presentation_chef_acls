## Authentication


## Authentication

- Communication with Chef server must be authenticated
- Chef server responds only to requests made by trusted users
- Only authenticated requests will be authorized


## Authentication

- Implementation uses public key encryption, e.g.
  - Public key is stored on the Chef server
  - Private key (.pem file) is returned to the user for safe keeping