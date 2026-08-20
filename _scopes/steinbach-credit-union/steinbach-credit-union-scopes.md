---
authorization_urls: []
description: ''
docs: https://online.scu.mb.ca/am/oauth2
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Steinbach Credit Union Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Steinbach Credit Union publishes 7 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Steinbach Credit Union API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Steinbach Credit Union
provider_slug: steinbach-credit-union
schemes:
- authorizationUrl: https://online.scu.mb.ca/am/oauth2/authorize
  name: oauth2
  source: well-known/steinbach-credit-union-openid-configuration.json
  tokenUrl: https://online.scu.mb.ca/am/oauth2/steinbach_token
scope_count: 7
scope_names:
- openid
- profile
- email
- address
- phone
- fr:idm:*
- am-introspect-all-tokens
scopes:
- description: OpenID Connect authentication; returns an ID token.
  flows: []
  scope: openid
- description: Standard OIDC profile claims for the authenticated member.
  flows: []
  scope: profile
- description: Member email-address claim.
  flows: []
  scope: email
- description: Member postal-address claim.
  flows: []
  scope: address
- description: Member phone-number claim.
  flows: []
  scope: phone
- description: ForgeRock Identity Management resource access (AM/IDM platform scope).
  flows: []
  scope: fr:idm:*
- description: ForgeRock AM administrative scope permitting introspection of all tokens.
  flows: []
  scope: am-introspect-all-tokens
slug: steinbach-credit-union-scopes
source_filename: steinbach-credit-union-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: https://online.scu.mb.ca/.well-known/openid-configuration\ndocs: https://online.scu.mb.ca/am/oauth2\nscope_note: >-\n  Scopes advertised by the ForgeRock/Ping AM OAuth2 server behind SCU's\n  members-only digital banking (issuer https://online.scu.mb.ca/am/oauth2).\n  These are the standard OIDC scopes plus the AM platform's identity-management\n  scopes; they are NOT a public developer-API permission surface. Captured from\n  scopes_supported in the anonymously published OIDC discovery document.\nschemes:\n- name: oauth2\n  source: well-known/steinbach-credit-union-openid-configuration.json\n  authorizationUrl: https://online.scu.mb.ca/am/oauth2/authorize\n  tokenUrl: https://online.scu.mb.ca/am/oauth2/steinbach_token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; returns an ID token.\n- scope: profile\n  description: Standard OIDC profile claims for the authenticated member.\n- scope: email\n  description:\
  \ Member email-address claim.\n- scope: address\n  description: Member postal-address claim.\n- scope: phone\n  description: Member phone-number claim.\n- scope: 'fr:idm:*'\n  description: ForgeRock Identity Management resource access (AM/IDM platform scope).\n- scope: am-introspect-all-tokens\n  description: ForgeRock AM administrative scope permitting introspection of all tokens.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/steinbach-credit-union/refs/heads/main/scopes/steinbach-credit-union-scopes.yml
summary_line: 7 scopes
tags:
- Financial-Services
- Banking
- Canada
- Credit Union
- Cooperative
- Manitoba
- Interac
- Data Aggregation
- Open Banking
token_urls: []
---
