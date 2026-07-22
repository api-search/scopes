---
authorization_urls: []
description: RightRev authenticates through a per-tenant Keycloak (OpenID Connect) realm. The documented token response grants the standard OIDC identity scopes; API authorization beyond identity is governed by tenant/user role assignment rather than fine-grained OAuth scopes.
docs: https://apis.rightrev.com/getting-started/authentication.md
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Rightrev Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Rightrev publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Rightrev API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Rightrev
provider_slug: rightrev
schemes:
- docs: https://apis.rightrev.com/getting-started/authentication.md
  grant_types:
  - password
  - implicit
  name: RightRev OIDC (Keycloak)
  tokenUrl: https://auth.rightrev.cloud/auth/realms/<tenant_id>/protocol/openid-connect/token
  type: oauth2
scope_count: 2
scope_names:
- profile
- email
scopes:
- description: Standard OpenID Connect profile claims for the authenticated user.
  flows: []
  scope: profile
- description: Standard OpenID Connect email claim for the authenticated user.
  flows: []
  scope: email
slug: rightrev-scopes
source_filename: rightrev-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: >-\n  https://apis.rightrev.com/getting-started/authentication.md — the documented\n  token response returns scope \"profile email\". RightRev publishes no OpenAPI\n  oauth2 securityScheme, so these are the OpenID Connect scopes observed in the\n  Keycloak token response rather than a derived spec baseline.\ndocs: https://apis.rightrev.com/getting-started/authentication.md\ndescription: >-\n  RightRev authenticates through a per-tenant Keycloak (OpenID Connect) realm.\n  The documented token response grants the standard OIDC identity scopes; API\n  authorization beyond identity is governed by tenant/user role assignment\n  rather than fine-grained OAuth scopes.\nschemes:\n- name: RightRev OIDC (Keycloak)\n  type: oauth2\n  grant_types: [password, implicit]\n  tokenUrl: https://auth.rightrev.cloud/auth/realms/<tenant_id>/protocol/openid-connect/token\n  docs: https://apis.rightrev.com/getting-started/authentication.md\nscopes:\n\
  - scope: profile\n  description: Standard OpenID Connect profile claims for the authenticated user.\n- scope: email\n  description: Standard OpenID Connect email claim for the authenticated user.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rightrev/refs/heads/main/scopes/rightrev-scopes.yml
summary_line: 2 scopes
tags:
- Company
- Revenue Recognition
- Accounting
- Finance
- Billing
- ASC 606
- IFRS 15
- Revenue
- SaaS Metrics
token_urls: []
---
