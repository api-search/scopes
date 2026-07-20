---
api_specs:
- filename: avalara-avatax-rest-openapi.yml
  format: yaml
  label: AvaTax APIs
  slug: avatax-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-avatax-rest-openapi.yml
- filename: avalara-communications-openapi.yml
  format: yaml
  label: Communications Tax API
  slug: communications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-communications-openapi.yml
- filename: avalara-excise-openapi.yml
  format: yaml
  label: Excise Platform API
  slug: excise-tax-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-excise-openapi.yml
- filename: avalara-item-classification-openapi.yml
  format: yaml
  label: Item Classification API
  slug: item-classification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-item-classification-openapi.yml
- filename: avalara-avatax-brazil-openapi.yml
  format: yaml
  label: AvaTax Brazil API
  slug: avatax-brazil-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-avatax-brazil-openapi.yml
- filename: avalara-vat-reporting-openapi.yml
  format: yaml
  label: VAT Reporting API
  slug: vat-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-vat-reporting-openapi.yml
- filename: avalara-mylodgetax-openapi.yml
  format: yaml
  label: MyLodgeTax API
  slug: mylodgetax-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-mylodgetax-openapi.yml
- filename: avalara-certcapture-openapi.yml
  format: yaml
  label: CertCapture API
  slug: certcapture-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-certcapture-openapi.yml
- filename: avalara-e-invoicing-openapi.yml
  format: yaml
  label: E-Invoicing REST API
  slug: e-invoicing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-e-invoicing-openapi.yml
- filename: avalara-activation-service-openapi.yml
  format: yaml
  label: Activation Service API
  slug: activation-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-activation-service-openapi.yml
- filename: avalara-business-openapi.yml
  format: yaml
  label: Avalara Business API
  slug: business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-business-openapi.yml
- filename: avalara-portal-oauth-openapi.yml
  format: yaml
  label: Portal OAuth API
  slug: portal-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-portal-oauth-openapi.yml
- filename: avalara-shared-company-service-openapi.yml
  format: yaml
  label: Shared Company Service API
  slug: shared-company-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-shared-company-service-openapi.yml
- filename: avalara-hs-code-classification-openapi.yml
  format: yaml
  label: Automated Tariff Code Classification API
  slug: hs-code-classification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-hs-code-classification-openapi.yml
- filename: avalara-1099-w9-openapi.yml
  format: yaml
  label: 1099 & W-9 API
  slug: 1099-w9-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-1099-w9-openapi.yml
authorization_urls: []
description: ''
docs: https://developer.avalara.com/api-reference/oauth/oauth/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Avalara Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Avalara publishes 24 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Avalara API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Avalara
provider_slug: avalara
schemes: []
scope_count: 24
scope_names:
- openid
- profile
- email
- phone
- address
- offline_access
- avatax
- avatax_account_override
- excise
- ecm
- saas_vat_reporting
- orl
- svr
- crr_api
- cross-border-quoting
- provisioning_agent
- elr.audit.publish
- content-studio-sourcing:read
- content-studio-sourcing:write
- content-studio-compliance:read
- content-studio-compliance:write
- studio.connector
- studio.connector.adapter
- studio.extractor.adapter
scopes:
- description: OpenID Connect authentication (subject identity).
  flows: []
  scope: openid
- description: Standard OIDC profile claims.
  flows: []
  scope: profile
- description: Email address claim.
  flows: []
  scope: email
- description: Phone number claim.
  flows: []
  scope: phone
- description: Address claim.
  flows: []
  scope: address
- description: Issue a refresh token for long-lived access.
  flows: []
  scope: offline_access
- description: Access to AvaTax sales/use tax calculation and transaction APIs.
  flows: []
  scope: avatax
- description: Act against a specified AvaTax account (account override).
  flows: []
  scope: avatax_account_override
- description: Access to Avalara Excise tax APIs.
  flows: []
  scope: excise
- description: Access to Exemption Certificate Management (CertCapture/ECM).
  flows: []
  scope: ecm
- description: Access to the SaaS VAT Reporting APIs.
  flows: []
  scope: saas_vat_reporting
- description: Avalara ORL (returns/reporting) service scope.
  flows: []
  scope: orl
- description: Avalara SVR service scope.
  flows: []
  scope: svr
- description: CRR API scope.
  flows: []
  scope: crr_api
- description: Cross-border duty/tax quoting (landed cost).
  flows: []
  scope: cross-border-quoting
- description: Account/service provisioning agent scope.
  flows: []
  scope: provisioning_agent
- description: E-Invoicing and Live Reporting (ELR) audit publish scope.
  flows: []
  scope: elr.audit.publish
- description: Read access to Content Studio sourcing content.
  flows: []
  scope: content-studio-sourcing:read
- description: Write access to Content Studio sourcing content.
  flows: []
  scope: content-studio-sourcing:write
- description: Read access to Content Studio compliance content.
  flows: []
  scope: content-studio-compliance:read
- description: Write access to Content Studio compliance content.
  flows: []
  scope: content-studio-compliance:write
- description: Studio connector service scope.
  flows: []
  scope: studio.connector
- description: Studio connector adapter scope.
  flows: []
  scope: studio.connector.adapter
- description: Studio extractor adapter scope.
  flows: []
  scope: studio.extractor.adapter
slug: avalara-scopes
source_filename: avalara-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: https://identity.avalara.com/.well-known/openid-configuration\ndocs: https://developer.avalara.com/api-reference/oauth/oauth/\nnotes: >-\n  Avalara authenticates via IdentityServer at identity.avalara.com. The OpenID\n  Connect discovery document publishes the full OAuth 2.0 surface: authorization,\n  token, introspection, revocation, device-authorization and userinfo endpoints,\n  the supported grant types, and the scopes_supported list captured below. The\n  per-API OpenAPI specs model calls with HTTP basic/bearer (see authentication/),\n  but the platform-level authorization is OAuth 2.0 / OIDC against this issuer.\nissuer: https://identity.avalara.com\nendpoints:\n  authorization: https://identity.avalara.com/connect/authorize\n  token: https://identity.avalara.com/connect/token\n  userinfo: https://identity.avalara.com/connect/userinfo\n  introspection: https://identity.avalara.com/connect/introspect\n  revocation: https://identity.avalara.com/connect/revocation\n\
  \  device_authorization: https://identity.avalara.com/connect/deviceauthorization\n  end_session: https://identity.avalara.com/connect/endsession\n  jwks: https://identity.avalara.com/.well-known/openid-configuration/jwks\n  registration: https://identity.avalara.com/register/public\ngrant_types_supported:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - implicit\n  - password\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\ncode_challenge_methods_supported: [plain, S256]\ntoken_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  - private_key_jwt\nscopes:\n  - scope: openid\n    description: OpenID Connect authentication (subject identity).\n  - scope: profile\n    description: Standard OIDC profile claims.\n  - scope: email\n    description: Email address claim.\n  - scope: phone\n    description: Phone number claim.\n  - scope: address\n    description: Address claim.\n  -\
  \ scope: offline_access\n    description: Issue a refresh token for long-lived access.\n  - scope: avatax\n    description: Access to AvaTax sales/use tax calculation and transaction APIs.\n  - scope: avatax_account_override\n    description: Act against a specified AvaTax account (account override).\n  - scope: excise\n    description: Access to Avalara Excise tax APIs.\n  - scope: ecm\n    description: Access to Exemption Certificate Management (CertCapture/ECM).\n  - scope: saas_vat_reporting\n    description: Access to the SaaS VAT Reporting APIs.\n  - scope: orl\n    description: Avalara ORL (returns/reporting) service scope.\n  - scope: svr\n    description: Avalara SVR service scope.\n  - scope: crr_api\n    description: CRR API scope.\n  - scope: cross-border-quoting\n    description: Cross-border duty/tax quoting (landed cost).\n  - scope: provisioning_agent\n    description: Account/service provisioning agent scope.\n  - scope: elr.audit.publish\n    description: E-Invoicing\
  \ and Live Reporting (ELR) audit publish scope.\n  - scope: content-studio-sourcing:read\n    description: Read access to Content Studio sourcing content.\n  - scope: content-studio-sourcing:write\n    description: Write access to Content Studio sourcing content.\n  - scope: content-studio-compliance:read\n    description: Read access to Content Studio compliance content.\n  - scope: content-studio-compliance:write\n    description: Write access to Content Studio compliance content.\n  - scope: studio.connector\n    description: Studio connector service scope.\n  - scope: studio.connector.adapter\n    description: Studio connector adapter scope.\n  - scope: studio.extractor.adapter\n    description: Studio extractor adapter scope.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/scopes/avalara-scopes.yml
summary_line: 24 scopes
tags:
- Taxes
token_urls: []
---
