---
api_specs:
- filename: ppl-london-market-placements.json
  format: json
  label: PPL Placements API
  slug: ppl-placements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppl-london-market/refs/heads/main/openapi/ppl-london-market-placements.json
- filename: ppl-london-market-submissions.json
  format: json
  label: PPL Submissions API
  slug: ppl-submissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppl-london-market/refs/heads/main/openapi/ppl-london-market-submissions.json
- filename: ppl-london-market-organisations.json
  format: json
  label: PPL Organisations API
  slug: ppl-organisations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppl-london-market/refs/heads/main/openapi/ppl-london-market-organisations.json
- filename: ppl-london-market-documents.json
  format: json
  label: PPL Documents API
  slug: ppl-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppl-london-market/refs/heads/main/openapi/ppl-london-market-documents.json
- filename: ppl-london-market-events.json
  format: json
  label: PPL Events API
  slug: ppl-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppl-london-market/refs/heads/main/openapi/ppl-london-market-events.json
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
