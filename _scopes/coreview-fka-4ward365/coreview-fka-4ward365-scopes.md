---
authorization_urls: []
description: ''
docs: https://help.coreview.com/api-authentication
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Coreview Fka 4Ward365 Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'CoreView (FKA 4ward365) publishes 14 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the CoreView (FKA 4ward365) API on a user''s behalf.


  Tokens are issued from https://identity.coreview.com/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CoreView (FKA 4ward365)
provider_slug: coreview-fka-4ward365
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://identity.coreview.com/connect/token
  name: OAuth2ClientCredentials
  source: https://help.coreview.com/api-authentication
scope_count: 14
scope_names:
- customer.read
- customer.write
- delegation.read
- delegation.write
- operator.read
- operator.write
- platform.read
- licensepool.read
- licensepool.write
- license.read
- openid
- profile
- email
- offline_access
scopes:
- description: Read access to customer/tenant configuration.
  flows:
  - clientCredentials
  scope: customer.read
- description: Manage customer/tenant configuration.
  flows:
  - clientCredentials
  scope: customer.write
- description: Read delegated administration assignments and roles.
  flows:
  - clientCredentials
  scope: delegation.read
- description: Manage delegated administration assignments and roles.
  flows:
  - clientCredentials
  scope: delegation.write
- description: Read operator (administrator) accounts and their permissions.
  flows:
  - clientCredentials
  scope: operator.read
- description: Manage operator (administrator) accounts and their permissions.
  flows:
  - clientCredentials
  scope: operator.write
- description: Read platform-level reporting and governance data.
  flows:
  - clientCredentials
  scope: platform.read
- description: Read Microsoft 365 license pool allocations.
  flows:
  - clientCredentials
  scope: licensepool.read
- description: Manage Microsoft 365 license pool allocations.
  flows:
  - clientCredentials
  scope: licensepool.write
- description: Read Microsoft 365 license assignments and inventory.
  flows:
  - clientCredentials
  scope: license.read
- description: Standard OpenID Connect scope requesting an ID token.
  flows:
  - clientCredentials
  scope: openid
- description: Standard OpenID Connect profile claims.
  flows:
  - clientCredentials
  scope: profile
- description: Standard OpenID Connect email claim.
  flows:
  - clientCredentials
  scope: email
- description: Request a refresh token for long-lived access.
  flows:
  - clientCredentials
  scope: offline_access
slug: coreview-fka-4ward365-scopes
source_filename: coreview-fka-4ward365-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://identity.coreview.com/.well-known/openid-configuration\ndocs: https://help.coreview.com/api-authentication\nschemes:\n- name: OAuth2ClientCredentials\n  source: https://help.coreview.com/api-authentication\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://identity.coreview.com/connect/token\nscopes:\n- scope: customer.read\n  description: Read access to customer/tenant configuration.\n  flows: [clientCredentials]\n- scope: customer.write\n  description: Manage customer/tenant configuration.\n  flows: [clientCredentials]\n- scope: delegation.read\n  description: Read delegated administration assignments and roles.\n  flows: [clientCredentials]\n- scope: delegation.write\n  description: Manage delegated administration assignments and roles.\n  flows: [clientCredentials]\n- scope: operator.read\n  description: Read operator (administrator) accounts and their permissions.\n  flows: [clientCredentials]\n- scope:\
  \ operator.write\n  description: Manage operator (administrator) accounts and their permissions.\n  flows: [clientCredentials]\n- scope: platform.read\n  description: Read platform-level reporting and governance data.\n  flows: [clientCredentials]\n- scope: licensepool.read\n  description: Read Microsoft 365 license pool allocations.\n  flows: [clientCredentials]\n- scope: licensepool.write\n  description: Manage Microsoft 365 license pool allocations.\n  flows: [clientCredentials]\n- scope: license.read\n  description: Read Microsoft 365 license assignments and inventory.\n  flows: [clientCredentials]\n- scope: openid\n  description: Standard OpenID Connect scope requesting an ID token.\n  flows: [clientCredentials]\n- scope: profile\n  description: Standard OpenID Connect profile claims.\n  flows: [clientCredentials]\n- scope: email\n  description: Standard OpenID Connect email claim.\n  flows: [clientCredentials]\n- scope: offline_access\n  description: Request a refresh token for long-lived\
  \ access.\n  flows: [clientCredentials]\nnotes: >-\n  Scope names are taken verbatim from the CoreView OIDC discovery document\n  (scopes_supported) and the API authentication documentation. Descriptions are\n  derived from the scope naming (resource.read / resource.write) and CoreView's\n  documented delegation, operator, platform, and license-management domains.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coreview-fka-4ward365/refs/heads/main/scopes/coreview-fka-4ward365-scopes.yml
summary_line: 14 scopes · clientCredentials
tags:
- Company
- Microsoft 365
- SaaS Management
- Governance
- Security
- Identity
- Automation
- Workflow
- License Management
- IT Operations
token_urls:
- https://identity.coreview.com/connect/token
---
