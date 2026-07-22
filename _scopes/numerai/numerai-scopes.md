---
authorization_urls: []
description: ''
docs: https://docs.numer.ai/numerai-tournament/automation/automation-legacy
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Numerai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Numerai publishes 8 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Numerai API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Numerai
provider_slug: numerai
schemes:
- in: header
  key_headers:
  - x-public-id
  - x-secret-key
  name: ApiToken
  source: https://api-tournament.numer.ai
  type: apiKey
scope_count: 8
scope_names:
- write_user_info
- upload_submission
- download_submission
- stake
- web3_staking
- read_submission_info
- read_user_info
- delete
scopes:
- description: Update account and model profile information
  flows: []
  scope: write_user_info
- description: Upload submissions and pickled models
  flows: []
  scope: upload_submission
- description: Download previous submissions and pickled models.
  flows: []
  scope: download_submission
- description: Make stakes
  flows: []
  scope: stake
- description: Manage web3 staking
  flows: []
  scope: web3_staking
- description: View historical submission info
  flows: []
  scope: read_submission_info
- description: View user info, (e.g. balance, withdrawal history)
  flows: []
  scope: read_user_info
- description: Ability to delete your models and your account.
  flows: []
  scope: delete
slug: numerai-scopes
source_filename: numerai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://api-tournament.numer.ai (apiTokenScopes query, live introspection)\ndocs: https://docs.numer.ai/numerai-tournament/automation/automation-legacy\nmodel: API token scopes (public key + secret key pair). Scopes are selected when creating an API token in Account > Settings;\n  tokens are passed as x-public-id / x-secret-key headers to the GraphQL API.\nschemes:\n- name: ApiToken\n  type: apiKey\n  in: header\n  key_headers:\n  - x-public-id\n  - x-secret-key\n  source: https://api-tournament.numer.ai\nscopes:\n- scope: write_user_info\n  description: Update account and model profile information\n- scope: upload_submission\n  description: Upload submissions and pickled models\n- scope: download_submission\n  description: Download previous submissions and pickled models.\n- scope: stake\n  description: Make stakes\n- scope: web3_staking\n  description: Manage web3 staking\n- scope: read_submission_info\n  description: View\
  \ historical submission info\n- scope: read_user_info\n  description: View user info, (e.g. balance, withdrawal history)\n- scope: delete\n  description: Ability to delete your models and your account.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/numerai/refs/heads/main/scopes/numerai-scopes.yml
summary_line: 8 scopes
tags:
- Company
- Fintech
- Machine Learning
- Data Science
- Hedge Fund
- GraphQL
- Crypto
- Quantitative Finance
- Tournament
- API
token_urls: []
---
