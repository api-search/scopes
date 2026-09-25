---
authorization_urls:
- https://gateway-portal.hub-verify.innovation.interac.ca/auth
description: ''
docs: https://documents.hub-verify.innovation.interac.ca/docs/pre-configured-scopes
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Interac Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Interac publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Interac API on a user''s behalf.


  Tokens are issued from https://gateway-portal.hub-verify.innovation.interac.ca/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Interac
provider_slug: interac
schemes:
- flows:
  - authorizationUrl: https://gateway-portal.hub-verify.innovation.interac.ca/auth
    flow: authorizationCode
    tokenUrl: https://gateway-portal.hub-verify.innovation.interac.ca/oauth2/token
  issuer: https://gateway-portal.hub-verify.innovation.interac.ca/
  name: openid_connect
  source: well-known/interac-openid-configuration.json
scope_count: 3
scope_names:
- openid
- offline_access
- offline
scopes:
- description: Base OpenID Connect scope; required on every request.
  flows: []
  scope: openid
- description: Request a refresh token for offline access.
  flows: []
  scope: offline_access
- description: Legacy offline-access alias advertised by the provider.
  flows: []
  scope: offline
slug: interac-scopes
source_filename: interac-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: https://gateway-portal.hub-verify.innovation.interac.ca/.well-known/openid-configuration\ndocs: https://documents.hub-verify.innovation.interac.ca/docs/pre-configured-scopes\nschemes:\n- name: openid_connect\n  source: well-known/interac-openid-configuration.json\n  issuer: https://gateway-portal.hub-verify.innovation.interac.ca/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://gateway-portal.hub-verify.innovation.interac.ca/auth\n    tokenUrl: https://gateway-portal.hub-verify.innovation.interac.ca/oauth2/token\n# Standard OIDC scopes advertised by the discovery document\nscopes:\n- scope: openid\n  description: Base OpenID Connect scope; required on every request.\n  sources: [well-known/interac-openid-configuration.json, docs]\n- scope: offline_access\n  description: Request a refresh token for offline access.\n  sources: [well-known/interac-openid-configuration.json]\n- scope: offline\n  description:\
  \ Legacy offline-access alias advertised by the provider.\n  sources: [well-known/interac-openid-configuration.json]\n# Pre-configured product scopes documented in the Integration Guide appendix.\n# Each is requested combined with the base `openid` scope, e.g. \"openid onlyVme_scope\".\nproduct_scopes:\n- scope: onlyVme_scope\n  request: openid onlyVme_scope\n  flow: IVS\n  description: >-\n    Presents the user with the Interac verification service financial-institution\n    selection screen (Interac Verification Service only).\n  source: docs\n- scope: document_scope\n  request: openid document_scope\n  flow: IDVS\n  description: >-\n    Presents the user with the Interac document verification service screen for\n    government-ID document and biometric selfie scanning.\n  returns_claims:\n  - doc_type\n  - scan_result\n  - suspected_flags\n  - rejected_flags\n  - doc_number\n  - birthdate\n  - expiry_date\n  - family_name\n  - given_name\n  - issue_date\n  - issuing_authority\n  - issuing_country\n\
  \  - nationality\n  - address\n  - source\n  - sub\n  - com.securekey.verified.me.ui_locale\n  - com.securekey.vids.job_id\n  source: docs\n- scope: general_scope\n  request: openid general_scope\n  flow: IVS | IDVS\n  description: >-\n    Presents the user with an option to choose the Interac verification service\n    flow OR the document verification service flow; claims vary by user selection.\n  source: docs\n- scope: dual_scope\n  request: openid dual_scope\n  flow: IVS + IDVS\n  description: >-\n    Two-step flow: the user completes the Interac verification service flow first\n    and then document verification. Returns the combined IVS + IDVS claims plus\n    match scores comparing the verified financial-institution data against the\n    scanned document (populated when both flows complete with CLEAR status).\n  source: docs\nnotes: >-\n  The discovery document advertises only the base OIDC scopes (openid,\n  offline_access, offline). The product scopes above (onlyVme_scope,\n \
  \ document_scope, general_scope, dual_scope) are pre-configured per relying\n  party and documented in the Hub Integration Guide appendix rather than in the\n  discovery metadata; the exact scope strings provisioned for a partner are\n  issued during onboarding.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/interac/refs/heads/main/scopes/interac-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Financial Services
- Payments
- Canada
- Interac
- Digital Identity
- Verification
- Open Banking
- Consumer-Driven Banking
- Infrastructure
token_urls:
- https://gateway-portal.hub-verify.innovation.interac.ca/oauth2/token
---
