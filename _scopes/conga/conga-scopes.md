---
api_specs:
- filename: conga-administration.json
  format: json
  label: Conga Advantage Platform REST API
  slug: conga-advantage-platform-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conga/refs/heads/main/openapi/conga-administration.json
authorization_urls:
- https://login-rls.congacloud.com/api/v1/auth/connect/authorize
- https://login.conga.com/authorize
description: ''
docs: https://developer.conga.com/platform/reference/authentication
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Conga Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Conga publishes 28 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Conga API on a user''s behalf.


  Tokens are issued from https://login-rls.congacloud.com/api/v1/auth/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Conga
provider_slug: conga
schemes:
- flows:
  - authorizationUrl: https://login-rls.congacloud.com/api/v1/auth/connect/authorize
    flow: authorizationCode
    tokenUrl: https://login-rls.congacloud.com/api/v1/auth/connect/token
  - flow: clientCredentials
    tokenUrl: https://login-rls.congacloud.com/api/v1/auth/connect/token
  grant_types_supported:
  - authorization_code
  - client_credentials
  - refresh_token
  - implicit
  - password
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:openid:params:grant-type:ciba
  - urn:ietf:params:oauth:grant-type:token-exchange
  introspection_endpoint: https://login-rls.congacloud.com/api/v1/auth/connect/introspect
  issuer: https://login-rls.congacloud.com/api/v1/auth
  name: CongaPlatformOAuth
  pkce:
  - S256
  - plain
  regions:
  - issuer: https://login-rls.congacloud.com/api/v1/auth
    region: NA
  - issuer: https://login.congacloud.eu/api/v1/auth
    region: EU
  - issuer: https://login.congacloud.au/api/v1/auth
    region: AU
  revocation_endpoint: https://login-rls.congacloud.com/api/v1/auth/connect/revocation
  source: https://login-rls.congacloud.com/api/v1/auth/.well-known/openid-configuration
- flows:
  - authorizationUrl: https://login.conga.com/authorize
    flow: authorizationCode
    tokenUrl: https://login.conga.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://login.conga.com/oauth/token
  issuer: https://login.conga.com/
  name: DeveloperPortalOIDC
  note: Auth0 tenant behind the developer portal login, not the platform API.
  source: https://login.conga.com/.well-known/openid-configuration
scope_count: 28
scope_names:
- api.cart
- api.catalog
- api.quote
- api.order
- api.document-management
- api.user-management
- api.metadata
- api.data
- api.localization
- api.revenue-admin
- api.custom-api
- api.email
- doc-gen.composer
- sign
- sign.provisioning
- Auth.Api.Read
- IngressIbis
- EUF-Reference-App
- CCI-Prod-RLS-PREVIEW
- https://rls-preview.congacloud.au/mcp
- openid
- profile
- email
- address
- phone
- external_claims
- force_login
- offline_access
scopes:
- description: CPQ cart operations - configuration, pricing and cart actions.
  flows: []
  scope: api.cart
- description: Product catalog - products, categories, price lists, product groups.
  flows: []
  scope: api.catalog
- description: Quote/proposal objects.
  flows: []
  scope: api.quote
- description: Order objects.
  flows: []
  scope: api.order
- description: Document storage, retrieval and metadata.
  flows: []
  scope: api.document-management
- description: Users, user groups, roles, permission groups and organization info.
  flows: []
  scope: api.user-management
- description: Platform metadata / schema definitions.
  flows: []
  scope: api.metadata
- description: Generic platform data access over business objects.
  flows: []
  scope: api.data
- description: Localization - languages, translations, locale settings.
  flows: []
  scope: api.localization
- description: Revenue administration - the largest service in the catalogue (583 operations).
  flows: []
  scope: api.revenue-admin
- description: Customer-authored extensibility endpoints.
  flows: []
  scope: api.custom-api
- description: Platform email service.
  flows: []
  scope: api.email
- description: Conga Composer document generation.
  flows: []
  scope: doc-gen.composer
- description: Conga Sign e-signature.
  flows: []
  scope: sign
- description: Conga Sign account/tenant provisioning.
  flows: []
  scope: sign.provisioning
- description: Read access to the authorization service's own API.
  flows: []
  scope: Auth.Api.Read
- description: Ingress service (document ingestion pipeline).
  flows: []
  scope: IngressIbis
- description: Reference-application client registration; not a general API scope.
  flows: []
  scope: EUF-Reference-App
- description: Preview environment client registration; not a general API scope.
  flows: []
  scope: CCI-Prod-RLS-PREVIEW
- description: RFC 8707 resource indicator for Conga's MCP server. Present only in the AU discovery document; this string is how the otherwise-undocumented MCP surface was found. See mcp/conga-mcp.yml.
  flows: []
  scope: https://rls-preview.congacloud.au/mcp
- description: OpenID Connect authentication; issue an ID token.
  flows: []
  scope: openid
- description: Access to the user's default profile claims.
  flows: []
  scope: profile
- description: Access to the user's email and email_verified claims.
  flows: []
  scope: email
- description: Access to the user's address claim.
  flows: []
  scope: address
- description: Access to the user's phone_number claims.
  flows: []
  scope: phone
- description: Claims federated from an external identity provider.
  flows: []
  scope: external_claims
- description: Force re-authentication rather than reusing an existing session.
  flows: []
  scope: force_login
- description: Issue a refresh token for long-lived access.
  flows: []
  scope: offline_access
slug: conga-scopes
source_filename: conga-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://login-rls.congacloud.com/api/v1/auth/.well-known/openid-configuration\ndocs: https://developer.conga.com/platform/reference/authentication\nnotes: >-\n  Conga's developer documentation does not publish a scopes or permissions\n  reference page - it describes the client_credentials flow and says access is\n  governed by the Integration User's platform permissions. The platform's own\n  OAuth authorization servers, however, advertise a full scope set in their OIDC\n  discovery documents, and those scopes map cleanly onto the services in\n  openapi/. The api.* scopes below are Conga's own published strings, read\n  verbatim from the discovery documents of all three production regions. They\n  are undocumented in prose, so the service mapping in `covers:` is our\n  derivation from the matching OpenAPI document, marked as such.\nschemes:\n- name: CongaPlatformOAuth\n  source: https://login-rls.congacloud.com/api/v1/auth/.well-known/openid-configuration\n\
  \  issuer: https://login-rls.congacloud.com/api/v1/auth\n  regions:\n  - region: NA\n    issuer: https://login-rls.congacloud.com/api/v1/auth\n  - region: EU\n    issuer: https://login.congacloud.eu/api/v1/auth\n  - region: AU\n    issuer: https://login.congacloud.au/api/v1/auth\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login-rls.congacloud.com/api/v1/auth/connect/authorize\n    tokenUrl: https://login-rls.congacloud.com/api/v1/auth/connect/token\n  - flow: clientCredentials\n    tokenUrl: https://login-rls.congacloud.com/api/v1/auth/connect/token\n  grant_types_supported: [authorization_code, client_credentials, refresh_token, implicit,\n    password, 'urn:ietf:params:oauth:grant-type:device_code', 'urn:openid:params:grant-type:ciba',\n    'urn:ietf:params:oauth:grant-type:token-exchange']\n  pkce: [S256, plain]\n  introspection_endpoint: https://login-rls.congacloud.com/api/v1/auth/connect/introspect\n  revocation_endpoint: https://login-rls.congacloud.com/api/v1/auth/connect/revocation\n\
  - name: DeveloperPortalOIDC\n  source: https://login.conga.com/.well-known/openid-configuration\n  issuer: https://login.conga.com/\n  note: Auth0 tenant behind the developer portal login, not the platform API.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.conga.com/authorize\n    tokenUrl: https://login.conga.com/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://login.conga.com/oauth/token\nscopes:\n- scope: api.cart\n  kind: api\n  description: CPQ cart operations - configuration, pricing and cart actions.\n  covers: openapi/conga-cart-v1.json\n  covers_method: derived\n- scope: api.catalog\n  kind: api\n  description: Product catalog - products, categories, price lists, product groups.\n  covers: openapi/conga-catalog.json\n  covers_method: derived\n- scope: api.quote\n  kind: api\n  description: Quote/proposal objects.\n  covers: openapi/conga-quote.json\n  covers_method: derived\n- scope: api.order\n  kind: api\n  description: Order objects.\n\
  \  covers: openapi/conga-order.json\n  covers_method: derived\n- scope: api.document-management\n  kind: api\n  description: Document storage, retrieval and metadata.\n  covers: openapi/conga-document-management.json\n  covers_method: derived\n- scope: api.user-management\n  kind: api\n  description: Users, user groups, roles, permission groups and organization info.\n  covers: openapi/conga-user-management.json\n  covers_method: derived\n- scope: api.metadata\n  kind: api\n  description: Platform metadata / schema definitions.\n  covers: openapi/conga-schema-manager.json\n  covers_method: derived\n- scope: api.data\n  kind: api\n  description: Generic platform data access over business objects.\n  covers: openapi/conga-data.json\n  covers_method: derived\n- scope: api.localization\n  kind: api\n  description: Localization - languages, translations, locale settings.\n  covers: openapi/conga-localization.json\n  covers_method: derived\n- scope: api.revenue-admin\n  kind: api\n  description:\
  \ Revenue administration - the largest service in the catalogue (583 operations).\n  covers: openapi/conga-administration.json\n  covers_method: derived\n- scope: api.custom-api\n  kind: api\n  description: Customer-authored extensibility endpoints.\n  covers: openapi/conga-extensibility.json\n  covers_method: derived\n- scope: api.email\n  kind: api\n  description: Platform email service.\n  covers: openapi/conga-email.json\n  covers_method: derived\n- scope: doc-gen.composer\n  kind: api\n  description: Conga Composer document generation.\n  covers: null\n  covers_method: derived\n- scope: sign\n  kind: api\n  description: Conga Sign e-signature.\n  covers: openapi/conga-conga-sign.json\n  covers_method: derived\n- scope: sign.provisioning\n  kind: api\n  description: Conga Sign account/tenant provisioning.\n  covers: null\n  covers_method: derived\n- scope: Auth.Api.Read\n  kind: api\n  description: Read access to the authorization service's own API.\n  covers: null\n  covers_method:\
  \ derived\n- scope: IngressIbis\n  kind: api\n  description: Ingress service (document ingestion pipeline).\n  covers: openapi/conga-ingress.json\n  covers_method: derived\n- scope: EUF-Reference-App\n  kind: application\n  description: Reference-application client registration; not a general API scope.\n- scope: CCI-Prod-RLS-PREVIEW\n  kind: application\n  region: NA only\n  description: Preview environment client registration; not a general API scope.\n- scope: https://rls-preview.congacloud.au/mcp\n  kind: resource\n  region: AU only\n  description: >-\n    RFC 8707 resource indicator for Conga's MCP server. Present only in the AU\n    discovery document; this string is how the otherwise-undocumented MCP surface\n    was found. See mcp/conga-mcp.yml.\n- scope: openid\n  kind: oidc\n  description: OpenID Connect authentication; issue an ID token.\n- scope: profile\n  kind: oidc\n  description: Access to the user's default profile claims.\n- scope: email\n  kind: oidc\n  description:\
  \ Access to the user's email and email_verified claims.\n- scope: address\n  kind: oidc\n  description: Access to the user's address claim.\n- scope: phone\n  kind: oidc\n  description: Access to the user's phone_number claims.\n- scope: external_claims\n  kind: oidc\n  description: Claims federated from an external identity provider.\n- scope: force_login\n  kind: oidc\n  description: Force re-authentication rather than reusing an existing session.\n- scope: offline_access\n  kind: oidc\n  description: Issue a refresh token for long-lived access.\nregional_differences:\n  note: >-\n    The three production regions publish nearly identical scope sets. NA\n    additionally advertises CCI-Prod-RLS-PREVIEW; AU additionally advertises the\n    MCP resource indicator. EU advertises neither.\nspec_declared_scopes:\n  count: 0\n  note: >-\n    None of the 31 OpenAPI documents declare an oauth2 securityScheme - every one\n    declares a single apiKey scheme named \"Bearer\" in the Authorization\
  \ header\n    (\"Please insert JWT with Bearer into field\"). The specs therefore carry no\n    per-operation scope requirements, and the authorization surface is only\n    visible from the OIDC discovery documents above. That mismatch is recorded in\n    conformance/conga-conformance.yml.\nchecked: '2026-08-13'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conga/refs/heads/main/scopes/conga-scopes.yml
summary_line: 28 scopes · authorizationCode/clientCredentials
tags:
- Company
- Enterprise Software
- Contract Lifecycle Management
- CPQ
- Revenue Lifecycle Management
- Document Automation
- E-Signature
- Contract Intelligence
- CRM
- OpenAPI
- MCP
- GraphQL
- Billing
- Approvals
token_urls:
- https://login-rls.congacloud.com/api/v1/auth/connect/token
- https://login.conga.com/oauth/token
---
