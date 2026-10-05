---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Andersons Scopes
name_suffix: OAuth Scopes
note: Scopes read verbatim from `scopes_supported` in the OIDC discovery document The Andersons serves at portalauth.andersonsinc.com. These are the Microsoft ADFS built-in scopes for the company's portal federation service, not scopes of a business API — The Andersons publishes no API and no scope reference page. Descriptions below are the ADFS-defined meanings, marked as such; the provider does not document them itself.
overview: 'The Andersons publishes 9 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the The Andersons API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: The Andersons
provider_slug: andersons
schemes: []
scope_count: 9
scope_names:
- openid
- profile
- email
- allatclaims
- aza
- user_impersonation
- logon_cert
- winhello_cert
- vpn_cert
scopes:
- description: Request an OpenID Connect id_token for the signed-in user.
  flows: []
  scope: openid
- description: Release the user's profile claims (unique_name, upn, sid).
  flows: []
  scope: profile
- description: Release the user's email claim.
  flows: []
  scope: email
- description: Release all claims that would appear in the access token into the id_token as well.
  flows: []
  scope: allatclaims
- description: Microsoft broker/multi-resource refresh-token scope (primary refresh token).
  flows: []
  scope: aza
- description: Act on behalf of the signed-in user against a relying-party resource.
  flows: []
  scope: user_impersonation
- description: Issue a logon certificate for the authenticated user.
  flows: []
  scope: logon_cert
- description: Issue a Windows Hello for Business certificate.
  flows: []
  scope: winhello_cert
- description: Issue a VPN client certificate.
  flows: []
  scope: vpn_cert
slug: andersons-scopes
source_filename: andersons-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: https://portalauth.andersonsinc.com/adfs/.well-known/openid-configuration\ndocs: null\nnote: >-\n  Scopes read verbatim from `scopes_supported` in the OIDC discovery document The Andersons\n  serves at portalauth.andersonsinc.com. These are the Microsoft ADFS built-in scopes for the\n  company's portal federation service, not scopes of a business API — The Andersons publishes\n  no API and no scope reference page. Descriptions below are the ADFS-defined meanings, marked\n  as such; the provider does not document them itself.\nissuer: https://portalauth.andersonsinc.com/adfs\nscope_count: 9\nscopes:\n  - name: openid\n    description: Request an OpenID Connect id_token for the signed-in user.\n    origin: adfs-builtin\n  - name: profile\n    description: Release the user's profile claims (unique_name, upn, sid).\n    origin: adfs-builtin\n  - name: email\n    description: Release the user's email claim.\n    origin: adfs-builtin\n\
  \  - name: allatclaims\n    description: Release all claims that would appear in the access token into the id_token as well.\n    origin: adfs-builtin\n  - name: aza\n    description: Microsoft broker/multi-resource refresh-token scope (primary refresh token).\n    origin: adfs-builtin\n  - name: user_impersonation\n    description: Act on behalf of the signed-in user against a relying-party resource.\n    origin: adfs-builtin\n  - name: logon_cert\n    description: Issue a logon certificate for the authenticated user.\n    origin: adfs-builtin\n  - name: winhello_cert\n    description: Issue a Windows Hello for Business certificate.\n    origin: adfs-builtin\n  - name: vpn_cert\n    description: Issue a VPN client certificate.\n    origin: adfs-builtin\nclaims_supported:\n  - aud\n  - iss\n  - iat\n  - exp\n  - auth_time\n  - nonce\n  - at_hash\n  - c_hash\n  - sub\n  - upn\n  - unique_name\n  - pwd_url\n  - pwd_exp\n  - mfa_auth_time\n  - sid\ngaps:\n  - The provider publishes no scope/permission\
  \ reference page; nothing here is provider-authored prose.\n  - No API-specific scopes exist because no API is published.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/andersons/refs/heads/main/scopes/andersons-scopes.yml
summary_line: 9 scopes
tags:
- Agribusiness
- Agriculture
- Grain
- Commodity Merchandising
- Plant Nutrients
- Fertilizer
- Renewables
- Ethanol
- Food and Feed Ingredients
- Turf and Specialty Products
- Rail Leasing
- Supply Chain
token_bound: false
token_urls: []
---
