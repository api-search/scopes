---
authorization_urls: []
description: ''
docs: https://octopus.com/docs/octopus-rest-api/openid-connect
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Octopus Deploy Scopes
name_suffix: OAuth Scopes
note: Octopus Deploy does not use OAuth scopes; the OIDC client_credentials exchange only validates a service account identity, and API access is authorized by the service account's team and role permissions (or an API key) per https://octopus.com/docs/octopus-rest-api/openid-connect.
overview: 'Octopus Deploy uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://your-octopus-instance/api/oidc/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Octopus Deploy
provider_slug: octopus-deploy
schemes:
- description: 'Authenticate by exchanging an OpenID Connect identity token from

    a trusted external system (for example GitHub Actions) for a

    short-lived Octopus access token.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://your-octopus-instance/api/oidc/token
  name: OidcAuth
  source: openapi/octopus-deploy-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: octopus-deploy-scopes
source_filename: octopus-deploy-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/octopus-deploy-openapi.yml\ndocs: https://octopus.com/docs/octopus-rest-api/openid-connect\nnote: >-\n  Octopus Deploy does not use OAuth scopes; the OIDC client_credentials\n  exchange only validates a service account identity, and API access is\n  authorized by the service account's team and role permissions (or an\n  API key) per https://octopus.com/docs/octopus-rest-api/openid-connect.\nschemes:\n- name: OidcAuth\n  source: openapi/octopus-deploy-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://your-octopus-instance/api/oidc/token\n  description: |-\n    Authenticate by exchanging an OpenID Connect identity token from\n    a trusted external system (for example GitHub Actions) for a\n    short-lived Octopus access token.\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/octopus-deploy/refs/heads/main/scopes/octopus-deploy-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- DevOps
- Continuous Delivery
- Deployment Automation
- Release Management
- Runbooks
- CI/CD
token_urls:
- https://your-octopus-instance/api/oidc/token
---
