---
api_specs:
- filename: triodos-bank-uk-xs2a-openapi.json
  format: json
  label: Triodos Account Information Service (AIS) API
  slug: triodos-account-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triodos-bank-uk/refs/heads/main/openapi/triodos-bank-uk-xs2a-openapi.json
- filename: triodos-bank-uk-xs2a-openapi.json
  format: json
  label: Triodos Payment Initiation Service (PIS) API
  slug: triodos-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triodos-bank-uk/refs/heads/main/openapi/triodos-bank-uk-xs2a-openapi.json
- filename: triodos-bank-uk-xs2a-openapi.json
  format: json
  label: Triodos Confirmation of Funds Service (CoF) API
  slug: triodos-confirmation-of-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triodos-bank-uk/refs/heads/main/openapi/triodos-bank-uk-xs2a-openapi.json
- filename: triodos-bank-uk-auth-openapi.json
  format: json
  label: Triodos XS2A Authorization (OAuth2/OIDC) API
  slug: triodos-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triodos-bank-uk/refs/heads/main/openapi/triodos-bank-uk-auth-openapi.json
authorization_urls: []
description: ''
docs: https://developer.triodos.com/docs/authorisation
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Triodos Bank Uk Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Triodos Bank UK publishes 5 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Triodos Bank UK API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Triodos Bank UK
provider_slug: triodos-bank-uk
schemes:
- authorizationUrl: https://api.triodos.com/auth/{tenant}/v1/auth
  flow: authorizationCode
  name: openid-connect
  tokenUrl: https://api.triodos.com/auth/{tenant}/v1/token
scope_count: 5
scope_names:
- openid
- offline_access
- AIS:{consent-id}
- PIS:{payment-id}
- PIIS:{consent-id}
scopes:
- description: Standard OpenID Connect scope; always requested to start the SCA flow.
  flows:
  - authorizationCode
  scope: openid
- description: Requests a refresh token for long-lived (recurring) account access. Added automatically to the scaRedirect link when recurring account access is requested.
  flows:
  - authorizationCode
  scope: offline_access
- description: Account Information Service access bound to a specific registered consent resource id (e.g. AIS:5e70106a-...). Grants read access to the accounts, balances, and transactions covered by that consent.
  flows:
  - authorizationCode
  scope: AIS:{consent-id}
- description: Payment Initiation Service authorisation bound to a specific payment resource id (e.g. PIS:5e70106a-...). Authorises execution of that single payment.
  flows:
  - authorizationCode
  scope: PIS:{payment-id}
- description: Confirmation of Funds (CBPII/PIIS) access bound to a specific funds- confirmation consent resource id. Grants the right to query availability of funds on the covered account.
  flows:
  - authorizationCode
  scope: PIIS:{consent-id}
slug: triodos-bank-uk-scopes
source_filename: triodos-bank-uk-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: https://developer.triodos.com/docs/authorisation\ndocs: https://developer.triodos.com/docs/authorisation\nnotes: >-\n  Scopes are documented in the Triodos authorisation guide, not in the OpenAPI\n  securitySchemes (which the Berlin Group template leaves empty). Following\n  NextGenPSD2, the resource scope is dynamic and bound to a specific consent or\n  payment resource id, so access is scoped per-resource rather than per-tenant.\nschemes:\n- name: openid-connect\n  flow: authorizationCode\n  authorizationUrl: https://api.triodos.com/auth/{tenant}/v1/auth\n  tokenUrl: https://api.triodos.com/auth/{tenant}/v1/token\nscopes:\n- scope: openid\n  description: Standard OpenID Connect scope; always requested to start the SCA flow.\n  flows: [authorizationCode]\n- scope: offline_access\n  description: >-\n    Requests a refresh token for long-lived (recurring) account access. Added\n    automatically to the scaRedirect link when\
  \ recurring account access is\n    requested.\n  flows: [authorizationCode]\n- scope: 'AIS:{consent-id}'\n  description: >-\n    Account Information Service access bound to a specific registered consent\n    resource id (e.g. AIS:5e70106a-...). Grants read access to the accounts,\n    balances, and transactions covered by that consent.\n  flows: [authorizationCode]\n- scope: 'PIS:{payment-id}'\n  description: >-\n    Payment Initiation Service authorisation bound to a specific payment resource\n    id (e.g. PIS:5e70106a-...). Authorises execution of that single payment.\n  flows: [authorizationCode]\n- scope: 'PIIS:{consent-id}'\n  description: >-\n    Confirmation of Funds (CBPII/PIIS) access bound to a specific funds-\n    confirmation consent resource id. Grants the right to query availability of\n    funds on the covered account.\n  flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/triodos-bank-uk/refs/heads/main/scopes/triodos-bank-uk-scopes.yml
summary_line: 5 scopes
tags:
- Financial Services
- Banking
- Open Banking
- PSD2
- XS2A
- Berlin Group
- United Kingdom
- Payments
- Account Information
- Confirmation of Funds
- Ethical Banking
- Sustainable Finance
- Specialist Lender
token_urls: []
---
