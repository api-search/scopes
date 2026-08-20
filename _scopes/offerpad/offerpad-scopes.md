---
api_specs:
- filename: offerpad-wordpress-wp-v2-openapi.yml
  format: yaml
  label: Offerpad WordPress REST API
  slug: offerpad-wordpress-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/offerpad/refs/heads/main/openapi/offerpad-wordpress-wp-v2-openapi.yml
authorization_urls:
- https://offerpad.okta.com/oauth2/ausftur6n2aTu6Sur357/v1/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Offerpad Scopes
name_suffix: OAuth Scopes
note: Offerpad publishes no scope reference page. Every scope below is taken verbatim from the scopes_supported array of an anonymously fetchable RFC 8414 / OpenID Connect discovery document. Descriptions are the standard OpenID Connect and Okta meanings for these scope names — Offerpad documents none of them. The helix backend advertises only the three OIDC scopes; the underlying Okta custom authorization server advertises a wider set that includes Okta's own MyAccount scopes, which are platform scopes rather than Offerpad business scopes.
overview: 'Offerpad publishes 9 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Offerpad API on a user''s behalf.


  Tokens are issued from https://offerpad.okta.com/oauth2/ausftur6n2aTu6Sur357/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Offerpad
provider_slug: offerpad
schemes:
- flows:
  - authorizationUrl: https://offerpad.okta.com/oauth2/ausftur6n2aTu6Sur357/v1/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://offerpad.okta.com/oauth2/ausftur6n2aTu6Sur357/v1/token
  name: offerpadHelixOAuth
  source: well-known/offerpad-helix-oauth-authorization-server.json
scope_count: 9
scope_names:
- openid
- profile
- email
- address
- phone
- offline_access
- device_sso
- groups
- interclient_access
scopes:
- description: Request an OpenID Connect ID token for the signed-in Offerpad customer.
  flows:
  - authorizationCode
  scope: openid
- description: Basic profile claims (name, preferred_username, locale, updated_at).
  flows:
  - authorizationCode
  scope: profile
- description: Email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Physical address claim.
  flows:
  - authorizationCode
  scope: address
- description: Phone number and phone_number_verified claims.
  flows:
  - authorizationCode
  scope: phone
- description: Issue a refresh token so the client can renew access without re-prompting.
  flows:
  - authorizationCode
  scope: offline_access
- description: Okta device single sign-on token issuance.
  flows:
  - authorizationCode
  scope: device_sso
- description: Group memberships of the signed-in user (Okta org authorization server only).
  flows:
  - authorizationCode
  scope: groups
- description: Okta token-exchange scope allowing one client to act for another.
  flows:
  - authorizationCode
  scope: interclient_access
slug: offerpad-scopes
source_filename: offerpad-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: >-\n  https://helix.offerpad.com/.well-known/oauth-authorization-server and\n  https://offerpad.okta.com/oauth2/ausftur6n2aTu6Sur357/.well-known/openid-configuration\nnote: >-\n  Offerpad publishes no scope reference page. Every scope below is taken verbatim from the\n  scopes_supported array of an anonymously fetchable RFC 8414 / OpenID Connect discovery\n  document. Descriptions are the standard OpenID Connect and Okta meanings for these scope\n  names — Offerpad documents none of them. The helix backend advertises only the three\n  OIDC scopes; the underlying Okta custom authorization server advertises a wider set that\n  includes Okta's own MyAccount scopes, which are platform scopes rather than Offerpad\n  business scopes.\nschemes:\n  - name: offerpadHelixOAuth\n    source: well-known/offerpad-helix-oauth-authorization-server.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://offerpad.okta.com/oauth2/ausftur6n2aTu6Sur357/v1/authorize\n\
  \        tokenUrl: https://offerpad.okta.com/oauth2/ausftur6n2aTu6Sur357/v1/token\n        pkce: S256\nscopes:\n  - scope: openid\n    description: Request an OpenID Connect ID token for the signed-in Offerpad customer.\n    flows: [authorizationCode]\n    advertised_by: [helix, okta-custom-as, okta-org-as]\n    sources: [well-known/offerpad-helix-oauth-authorization-server.json]\n  - scope: profile\n    description: Basic profile claims (name, preferred_username, locale, updated_at).\n    flows: [authorizationCode]\n    advertised_by: [helix, okta-custom-as, okta-org-as]\n    sources: [well-known/offerpad-helix-oauth-authorization-server.json]\n  - scope: email\n    description: Email address and email_verified claim.\n    flows: [authorizationCode]\n    advertised_by: [helix, okta-custom-as, okta-org-as]\n    sources: [well-known/offerpad-helix-oauth-authorization-server.json]\n  - scope: address\n    description: Physical address claim.\n    flows: [authorizationCode]\n    advertised_by:\
  \ [okta-custom-as, okta-org-as]\n    sources: [well-known/offerpad-okta-openid-configuration.json]\n  - scope: phone\n    description: Phone number and phone_number_verified claims.\n    flows: [authorizationCode]\n    advertised_by: [okta-custom-as, okta-org-as]\n    sources: [well-known/offerpad-okta-openid-configuration.json]\n  - scope: offline_access\n    description: Issue a refresh token so the client can renew access without re-prompting.\n    flows: [authorizationCode]\n    advertised_by: [okta-custom-as, okta-org-as]\n    sources: [well-known/offerpad-okta-openid-configuration.json]\n  - scope: device_sso\n    description: Okta device single sign-on token issuance.\n    flows: [authorizationCode]\n    advertised_by: [okta-custom-as]\n    sources: [well-known/offerpad-okta-openid-configuration.json]\n  - scope: groups\n    description: Group memberships of the signed-in user (Okta org authorization server only).\n    flows: [authorizationCode]\n    advertised_by: [okta-org-as]\n\
  \    sources: [well-known/offerpad-okta-org-openid-configuration.json]\n  - scope: interclient_access\n    description: Okta token-exchange scope allowing one client to act for another.\n    flows: [authorizationCode]\n    advertised_by: [okta-custom-as]\n    sources: [well-known/offerpad-okta-openid-configuration.json]\nplatform_scopes:\n  note: >-\n    Okta MyAccount management scopes advertised by the custom authorization server. These\n    govern the end user's own Okta account, not Offerpad business data.\n  scopes:\n    - okta.myAccount.read\n    - okta.myAccount.manage\n    - okta.myAccount.profile.read\n    - okta.myAccount.profile.manage\n    - okta.myAccount.email.read\n    - okta.myAccount.email.manage\n    - okta.myAccount.phone.read\n    - okta.myAccount.phone.manage\n    - okta.myAccount.authenticators.read\n    - okta.myAccount.authenticators.manage\n    - okta.myAccount.appAuthenticator.read\n    - okta.myAccount.appAuthenticator.manage\n    - okta.myAccount.appAuthenticator.maintenance.read\n\
  \    - okta.myAccount.appAuthenticator.maintenance.manage\n    - okta.myAccount.oktaApplications.read\n    - okta.myAccount.organization.read\ngaps:\n  - No Offerpad business scope (property, offer, contract, transaction, document) is advertised anywhere.\n  - No public client registration, so a third party cannot exercise any of these scopes.\n  - Offerpad publishes no scopes/permissions reference page to enrich these descriptions from.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/offerpad/refs/heads/main/scopes/offerpad-scopes.yml
summary_line: 9 scopes · authorizationCode
tags:
- Real-Estate
- United States
- iBuyer
- PropTech
- Property Listings
- Brokerage
- MLS
- Cash Offer
- Renovation
- Home Buying
token_urls:
- https://offerpad.okta.com/oauth2/ausftur6n2aTu6Sur357/v1/token
---
