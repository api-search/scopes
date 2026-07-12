---
authorization_urls:
- https://us.ovhcloud.com/auth/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Ovh Cloud Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'OVH Cloud publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the OVH Cloud API on a user''s behalf.


  Tokens are issued from https://us.ovhcloud.com/auth/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: OVH Cloud
provider_slug: ovh-cloud
schemes:
- description: Oauth2
  flows:
  - authorizationUrl: https://us.ovhcloud.com/auth/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://us.ovhcloud.com/auth/oauth2/token
  name: oAuth2AuthCode
  source: openapi/ovh-cloud-openapi-original.yml
scope_count: 3
scope_names:
- account/all
- all
- services/all
scopes:
- description: Manage your account
  flows:
  - authorizationCode
  scope: account/all
- description: Manage your whole account and all your services
  flows:
  - authorizationCode
  scope: all
- description: Manage your services lifecycle and billing
  flows:
  - authorizationCode
  scope: services/all
slug: ovh-cloud-scopes
source_filename: ovh-cloud-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ovh-cloud-openapi-original.yml\nschemes:\n- name: oAuth2AuthCode\n  source: openapi/ovh-cloud-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://us.ovhcloud.com/auth/oauth2/authorize\n    tokenUrl: https://us.ovhcloud.com/auth/oauth2/token\n  description: Oauth2\nscopes:\n- scope: account/all\n  description: Manage your account\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ovh-cloud-openapi-original.yml\n- scope: all\n  description: Manage your whole account and all your services\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ovh-cloud-openapi-original.yml\n- scope: services/all\n  description: Manage your services lifecycle and billing\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ovh-cloud-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ovh-cloud/refs/heads/main/scopes/ovh-cloud-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Cloud
- Compute
- Servers
- Hosting
token_urls:
- https://us.ovhcloud.com/auth/oauth2/token
---
