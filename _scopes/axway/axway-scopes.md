---
api_specs:
- filename: axway-aca-api-openapi.yml
  format: yaml
  label: Axway aca API
  slug: axway-aca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axway/refs/heads/main/openapi/axway-aca-api-openapi.yml
- filename: axway-activity-api-openapi.yml
  format: yaml
  label: Axway activity API
  slug: axway-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axway/refs/heads/main/openapi/axway-activity-api-openapi.yml
- filename: axway-analytics-api-openapi.yml
  format: yaml
  label: Axway analytics API
  slug: axway-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axway/refs/heads/main/openapi/axway-analytics-api-openapi.yml
- filename: axway-app-api-openapi.yml
  format: yaml
  label: Axway app API
  slug: axway-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axway/refs/heads/main/openapi/axway-app-api-openapi.yml
- filename: axway-auth-api-openapi.yml
  format: yaml
  label: Axway auth API
  slug: axway-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axway/refs/heads/main/openapi/axway-auth-api-openapi.yml
- filename: axway-client-api-openapi.yml
  format: yaml
  label: Axway client API
  slug: axway-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axway/refs/heads/main/openapi/axway-client-api-openapi.yml
- filename: axway-domain-api-openapi.yml
  format: yaml
  label: Axway domain API
  slug: axway-domain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axway/refs/heads/main/openapi/axway-domain-api-openapi.yml
- filename: axway-entitlement-api-openapi.yml
  format: yaml
  label: Axway entitlement API
  slug: axway-entitlement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axway/refs/heads/main/openapi/axway-entitlement-api-openapi.yml
- filename: axway-env-api-openapi.yml
  format: yaml
  label: Axway env API
  slug: axway-env-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axway/refs/heads/main/openapi/axway-env-api-openapi.yml
- filename: axway-export-api-openapi.yml
  format: yaml
  label: Axway export API
  slug: axway-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axway/refs/heads/main/openapi/axway-export-api-openapi.yml
- filename: axway-idp-api-openapi.yml
  format: yaml
  label: Axway idp API
  slug: axway-idp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axway/refs/heads/main/openapi/axway-idp-api-openapi.yml
- filename: axway-org-api-openapi.yml
  format: yaml
  label: Axway org API
  slug: axway-org-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axway/refs/heads/main/openapi/axway-org-api-openapi.yml
- filename: axway-provider-api-openapi.yml
  format: yaml
  label: Axway provider API
  slug: axway-provider-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axway/refs/heads/main/openapi/axway-provider-api-openapi.yml
- filename: axway-role-api-openapi.yml
  format: yaml
  label: Axway role API
  slug: axway-role-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axway/refs/heads/main/openapi/axway-role-api-openapi.yml
- filename: axway-session-api-openapi.yml
  format: yaml
  label: Axway session API
  slug: axway-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axway/refs/heads/main/openapi/axway-session-api-openapi.yml
- filename: axway-subscription-api-openapi.yml
  format: yaml
  label: Axway subscription API
  slug: axway-subscription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axway/refs/heads/main/openapi/axway-subscription-api-openapi.yml
- filename: axway-team-api-openapi.yml
  format: yaml
  label: Axway team API
  slug: axway-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axway/refs/heads/main/openapi/axway-team-api-openapi.yml
- filename: axway-telemetry-api-openapi.yml
  format: yaml
  label: Axway telemetry API
  slug: axway-telemetry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axway/refs/heads/main/openapi/axway-telemetry-api-openapi.yml
- filename: axway-usage-api-openapi.yml
  format: yaml
  label: Axway usage API
  slug: axway-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axway/refs/heads/main/openapi/axway-usage-api-openapi.yml
- filename: axway-user-api-openapi.yml
  format: yaml
  label: Axway user API
  slug: axway-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axway/refs/heads/main/openapi/axway-user-api-openapi.yml
authorization_urls:
- https://login.axway.com/auth/realms/Broker/openid-connect/auth
description: ''
docs: https://blog.axway.com/product-insights/amplify-platform/axway-amplify-platform-api-calls
flows:
- clientCredentials
- authorizationCode
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Axway Scopes
name_suffix: OAuth Scopes
note: Axway does not publish OAuth scopes for the Amplify Platform API; authorization is handled through org roles assigned to client-secret service accounts, and tokens carry only generic OIDC scopes (see https://blog.axway.com/product-insights/amplify-platform/axway-amplify-platform-api-calls).
overview: 'Axway uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://login.axway.com/auth/realms/Broker/protocol/openid-connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Axway
provider_slug: axway
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://login.axway.com/auth/realms/Broker/protocol/openid-connect/token
  - authorizationUrl: https://login.axway.com/auth/realms/Broker/openid-connect/auth
    flow: authorizationCode
    tokenUrl: https://login.axway.com/auth/realms/Broker/openid-connect/token
  - authorizationUrl: https://login.axway.com/auth/realms/Broker/openid-connect/auth
    flow: implicit
  name: OAuth2
  source: openapi/axway-amplify-platform-openapi-original.json
scope_count: 0
scope_names: []
scopes: []
slug: axway-scopes
source_filename: axway-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/axway-amplify-platform-openapi-original.json\ndocs: https://blog.axway.com/product-insights/amplify-platform/axway-amplify-platform-api-calls\nnote: >-\n  Axway does not publish OAuth scopes for the Amplify Platform API; authorization is\n  handled through org roles assigned to client-secret service accounts, and tokens carry\n  only generic OIDC scopes (see\n  https://blog.axway.com/product-insights/amplify-platform/axway-amplify-platform-api-calls).\nschemes:\n- name: OAuth2\n  source: openapi/axway-amplify-platform-openapi-original.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.axway.com/auth/realms/Broker/protocol/openid-connect/token\n  - flow: authorizationCode\n    authorizationUrl: https://login.axway.com/auth/realms/Broker/openid-connect/auth\n    tokenUrl: https://login.axway.com/auth/realms/Broker/openid-connect/token\n  - flow: implicit\n    authorizationUrl: https://login.axway.com/auth/realms/Broker/openid-connect/auth\n\
  scopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/axway/refs/heads/main/scopes/axway-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- API Management
- Enterprise
- Integration
- Security
token_urls:
- https://login.axway.com/auth/realms/Broker/protocol/openid-connect/token
- https://login.axway.com/auth/realms/Broker/openid-connect/token
---
