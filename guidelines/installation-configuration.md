# Installation & configuration 

## Default enviroment is Personal

![environment-naming-admin](/assets/environment-naming-admin.png)

## Deployment stratagy for customer type 1


## Security

Non-interactive:

- Poor: Connection string
- Less poor: Encrypted string
- Slightly Better: Non-interactive user
- Best: App service
- Bester: ClientId + Secret
- Bestest: Certificate-based
- Bonus points: Azure Vault
- Medal: Managed Identities

Interactive:

- Passive
  - Poor: Connection string
  - Still poor: Encrypted connection string
  - Better: Connection string deployed as part of Azure app
  - Best: Registered app
  - Best: OAuth if impersonation is required

- Active
  - Poor: Connection string
  - Better: Prompt for password
  - Better: Use registered app
  - Best: Xrm.Tooling