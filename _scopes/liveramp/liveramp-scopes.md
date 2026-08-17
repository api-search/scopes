---
api_specs:
- filename: liveramp-activation-api-openapi.yml
  format: yaml
  label: LiveRamp Activation API
  slug: activation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liveramp/refs/heads/main/openapi/liveramp-activation-api-openapi.yml
- filename: liveramp-clean-room-api-openapi.yml
  format: yaml
  label: LiveRamp Clean Room API
  slug: clean-room-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liveramp/refs/heads/main/openapi/liveramp-clean-room-api-openapi.yml
- filename: liveramp-privacy-api-openapi.yml
  format: yaml
  label: LiveRamp Privacy API
  slug: privacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liveramp/refs/heads/main/openapi/liveramp-privacy-api-openapi.yml
authorization_urls: []
description: ''
docs: https://developers.liveramp.com/activation-api/reference/oauth2defaultv1token
flows:
- clientCredentials
- password
kind: oauth-scopes
layout: scope
method: searched
name: Liveramp Scopes
name_suffix: OAuth Scopes
note: LiveRamp does not publish a scope/permission reference. The Clean Room API declares an oauth2 clientCredentials scheme with an EMPTY scopes map, and the LiveRamp Service Account token request documents exactly one scope value, `openid`. Authorization is carried by the service account itself (provisioned per organization by a LiveRamp representative) and by the LR-Org-Id header, not by OAuth scopes. Recorded as an honest near-absence rather than an invented scope list.
overview: 'LiveRamp publishes 1 OAuth 2.0 scope via the clientCredentials and password flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the LiveRamp API on a user''s behalf.


  Tokens are issued from https://api.habu.com/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: LiveRamp
provider_slug: liveramp
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.habu.com/v1/oauth/token
  name: application
  source: openapi/liveramp-clean-room-api-openapi.yml
- flows:
  - flow: password
    tokenUrl: https://serviceaccounts.liveramp.com/authn/v1/oauth2/token
  name: LiveRamp Service Accounts
  source: https://developers.liveramp.com/activation-api/reference/oauth2defaultv1token
scope_count: 1
scope_names:
- openid
scopes:
- description: The only scope value documented in the LiveRamp Service Account token request. Yields an OIDC id_token alongside the bearer access_token.
  flows:
  - password
  scope: openid
slug: liveramp-scopes
source_filename: liveramp-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/liveramp-clean-room-api-openapi.yml\ndocs: https://developers.liveramp.com/activation-api/reference/oauth2defaultv1token\nnote: >-\n  LiveRamp does not publish a scope/permission reference. The Clean Room API declares an oauth2\n  clientCredentials scheme with an EMPTY scopes map, and the LiveRamp Service Account token\n  request documents exactly one scope value, `openid`. Authorization is carried by the service\n  account itself (provisioned per organization by a LiveRamp representative) and by the LR-Org-Id\n  header, not by OAuth scopes. Recorded as an honest near-absence rather than an invented scope\n  list.\nschemes:\n- name: application\n  source: openapi/liveramp-clean-room-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.habu.com/v1/oauth/token\n- name: LiveRamp Service Accounts\n  source: https://developers.liveramp.com/activation-api/reference/oauth2defaultv1token\n  flows:\n\
  \  - flow: password\n    tokenUrl: https://serviceaccounts.liveramp.com/authn/v1/oauth2/token\nscopes:\n- scope: openid\n  description: >-\n    The only scope value documented in the LiveRamp Service Account token request. Yields an\n    OIDC id_token alongside the bearer access_token.\n  flows:\n  - password\n  sources:\n  - https://developers.liveramp.com/activation-api/reference/oauth2defaultv1token\nauthorization_model:\n  style: service-account\n  tenant_header: LR-Org-Id\n  description: >-\n    Access is bounded by the service account a LiveRamp representative issues, plus the LR-Org-Id\n    header that names the customer organization the call acts on behalf of. There is no\n    consent-screen scope selection surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liveramp/refs/heads/main/scopes/liveramp-scopes.yml
summary_line: 1 scope · clientCredentials/password
tags:
- Data Connectivity
- Data Collaboration
- Identity Resolution
- Activation
- Clean Room
- Privacy
- AdTech
- Marketing
- Consent
- Audience Segments
token_urls:
- https://api.habu.com/v1/oauth/token
- https://serviceaccounts.liveramp.com/authn/v1/oauth2/token
---
