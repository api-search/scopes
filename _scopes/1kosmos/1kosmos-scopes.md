---
api_specs:
- filename: 1kosmos-access-code-api-openapi.yml
  format: yaml
  label: 1Kosmos Access Code API
  slug: 1kosmos-access-code-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1kosmos/refs/heads/main/openapi/1kosmos-access-code-api-openapi.yml
- filename: 1kosmos-ial-api-openapi.yml
  format: yaml
  label: 1Kosmos IAL API
  slug: 1kosmos-ial-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1kosmos/refs/heads/main/openapi/1kosmos-ial-api-openapi.yml
- filename: 1kosmos-ial2-api-openapi.yml
  format: yaml
  label: 1Kosmos IAL2 API
  slug: 1kosmos-ial2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1kosmos/refs/heads/main/openapi/1kosmos-ial2-api-openapi.yml
- filename: 1kosmos-id-verification-api-openapi.yml
  format: yaml
  label: 1Kosmos ID Verification API
  slug: 1kosmos-id-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1kosmos/refs/heads/main/openapi/1kosmos-id-verification-api-openapi.yml
- filename: 1kosmos-otp-api-openapi.yml
  format: yaml
  label: 1Kosmos OTP API
  slug: 1kosmos-otp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1kosmos/refs/heads/main/openapi/1kosmos-otp-api-openapi.yml
- filename: 1kosmos-reports-api-openapi.yml
  format: yaml
  label: 1Kosmos Reports API
  slug: 1kosmos-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1kosmos/refs/heads/main/openapi/1kosmos-reports-api-openapi.yml
- filename: 1kosmos-set-up-api-openapi.yml
  format: yaml
  label: 1Kosmos Set up API
  slug: 1kosmos-set-up-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1kosmos/refs/heads/main/openapi/1kosmos-set-up-api-openapi.yml
- filename: 1kosmos-user-management-api-openapi.yml
  format: yaml
  label: 1Kosmos User Management API
  slug: 1kosmos-user-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1kosmos/refs/heads/main/openapi/1kosmos-user-management-api-openapi.yml
- filename: 1kosmos-verifiable-credentials-api-openapi.yml
  format: yaml
  label: 1Kosmos Verifiable Credentials API
  slug: 1kosmos-verifiable-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1kosmos/refs/heads/main/openapi/1kosmos-verifiable-credentials-api-openapi.yml
- filename: 1kosmos-workflow-api-api-openapi.yml
  format: yaml
  label: 1Kosmos Workflow API API
  slug: 1kosmos-workflow-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1kosmos/refs/heads/main/openapi/1kosmos-workflow-api-api-openapi.yml
authorization_urls: []
description: ''
docs: https://developer.1kosmos.com/devportal/docs/oauth2-oidc/
flows:
- authorizationCode
- refreshToken
kind: oauth-scopes
layout: scope
method: searched
name: 1Kosmos Scopes
name_suffix: OAuth Scopes
note: The licensekey-authenticated BlockID platform API declares no OAuth2 security scheme — see authentication/1kosmos-authentication.yml. This file covers the SEPARATE surface on which BlockID acts as an OAuth 2.0 / OpenID Connect authorization server for relying applications. The scope set below is exactly what the developer portal documents; 1Kosmos publishes no scopes reference page, no /.well-known/openid-configuration (404 on every host probed) and no scopes_supported list, so the real scope catalog of a live tenant cannot be enumerated anonymously.
overview: '1Kosmos publishes 3 OAuth 2.0 scopes via the authorizationCode and refreshToken flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the 1Kosmos API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: 1Kosmos
provider_slug: 1kosmos
schemes:
- flows:
  - authorizationUrl: null
    flow: authorizationCode
    note: Endpoints are tenant-scoped and obtained from the tenant's oauth2 service base URL in the /caas/sd service-discovery document; no absolute URLs are published in the docs. The helper SDKs expose BIDOauth2.requestAuthorizationCode() and BIDOauth2.requestToken().
    tokenUrl: null
  - flow: refreshToken
    tokenUrl: null
  grant_types:
  - authorization_code
  - refresh_token
  name: BlockID OAuth 2.0 / OIDC authorization server
  service_discovery_key: oauth2
  source: https://developer.1kosmos.com/devportal/docs/oauth2-oidc/
scope_count: 3
scope_names:
- openid
- email
- profile
scopes:
- description: Required for the OpenID Connect flow; requests an ID token.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the authenticated user's email address.
  flows:
  - authorizationCode
  scope: email
- description: Access to the authenticated user's profile attributes.
  flows:
  - authorizationCode
  scope: profile
slug: 1kosmos-scopes
source_filename: 1kosmos-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: https://developer.1kosmos.com/devportal/docs/oauth2-oidc/\ndocs: https://developer.1kosmos.com/devportal/docs/oauth2-oidc/\nnote: >-\n  The licensekey-authenticated BlockID platform API declares no OAuth2 security scheme — see\n  authentication/1kosmos-authentication.yml. This file covers the SEPARATE surface on which BlockID\n  acts as an OAuth 2.0 / OpenID Connect authorization server for relying applications. The scope set\n  below is exactly what the developer portal documents; 1Kosmos publishes no scopes reference page,\n  no /.well-known/openid-configuration (404 on every host probed) and no scopes_supported list, so\n  the real scope catalog of a live tenant cannot be enumerated anonymously.\nschemes:\n- name: BlockID OAuth 2.0 / OIDC authorization server\n  source: https://developer.1kosmos.com/devportal/docs/oauth2-oidc/\n  service_discovery_key: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl:\
  \ null\n    tokenUrl: null\n    note: >-\n      Endpoints are tenant-scoped and obtained from the tenant's oauth2 service base URL in the\n      /caas/sd service-discovery document; no absolute URLs are published in the docs. The helper\n      SDKs expose BIDOauth2.requestAuthorizationCode() and BIDOauth2.requestToken().\n  - flow: refreshToken\n    tokenUrl: null\n  grant_types: [authorization_code, refresh_token]\nscopes:\n- scope: openid\n  description: Required for the OpenID Connect flow; requests an ID token.\n  flows: [authorizationCode]\n  sources: [https://developer.1kosmos.com/devportal/docs/oauth2-oidc/]\n- scope: email\n  description: Access to the authenticated user's email address.\n  flows: [authorizationCode]\n  sources: [https://developer.1kosmos.com/devportal/docs/oauth2-oidc/]\n- scope: profile\n  description: Access to the authenticated user's profile attributes.\n  flows: [authorizationCode]\n  sources: [https://developer.1kosmos.com/devportal/docs/oauth2-oidc/]\n\
  documented_scope_strings:\n- {value: openid email profile, used_for: OIDC flow}\n- {value: email profile, used_for: OAuth2 authorization-code flow without OIDC}\nsession_scopes:\n  note: >-\n    Distinct from OAuth scopes — the UWL 2.0 session API takes a `scopes` parameter that selects\n    what the authenticator returns in the session payload.\n  documented_values: [device_info]\n  source: https://developer.1kosmos.com/devportal/docs/uwl/creates_session/\nclient_registration:\n  self_service: false\n  note: clientId, clientSecret and redirectUri are issued through the BlockID developer dashboard.\ngaps:\n- No published scopes/permissions reference page.\n- No OIDC discovery document, so scopes_supported cannot be read.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1kosmos/refs/heads/main/scopes/1kosmos-scopes.yml
summary_line: 3 scopes · authorizationCode/refreshToken
tags:
- Identity
- Authentication
- Identity Verification
- Passwordless
- Biometrics
- Verifiable Credentials
- FIDO2
- Security
- Company
token_urls: []
---
