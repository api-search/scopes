---
authorization_urls: []
description: 'Lloyd''s market APIs do not publish a granular OAuth scope catalogue. The Base API Standard mandates exactly one scope value on the consumer''s bearer token - the Azure AD delegated permission "user_impersonation" - and pushes all finer-grained authorisation onto JWT claims evaluated by the API Provider rather than onto scopes. This is a deliberately coarse scope surface: possession of a registered X.509 certificate plus a user_impersonation on-behalf-of token is the access decision, and per-resource authorisation is done from sub/upn/lmg_* claims inside the provider.'
docs: https://web.archive.org/web/20200930085423/https://developer.lloyds.com/Get-Started/Authentication-Information
flows:
- authorizationCode
- on-behalf-of
kind: oauth-scopes
layout: scope
method: searched
name: Lloyds Of London Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Lloyd''s of London publishes 1 OAuth 2.0 scope via the authorizationCode and on-behalf-of flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Lloyd''s of London API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Lloyd's of London
provider_slug: lloyds-of-london
schemes:
- flows:
  - authority: https://login.microsoftonline.com/{tenantId}
    flow: authorizationCode
  - flow: on-behalf-of
    grant_type: urn:ietf:params:oauth:grant-type:jwt-bearer
  name: AzureADBearer
  source: Lloyd's Base API Standard section 5.12.1
  type: oauth2
scope_count: 1
scope_names:
- user_impersonation
scopes:
- description: The only scope value the Lloyd's Base API Standard names. "The JWT MUST contain a claim called 'scp' and it must have the value of 'user_impersonation'." If the token returned from the login does not already carry it, the application must obtain an on-behalf-of token from Azure AD that does.
  flows:
  - authorizationCode
  - on-behalf-of
  scope: user_impersonation
slug: lloyds-of-london-scopes
source_filename: lloyds-of-london-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: >-\n  https://web.archive.org/web/20200930095802/https://developer.lloyds.com/Get-Started/Base-API-Standard\n  (section 5.12.1 API Consumer Security Rules)\ndocs: https://web.archive.org/web/20200930085423/https://developer.lloyds.com/Get-Started/Authentication-Information\ndescription: >-\n  Lloyd's market APIs do not publish a granular OAuth scope catalogue. The Base API Standard\n  mandates exactly one scope value on the consumer's bearer token - the Azure AD delegated\n  permission \"user_impersonation\" - and pushes all finer-grained authorisation onto JWT claims\n  evaluated by the API Provider rather than onto scopes. This is a deliberately coarse scope\n  surface: possession of a registered X.509 certificate plus a user_impersonation on-behalf-of\n  token is the access decision, and per-resource authorisation is done from sub/upn/lmg_* claims\n  inside the provider.\nidentity_provider: Azure Active Directory (LIMOSS\
  \ Common Services tenant, one per environment)\nschemes:\n- name: AzureADBearer\n  type: oauth2\n  source: Lloyd's Base API Standard section 5.12.1\n  flows:\n  - flow: authorizationCode\n    authority: https://login.microsoftonline.com/{tenantId}\n  - flow: on-behalf-of\n    grant_type: urn:ietf:params:oauth:grant-type:jwt-bearer\nscopes:\n- scope: user_impersonation\n  claim: scp\n  required: true\n  description: >-\n    The only scope value the Lloyd's Base API Standard names. \"The JWT MUST contain a claim\n    called 'scp' and it must have the value of 'user_impersonation'.\" If the token returned from\n    the login does not already carry it, the application must obtain an on-behalf-of token from\n    Azure AD that does.\n  flows: [authorizationCode, on-behalf-of]\n  sources: [\"Lloyd's Base API Standard section 5.12.1\"]\nauthorization_beyond_scopes:\n  mechanism: JWT claim evaluation by the API Provider\n  claims: [sub, upn, amr, aud, iss, appid, oid, lmg_mpo, lmg_cert_dn, lmg_pkt]\n\
  \  note: >-\n    \"The API Provider may use any field in the JWT for authorisation purposes.\" Multi-factor\n    authentication is signalled by an \"amr\" claim containing \"mfa\".\ngaps:\n- No scopes/permissions reference page is published; the developer portal that carried the Base\n  API Standard now redirects to www.lloyds.com.\n- The published OIDC discovery documents at /discovery/.well-known/openid-configuration carry only\n  issuer and jwks_uri - no scopes_supported, authorization_endpoint or token_endpoint - so the\n  scope set cannot be enumerated from discovery.\nrelated:\n- authentication/lloyds-of-london-authentication.yml\n- well-known/lloyds-of-london-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lloyds-of-london/refs/heads/main/scopes/lloyds-of-london-scopes.yml
summary_line: 1 scope · authorizationCode/on-behalf-of
tags:
- Insurance
- United Kingdom
- Reinsurance
- Specialty Insurance
- London Market
- Underwriting
- Claims
- Delegated Authority
- Brokers
- Market Infrastructure
- Standards
- ACORD
token_urls: []
---
