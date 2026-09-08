---
api_specs:
- filename: amtrust-financial-services-digital-wc-api-openapi.json
  format: json
  label: AmTrust Digital WC API
  slug: amtrust-financial-services-digital-wc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amtrust-financial-services/refs/heads/main/openapi/amtrust-financial-services-digital-wc-api-openapi.json
- filename: amtrust-financial-services-digital-bop-api-openapi.json
  format: json
  label: AmTrust Digital BOP API
  slug: amtrust-financial-services-digital-bop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amtrust-financial-services/refs/heads/main/openapi/amtrust-financial-services-digital-bop-api-openapi.json
- filename: amtrust-financial-services-digital-cyber-api-openapi.json
  format: json
  label: AmTrust Digital Cyber API
  slug: amtrust-financial-services-digital-cyber-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amtrust-financial-services/refs/heads/main/openapi/amtrust-financial-services-digital-cyber-api-openapi.json
- filename: amtrust-financial-services-digital-es-api-openapi.json
  format: json
  label: AmTrust Digital E&S API
  slug: amtrust-financial-services-digital-es-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amtrust-financial-services/refs/heads/main/openapi/amtrust-financial-services-digital-es-api-openapi.json
- filename: amtrust-financial-services-digital-pac-api-openapi.json
  format: json
  label: AmTrust Digital PAC API
  slug: amtrust-financial-services-digital-pac-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amtrust-financial-services/refs/heads/main/openapi/amtrust-financial-services-digital-pac-api-openapi.json
- filename: amtrust-financial-services-reinsurance-contract-entry-api-openapi.json
  format: json
  label: AmTrust Reinsurance Contract Entry API
  slug: amtrust-financial-services-reinsurance-contract-entry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amtrust-financial-services/refs/heads/main/openapi/amtrust-financial-services-reinsurance-contract-entry-api-openapi.json
- filename: amtrust-financial-services-experience-claims-medical-case-api-openapi.json
  format: json
  label: AmTrust Experience Claims Medical Case API
  slug: amtrust-financial-services-experience-claims-medical-case-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amtrust-financial-services/refs/heads/main/openapi/amtrust-financial-services-experience-claims-medical-case-api-openapi.json
- filename: amtrust-financial-services-experience-next-gen-bond-pro-api-openapi.json
  format: json
  label: AmTrust Experience Next Gen Bond Pro API
  slug: amtrust-financial-services-experience-next-gen-bond-pro-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amtrust-financial-services/refs/heads/main/openapi/amtrust-financial-services-experience-next-gen-bond-pro-api-openapi.json
- filename: amtrust-financial-services-conversa-engine-api-openapi.json
  format: json
  label: AmTrust Conversa Engine API
  slug: amtrust-financial-services-conversa-engine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amtrust-financial-services/refs/heads/main/openapi/amtrust-financial-services-conversa-engine-api-openapi.json
authorization_urls: []
description: ''
docs: https://apiportal.amtrustgroup.com/authentication
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Amtrust Financial Services Scopes
name_suffix: OAuth Scopes
note: 'These scopes come from AmTrust''s own OpenID Connect discovery document, not from any OpenAPI securityScheme — none of the nine harvested OpenAPI documents declares an oauth2 or openIdConnect scheme, so `derive-oauth-scopes.py` correctly found nothing to derive. The scope set is coarse: it authenticates the caller and carries legacy portal identity, and does NOT partition the API surface. There is no read/write split, no per-product scope (workers'' comp vs BOP vs claims vs reinsurance), and no per-operation scope. Authorization to a given API is enforced by the Azure API Management subscription (which product a subscriber_id is entitled to), not by the token.'
overview: 'AmTrust Financial Services uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AmTrust Financial Services
provider_slug: amtrust-financial-services
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: amtrust-financial-services-scopes
source_filename: amtrust-financial-services-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: >-\n  https://auth.amtrustgroup.com/AuthServer/.well-known/openid-configuration (HTTP 200) and\n  https://apiportal.amtrustgroup.com/authentication (HTTP 200) — probed 2026-09-02\ndocs: https://apiportal.amtrustgroup.com/authentication\nprovider: AmTrust Financial Services\nproviderId: amtrust-financial-services\nissuer: https://auth.amtrustgroup.com/AuthServer\ntoken_endpoint: https://auth.amtrustgroup.com/AuthServer/OpenIDConnect/Token\nnote: >-\n  These scopes come from AmTrust's own OpenID Connect discovery document, not from any OpenAPI\n  securityScheme — none of the nine harvested OpenAPI documents declares an oauth2 or openIdConnect\n  scheme, so `derive-oauth-scopes.py` correctly found nothing to derive. The scope set is coarse: it\n  authenticates the caller and carries legacy portal identity, and does NOT partition the API surface.\n  There is no read/write split, no per-product scope (workers' comp vs BOP vs claims\
  \ vs reinsurance),\n  and no per-operation scope. Authorization to a given API is enforced by the Azure API Management\n  subscription (which product a subscriber_id is entitled to), not by the token.\nscope_count: 7\nscopes:\n- name: openid\n  description: Standard OIDC scope. Requests an ID token identifying the caller.\n  requested_by: both documented flows\n- name: profile\n  description: Standard OIDC profile claims.\n  requested_by: both documented flows\n- name: offline_access\n  description: Requests a refresh token.\n  requested_by: advertised in discovery; not shown in the portal's documented flows\n- name: user\n  description: >-\n    AmTrust-specific. Advertised in discovery; the portal does not document it and does not state what\n    it grants.\n  requested_by: advertised in discovery only\n- name: legacy_id\n  description: >-\n    AmTrust-specific. Carries the caller's legacy AmTrust portal user identifier into the token.\n    Documented on the portal as part of the User\
  \ Authenticated Token request.\n  requested_by: User Authenticated Token (password grant)\n- name: legacy_info\n  description: >-\n    AmTrust-specific. Carries legacy AmTrust portal user information into the token. Documented on the\n    portal as part of the User Authenticated Token request.\n  requested_by: User Authenticated Token (password grant)\n- name: legacy_permission\n  description: >-\n    AmTrust-specific. Advertised in discovery; the portal does not document it and does not state what\n    permissions it conveys.\n  requested_by: advertised in discovery only\ndocumented_combinations:\n- flow: General Access Token\n  grant_type: client_credentials\n  scope: openid profile\n- flow: User Authenticated Token\n  grant_type: password\n  scope: openid profile legacy_info legacy_id\ngaps:\n- No scope maps to an API product or an operation, so a token cannot express least privilege.\n- Three advertised scopes (user, legacy_permission, offline_access) are undocumented.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amtrust-financial-services/refs/heads/main/scopes/amtrust-financial-services-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Commercial Insurance
- Insurance
- Property and Casualty
- Small Business
- Workers Compensation
- Fortune 1000
- Underwriting
- Claims
- Policy
- Reinsurance
- Cyber Insurance
- Surety
token_urls: []
---
