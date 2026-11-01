---
authorization_urls: []
description: ''
docs: https://docs.mapped.com/guides/platform/authentication-security.md
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Mapped Com Scopes
name_suffix: OAuth Scopes
note: Scopes are used for Personal Access Token permissions, not OAuth2. Documentation mentions scopes are role-dependent (ADMIN vs EXPLORER). EXPLORER role has read-only access to most resources.
overview: 'Mapped publishes 9 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Mapped API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Mapped
provider_slug: mapped-com
schemes: []
scope_count: 9
scope_names:
- PERSONALACCESSTOKEN_READ
- PERSONALACCESSTOKEN_READ_ALL
- PERSONALACCESSTOKEN_READWRITE
- PERSONALACCESSTOKEN_READWRITE_ALL
- ORG_READ
- USER_READ
- PLACE_READ_ALL
- THING_READ_ALL
- USER_READ_ALL
scopes:
- description: Read personal access tokens for your own user
  flows: []
  scope: PERSONALACCESSTOKEN_READ
- description: Read personal access tokens for all users (ADMIN only)
  flows: []
  scope: PERSONALACCESSTOKEN_READ_ALL
- description: Create and manage your own personal access tokens
  flows: []
  scope: PERSONALACCESSTOKEN_READWRITE
- description: Create and manage personal access tokens for all users (ADMIN only)
  flows: []
  scope: PERSONALACCESSTOKEN_READWRITE_ALL
- description: Read organization information
  flows: []
  scope: ORG_READ
- description: Read user information
  flows: []
  scope: USER_READ
- description: Read all place information
  flows: []
  scope: PLACE_READ_ALL
- description: Read all thing information
  flows: []
  scope: THING_READ_ALL
- description: Read all user information
  flows: []
  scope: USER_READ_ALL
slug: mapped-com-scopes
source_filename: mapped-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: searched\nsource: https://docs.mapped.com/guides/platform/authentication-security.md\ndocs: https://docs.mapped.com/guides/platform/authentication-security.md\nscopes:\n- scope: PERSONALACCESSTOKEN_READ\n  description: Read personal access tokens for your own user\n  evidence: \"To view all tokens associated with your user, you'll need a token with the scope PERSONALACCESSTOKEN_READ.\"\n- scope: PERSONALACCESSTOKEN_READ_ALL\n  description: Read personal access tokens for all users (ADMIN only)\n  evidence: \"If you want to view all tokens associated with a particular user, you'll need to be an ADMIN and have a token with the scope PERSONALACCESSTOKEN_READ_ALL\"\n- scope: PERSONALACCESSTOKEN_READWRITE\n  description: Create and manage your own personal access tokens\n  evidence: \"If the token you're using to make API calls has the PERSONALACCESSTOKEN_READWRITE (or PERSONALACCESSTOKEN_READWRITE_ALL for an ADMIN), you can create a new token programmatically.\"\
  \n- scope: PERSONALACCESSTOKEN_READWRITE_ALL\n  description: Create and manage personal access tokens for all users (ADMIN only)\n  evidence: \"If you're an ADMIN and your token has the permission PERSONALACCESSTOKEN_READWRITE_ALL, then you can remove a token from anyone in your organization.\"\n- scope: ORG_READ\n  description: Read organization information\n  evidence: \"The following example creates a token with the ORG_READ and USER_READ permissions\"\n- scope: USER_READ\n  description: Read user information\n  evidence: \"The following example creates a token with the ORG_READ and USER_READ permissions\"\n- scope: PLACE_READ_ALL\n  description: Read all place information\n  evidence: Found in example response showing permissions array\n- scope: THING_READ_ALL\n  description: Read all thing information\n  evidence: Found in example response showing permissions array\n- scope: USER_READ_ALL\n  description: Read all user information\n  evidence: Found in example response showing permissions\
  \ array\nnote: Scopes are used for Personal Access Token permissions, not OAuth2. Documentation mentions scopes are role-dependent (ADMIN vs EXPLORER). EXPLORER role has read-only access to most resources."
source_yaml_url: https://artifacts.apis.io/mapped-com/scopes/mapped-com-scopes.yml
summary_line: 9 scopes
tags:
- Company
- Smart Buildings
- IoT
- GraphQL
- Data Integration
- Ontology
- Physical AI
- MCP
token_bound: false
token_urls: []
---
