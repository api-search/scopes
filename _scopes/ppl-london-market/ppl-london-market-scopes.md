---
api_specs:
- filename: ppl-london-market-contract-api-openapi.yml
  format: yaml
  label: PPL Contract API
  slug: ppl-london-market-contract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppl-london-market/refs/heads/main/openapi/ppl-london-market-contract-api-openapi.yml
- filename: ppl-london-market-document-api-openapi.yml
  format: yaml
  label: PPL Document API
  slug: ppl-london-market-document-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppl-london-market/refs/heads/main/openapi/ppl-london-market-document-api-openapi.yml
- filename: ppl-london-market-health-api-openapi.yml
  format: yaml
  label: PPL Health API
  slug: ppl-london-market-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppl-london-market/refs/heads/main/openapi/ppl-london-market-health-api-openapi.yml
- filename: ppl-london-market-negotiation-api-openapi.yml
  format: yaml
  label: PPL Negotiation API
  slug: ppl-london-market-negotiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppl-london-market/refs/heads/main/openapi/ppl-london-market-negotiation-api-openapi.yml
- filename: ppl-london-market-notification-api-openapi.yml
  format: yaml
  label: PPL Notification API
  slug: ppl-london-market-notification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppl-london-market/refs/heads/main/openapi/ppl-london-market-notification-api-openapi.yml
- filename: ppl-london-market-organisation-api-openapi.yml
  format: yaml
  label: PPL Organisation API
  slug: ppl-london-market-organisation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppl-london-market/refs/heads/main/openapi/ppl-london-market-organisation-api-openapi.yml
- filename: ppl-london-market-participation-api-openapi.yml
  format: yaml
  label: PPL Participation API
  slug: ppl-london-market-participation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppl-london-market/refs/heads/main/openapi/ppl-london-market-participation-api-openapi.yml
- filename: ppl-london-market-placement-api-openapi.yml
  format: yaml
  label: PPL Placement API
  slug: ppl-london-market-placement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppl-london-market/refs/heads/main/openapi/ppl-london-market-placement-api-openapi.yml
- filename: ppl-london-market-programme-api-openapi.yml
  format: yaml
  label: PPL Programme API
  slug: ppl-london-market-programme-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppl-london-market/refs/heads/main/openapi/ppl-london-market-programme-api-openapi.yml
- filename: ppl-london-market-section-api-openapi.yml
  format: yaml
  label: PPL Section API
  slug: ppl-london-market-section-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppl-london-market/refs/heads/main/openapi/ppl-london-market-section-api-openapi.yml
- filename: ppl-london-market-submission-api-openapi.yml
  format: yaml
  label: PPL Submission API
  slug: ppl-london-market-submission-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppl-london-market/refs/heads/main/openapi/ppl-london-market-submission-api-openapi.yml
- filename: ppl-london-market-transaction-api-openapi.yml
  format: yaml
  label: PPL Transaction API
  slug: ppl-london-market-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppl-london-market/refs/heads/main/openapi/ppl-london-market-transaction-api-openapi.yml
- filename: ppl-london-market-version-api-openapi.yml
  format: yaml
  label: PPL Version API
  slug: ppl-london-market-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppl-london-market/refs/heads/main/openapi/ppl-london-market-version-api-openapi.yml
authorization_urls:
- https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/authorize
description: ''
docs: https://developer.pplnextgen.com/Get-Started/Authentication-Information
flows:
- authorizationCode
- onBehalfOf
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Ppl London Market Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'PPL publishes 1 OAuth 2.0 scope via the authorizationCode, onBehalfOf, and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the PPL API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: PPL
provider_slug: ppl-london-market
schemes:
- flows:
  - authorizationUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  - flow: onBehalfOf
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  name: entraIdBearer
  provider: Microsoft Entra ID (Azure AD)
  source: https://developer.pplnextgen.com/Get-Started/Authentication-Information
  type: oauth2
scope_count: 1
scope_names:
- user_impersonation
scopes:
- description: 'The single delegated permission the LIMOSS API Gateway checks. The Base API Standard states the JWT must carry the claim "scp": "user_impersonation"; the Authentication page states that "if there is a scope claim which includes ''user_impersonation'', then it may be passed directly to the API Gateway", and that otherwise the caller must acquire an on-behalf-of token that has it.'
  flows:
  - authorizationCode
  - onBehalfOf
  - clientCredentials
  scope: user_impersonation
slug: ppl-london-market-scopes
source_filename: ppl-london-market-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: >-\n  Docs only. python3 0-working/derive-oauth-scopes.py returned nothing for this provider because\n  none of the five PPL OpenAPI documents declares an oauth2 securityScheme — the OAuth contract is\n  published only in developer-portal prose.\ndocs: https://developer.pplnextgen.com/Get-Started/Authentication-Information\nalso_documented_at: https://developer.pplnextgen.com/Get-Started/Base-API-Standard\nmodel: >-\n  PPL does not operate its own authorization server and does not publish a per-resource scope\n  catalogue. Authorization is delegated wholesale to Microsoft Entra ID (Azure AD) in the LIMOSS\n  API Common Services tenant, and the LIMOSS API Gateway gates on a single delegated-permission\n  scope. Resource-level authorization is then enforced by team/user context carried in the\n  X-Auth-Team and X-Auth-Impersonated-User headers, and by the market roles held by that user —\n  not by OAuth scopes.\nschemes:\n- name:\
  \ entraIdBearer\n  type: oauth2\n  provider: Microsoft Entra ID (Azure AD)\n  source: https://developer.pplnextgen.com/Get-Started/Authentication-Information\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n  - flow: onBehalfOf\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\nscopes:\n- scope: user_impersonation\n  description: >-\n    The single delegated permission the LIMOSS API Gateway checks. The Base API Standard states the\n    JWT must carry the claim \"scp\": \"user_impersonation\"; the Authentication page states that \"if\n    there is a scope claim which includes 'user_impersonation', then it may be passed directly to\n    the API Gateway\", and that otherwise the caller must acquire\
  \ an on-behalf-of token that has it.\n  flows: [authorizationCode, onBehalfOf, clientCredentials]\n  sources: [https://developer.pplnextgen.com/Get-Started/Authentication-Information, https://developer.pplnextgen.com/Get-Started/Base-API-Standard]\naudience:\n  note: >-\n    Where the downstream API validates the audience claim, the gateway may need an on-behalf-of\n    token with the correct audience set. PPL does not publish the audience/resource identifier\n    values — they are issued per organisation and per environment during onboarding.\n  published: false\nnot_published:\n- Per-API or per-resource scopes (there is no read:placements / write:contracts style catalogue).\n- A scopes or permissions reference page.\n- Any consent screen or scope-selection UI for third-party applications.\nauthorization_model:\n  primary: single delegated Entra ID scope (user_impersonation)\n  secondary: >-\n    Team and user context supplied on every call via X-Auth-Team and X-Auth-Impersonated-User,\n\
  \    validated by the platform. An invalid combination returns HTTP 404 with error code\n    INVALID_ROLE_OR_TEAM.\n  transport: mutual TLS with a per-environment registered X.509 client certificate\nrelated:\n  authentication: authentication/ppl-london-market-authentication.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ppl-london-market/refs/heads/main/scopes/ppl-london-market-scopes.yml
summary_line: 1 scope · authorizationCode/onBehalfOf/clientCredentials
tags:
- Insurance
- United Kingdom
- London Market
- Lloyd's of London
- Reinsurance
- Commercial Insurance
- Brokers
- Underwriting
- Placement
- Market Infrastructure
- ACORD
- Electronic Placing
token_urls:
- https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
---
