##  Authentication


##  Authentication

- Communication with Chef server must be authenticated
- Ensures that the Chef server responds only to requests made by trusted users
- Only authenticated requests will be authorized
- Implementation uses public key encryption


##  Authentication

- When a node and/or a workstation is configured to run the chef-client, public and private keys are created
  - Public key is stored on the Chef server
  - Private key (.pem file) is returned to the user for safe keeping