---
authorization_urls:
- https://login.goodenergy.co.uk/connect/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
- implicit
- deviceCode
- ciba
kind: oauth-scopes
layout: scope
method: derived
name: Good Energy Scopes
name_suffix: OAuth Scopes
note: 'Harvested verbatim from scopes_supported in the live OpenID Connect Discovery document. Good Energy publishes NO scopes/permissions reference page — there is no developer portal — so descriptions for the two non-standard scopes are read from their names and from the customer-hub surface they gate, and are marked inferred_description. Nothing here is invented: every scope string is present in the fetched discovery document. These are PORTAL scopes (billing and tariff self-service), not energy consumption-data scopes; there is no registration_endpoint, so no third party can request them.'
overview: 'Good Energy publishes 6 OAuth 2.0 scopes via the authorizationCode, clientCredentials, implicit, deviceCode, and ciba flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Good Energy API on a user''s behalf.


  Tokens are issued from https://login.goodenergy.co.uk/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Good Energy
provider_slug: good-energy
schemes:
- flows:
  - authorizationUrl: https://login.goodenergy.co.uk/connect/authorize
    flow: authorizationCode
    tokenUrl: https://login.goodenergy.co.uk/connect/token
  - flow: clientCredentials
    tokenUrl: https://login.goodenergy.co.uk/connect/token
  - authorizationUrl: https://login.goodenergy.co.uk/connect/authorize
    flow: implicit
  - deviceAuthorizationUrl: https://login.goodenergy.co.uk/connect/deviceauthorization
    flow: deviceCode
  - backchannelAuthenticationUrl: https://login.goodenergy.co.uk/connect/ciba
    flow: ciba
  issuer: https://login.goodenergy.co.uk
  name: GoodEnergyCustomerIdentity
  source: authentication/good-energy-openid-configuration.json
  type: openIdConnect
scope_count: 6
scope_names:
- openid
- profile
- email
- offline_access
- customer_portal
- customer_portal_tariff_switch
scopes:
- description: Standard OpenID Connect scope requesting an ID token for the signed-in customer.
  flows: []
  scope: openid
- description: Standard OIDC claims about the end user (name, family_name, given_name, preferred_username, picture, locale, zoneinfo, updated_at and related claims advertised in claims_supported).
  flows: []
  scope: profile
- description: Standard OIDC email and email_verified claims.
  flows: []
  scope: email
- description: Requests a refresh token so the session can be renewed without re-authentication.
  flows: []
  scope: offline_access
- description: Access to the Good Energy customer hub (account.goodenergy.co.uk) — the signed-in billing, usage and account self-service surface.
  flows: []
  scope: customer_portal
- description: Elevated customer-hub capability covering tariff switching / change of tariff within the customer account.
  flows: []
  scope: customer_portal_tariff_switch
slug: good-energy-scopes
source_filename: good-energy-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: derived\nsource: authentication/good-energy-openid-configuration.json\nsource_url: https://login.goodenergy.co.uk/.well-known/openid-configuration\nfetched: '2026-07-27'\nhttp_status: 200\ndocs: null\nnote: >-\n  Harvested verbatim from scopes_supported in the live OpenID Connect Discovery document. Good Energy\n  publishes NO scopes/permissions reference page — there is no developer portal — so descriptions for\n  the two non-standard scopes are read from their names and from the customer-hub surface they gate,\n  and are marked inferred_description. Nothing here is invented: every scope string is present in the\n  fetched discovery document. These are PORTAL scopes (billing and tariff self-service), not energy\n  consumption-data scopes; there is no registration_endpoint, so no third party can request them.\nschemes:\n- name: GoodEnergyCustomerIdentity\n  type: openIdConnect\n  source: authentication/good-energy-openid-configuration.json\n\
  \  issuer: https://login.goodenergy.co.uk\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.goodenergy.co.uk/connect/authorize\n    tokenUrl: https://login.goodenergy.co.uk/connect/token\n  - flow: clientCredentials\n    tokenUrl: https://login.goodenergy.co.uk/connect/token\n  - flow: implicit\n    authorizationUrl: https://login.goodenergy.co.uk/connect/authorize\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://login.goodenergy.co.uk/connect/deviceauthorization\n  - flow: ciba\n    backchannelAuthenticationUrl: https://login.goodenergy.co.uk/connect/ciba\nscopes:\n- scope: openid\n  description: Standard OpenID Connect scope requesting an ID token for the signed-in customer.\n  standard: OpenID Connect Core 1.0\n  sources:\n  - authentication/good-energy-openid-configuration.json\n- scope: profile\n  description: Standard OIDC claims about the end user (name, family_name, given_name, preferred_username,\n    picture, locale, zoneinfo, updated_at and\
  \ related claims advertised in claims_supported).\n  standard: OpenID Connect Core 1.0\n  sources:\n  - authentication/good-energy-openid-configuration.json\n- scope: email\n  description: Standard OIDC email and email_verified claims.\n  standard: OpenID Connect Core 1.0\n  sources:\n  - authentication/good-energy-openid-configuration.json\n- scope: offline_access\n  description: Requests a refresh token so the session can be renewed without re-authentication.\n  standard: OpenID Connect Core 1.0\n  sources:\n  - authentication/good-energy-openid-configuration.json\n- scope: customer_portal\n  description: Access to the Good Energy customer hub (account.goodenergy.co.uk) — the signed-in\n    billing, usage and account self-service surface.\n  inferred_description: true\n  standard: provider-specific\n  sources:\n  - authentication/good-energy-openid-configuration.json\n- scope: customer_portal_tariff_switch\n  description: Elevated customer-hub capability covering tariff switching / change\
  \ of tariff within\n    the customer account.\n  inferred_description: true\n  standard: provider-specific\n  sources:\n  - authentication/good-energy-openid-configuration.json\naccess:\n  third_party_obtainable: false\n  reason: >-\n    The discovery document exposes no registration_endpoint and Good Energy publishes no developer\n    portal, partner API programme or client-onboarding form, so no third party can obtain a client_id\n    with which to request any of these scopes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/good-energy/refs/heads/main/scopes/good-energy-scopes.yml
summary_line: 6 scopes · authorizationCode/clientCredentials/implicit/deviceCode/ciba
tags:
- Energy
- United Kingdom
- Utilities
- Electricity
- Gas
- Renewables
- Smart Metering
- Solar
- EV Charging
- Energy Retail
token_urls:
- https://login.goodenergy.co.uk/connect/token
---
