---
authorization_urls:
- https://dv-ciam.doubleverify.com/realms/pinnacle/protocol/openid-connect/auth
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
- deviceCode
kind: oauth-scopes
layout: scope
method: probed
name: Doubleverify Scopes
name_suffix: OAuth Scopes
note: 'DoubleVerify publishes no scopes reference page — developer.doubleverify.com is behind a login. Every scope below is read verbatim from the `scopes_supported` array of the two discovery documents the provider serves anonymously. Descriptions marked `description_source: inferred` are our reading of the scope NAME and the realm it lives in, not text DoubleVerify published; they are labelled so they are never mistaken for a provider claim. No scope has been invented.'
overview: 'DoubleVerify publishes 21 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the DoubleVerify API on a user''s behalf.


  Tokens are issued from https://dv-ciam.doubleverify.com/realms/pinnacle/protocol/openid-connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: DoubleVerify
provider_slug: doubleverify
schemes:
- flows:
  - authorizationUrl: https://dv-ciam.doubleverify.com/realms/pinnacle/protocol/openid-connect/auth
    flow: authorizationCode
    tokenUrl: https://dv-ciam.doubleverify.com/realms/pinnacle/protocol/openid-connect/token
  - flow: clientCredentials
    tokenUrl: https://dv-ciam.doubleverify.com/realms/pinnacle/protocol/openid-connect/token
  - deviceAuthorizationUrl: https://dv-ciam.doubleverify.com/realms/pinnacle/protocol/openid-connect/auth/device
    flow: deviceCode
  issuer: https://dv-ciam.doubleverify.com/realms/pinnacle
  name: dv-ciam-pinnacle
  type: openIdConnect
scope_count: 21
scope_names:
- openid
- email
- profile
- address
- phone
- offline_access
- roles
- roles-limited
- web-origins
- microprofile-jwt
- acr
- amr
- basic
- service_account
- dv-agent-mcp-aud
- dv-agent-mcp-internal-aud
- dv-apis-aud
- dv-attributes
- ums-aud
- salesforce-id
- impersonation
scopes:
- description: Standard OIDC scope; requests an ID token.
  flows: []
  scope: openid
- description: Standard OIDC scope; releases the email and email_verified claims.
  flows: []
  scope: email
- description: Standard OIDC scope; releases basic profile claims.
  flows: []
  scope: profile
- description: Standard OIDC scope; releases the address claim.
  flows: []
  scope: address
- description: Standard OIDC scope; releases phone_number claims.
  flows: []
  scope: phone
- description: Standard OIDC scope; requests a refresh token for offline use.
  flows: []
  scope: offline_access
- description: Keycloak built-in; adds realm and client role mappings to the token.
  flows: []
  scope: roles
- description: A narrowed variant of the roles mapper.
  flows: []
  scope: roles-limited
- description: Keycloak built-in; adds allowed CORS web origins to the token.
  flows: []
  scope: web-origins
- description: Keycloak built-in; emits MicroProfile JWT claims (upn, groups).
  flows: []
  scope: microprofile-jwt
- description: Keycloak built-in; authentication context class reference.
  flows: []
  scope: acr
- description: Keycloak built-in; authentication methods references.
  flows: []
  scope: amr
- description: Keycloak built-in; core token claims (sub, auth_time).
  flows: []
  scope: basic
- description: Keycloak built-in; marks a client-credentials service-account token.
  flows: []
  scope: service_account
- description: DoubleVerify-specific audience scope for the DV Neura MCP agent surface. Its presence in the Pinnacle realm is the realm-side counterpart of the MCP server at mcp.doubleverify.com.
  flows: []
  scope: dv-agent-mcp-aud
- description: DoubleVerify-specific audience scope for an internal DV Neura MCP surface, distinct from the client-facing one above.
  flows: []
  scope: dv-agent-mcp-internal-aud
- description: DoubleVerify-specific audience scope for DV's API estate.
  flows: []
  scope: dv-apis-aud
- description: DoubleVerify-specific scope releasing DV account/entitlement attributes into the token.
  flows: []
  scope: dv-attributes
- description: DoubleVerify-specific audience scope for a user-management service.
  flows: []
  scope: ums-aud
- description: DoubleVerify-specific scope releasing the linked Salesforce account identifier.
  flows: []
  scope: salesforce-id
- description: Keycloak token-exchange impersonation scope.
  flows: []
  scope: impersonation
slug: doubleverify-scopes
source_filename: doubleverify-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://dv-ciam.doubleverify.com/realms/pinnacle/.well-known/openid-configuration\nalso_source: https://mcp.doubleverify.com/.well-known/oauth-protected-resource/mcp\ndocs: null\nnote: >-\n  DoubleVerify publishes no scopes reference page — developer.doubleverify.com is behind a\n  login. Every scope below is read verbatim from the `scopes_supported` array of the two\n  discovery documents the provider serves anonymously. Descriptions marked\n  `description_source: inferred` are our reading of the scope NAME and the realm it lives\n  in, not text DoubleVerify published; they are labelled so they are never mistaken for a\n  provider claim. No scope has been invented.\n\nschemes:\n- name: dv-ciam-pinnacle\n  type: openIdConnect\n  issuer: https://dv-ciam.doubleverify.com/realms/pinnacle\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://dv-ciam.doubleverify.com/realms/pinnacle/protocol/openid-connect/auth\n \
  \   tokenUrl: https://dv-ciam.doubleverify.com/realms/pinnacle/protocol/openid-connect/token\n  - flow: clientCredentials\n    tokenUrl: https://dv-ciam.doubleverify.com/realms/pinnacle/protocol/openid-connect/token\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://dv-ciam.doubleverify.com/realms/pinnacle/protocol/openid-connect/auth/device\n\nresources:\n- resource: https://mcp.doubleverify.com/mcp\n  scopes_required:\n  - openid\n  - email\n  - profile\n  source: RFC 9728 protected-resource metadata\n\nscopes:\n- scope: openid\n  description: Standard OIDC scope; requests an ID token.\n  description_source: oidc-standard\n  required_by:\n  - https://mcp.doubleverify.com/mcp\n- scope: email\n  description: Standard OIDC scope; releases the email and email_verified claims.\n  description_source: oidc-standard\n  required_by:\n  - https://mcp.doubleverify.com/mcp\n- scope: profile\n  description: Standard OIDC scope; releases basic profile claims.\n  description_source: oidc-standard\n\
  \  required_by:\n  - https://mcp.doubleverify.com/mcp\n- scope: address\n  description: Standard OIDC scope; releases the address claim.\n  description_source: oidc-standard\n- scope: phone\n  description: Standard OIDC scope; releases phone_number claims.\n  description_source: oidc-standard\n- scope: offline_access\n  description: Standard OIDC scope; requests a refresh token for offline use.\n  description_source: oidc-standard\n- scope: roles\n  description: Keycloak built-in; adds realm and client role mappings to the token.\n  description_source: keycloak-builtin\n- scope: roles-limited\n  description: A narrowed variant of the roles mapper.\n  description_source: inferred\n- scope: web-origins\n  description: Keycloak built-in; adds allowed CORS web origins to the token.\n  description_source: keycloak-builtin\n- scope: microprofile-jwt\n  description: Keycloak built-in; emits MicroProfile JWT claims (upn, groups).\n  description_source: keycloak-builtin\n- scope: acr\n  description:\
  \ Keycloak built-in; authentication context class reference.\n  description_source: keycloak-builtin\n- scope: amr\n  description: Keycloak built-in; authentication methods references.\n  description_source: keycloak-builtin\n- scope: basic\n  description: Keycloak built-in; core token claims (sub, auth_time).\n  description_source: keycloak-builtin\n- scope: service_account\n  description: Keycloak built-in; marks a client-credentials service-account token.\n  description_source: keycloak-builtin\n- scope: dv-agent-mcp-aud\n  description: DoubleVerify-specific audience scope for the DV Neura MCP agent surface.\n    Its presence in the Pinnacle realm is the realm-side counterpart of the MCP server at\n    mcp.doubleverify.com.\n  description_source: inferred\n  vendor_specific: true\n- scope: dv-agent-mcp-internal-aud\n  description: DoubleVerify-specific audience scope for an internal DV Neura MCP surface,\n    distinct from the client-facing one above.\n  description_source: inferred\n\
  \  vendor_specific: true\n- scope: dv-apis-aud\n  description: DoubleVerify-specific audience scope for DV's API estate.\n  description_source: inferred\n  vendor_specific: true\n- scope: dv-attributes\n  description: DoubleVerify-specific scope releasing DV account/entitlement attributes\n    into the token.\n  description_source: inferred\n  vendor_specific: true\n- scope: ums-aud\n  description: DoubleVerify-specific audience scope for a user-management service.\n  description_source: inferred\n  vendor_specific: true\n- scope: salesforce-id\n  description: DoubleVerify-specific scope releasing the linked Salesforce account\n    identifier.\n  description_source: inferred\n  vendor_specific: true\n- scope: impersonation\n  description: Keycloak token-exchange impersonation scope.\n  description_source: keycloak-builtin\n\nx-evidence:\n  fetched: '2026-08-13'\n  probes:\n  - url: https://dv-ciam.doubleverify.com/realms/pinnacle/.well-known/openid-configuration\n    http_status: 200\n\
  \  - url: https://mcp.doubleverify.com/.well-known/oauth-protected-resource/mcp\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/doubleverify/refs/heads/main/scopes/doubleverify-scopes.yml
summary_line: 21 scopes · authorizationCode/clientCredentials/deviceCode
tags:
- Ad Verification
- Ad Measurement
- Media Quality
- Brand Suitability
- Viewability
- Attention Measurement
- Invalid Traffic
- Fraud Detection
- Contextual Targeting
- Programmatic Advertising
- Connected TV
- Social Media Measurement
- Commerce Media
- Publisher Analytics
- MRC Accredited
- AdTech
token_urls:
- https://dv-ciam.doubleverify.com/realms/pinnacle/protocol/openid-connect/token
---
