# Project: Vault Guardian

A custodial private key solution for Ethereum-based chains that can sign transactions on the user's behalf
* Leverages [Hashicorp Vault](https://www.vaultproject.io/) to store user keys on a vault cluster, extending the Vault security model to keys managed by Guardian
* Uses a [Custom Vault Plugin](https://github.com/Lsquared13/vault-guardian-plugin) to restrict interactions to creating keys and requesting a signature on an unsigned transaction, ensuring the key is never exposed outside the Vault security barrier
* Integrates with [Okta](https://www.okta.com/) for API authorization, and uses [Okta Push Verify](https://help.okta.com/en/prod/Content/Topics/Mobile/okta-verify-overview.htm) to enforce 2FA when signing transactions

## Repositories

### Design

* [Guardian Design](https://github.com/Lsquared13/vault-guardian-design)

### Infrastructure

* [Terraform Infrastructure](https://github.com/Lsquared13/terraform-aws-vault-guardian)

### Plugin

* [Vault Plugin](https://github.com/Lsquared13/vault-guardian-plugin)