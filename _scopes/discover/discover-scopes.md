---
authorization_urls:
- https://identity.discoverglobalnetwork.com/oauth2/default/v1/authorize
description: ''
docs: https://partner.discoverglobalnetwork.com/going-live-with-discover?tab=developer-guide
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Discover Scopes
name_suffix: OAuth Scopes
note: Discover documents an OAuth 2.0 client-credentials scope model but does NOT publish a scope catalogue. Section 2.1 of the developer guide states scopes are "provided in the Discover Developer Center upon review by Discover" and the request form is literally scope=DISCOVER_SCOPE_NAME - a placeholder. The concrete scope names are issued per partner, per API product and per environment behind the invitation-only Developer Center login, so no scope list is recorded here. The published scopes below belong to the Okta authorization server that signs humans into the partner portal, not to the API gateway.
overview: 'Discover publishes 8 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Discover API on a user''s behalf.


  Tokens are issued from https://apis.discover.com/auth/oauth/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Discover
provider_slug: discover
schemes:
- flows:
  - flow: clientCredentials
    permission_model: read, write and delete access levels granted per API resource
    scope_parameter: scope=<DISCOVER_SCOPE_NAME>
    scopes_published: false
    tokenUrl: https://apis.discover.com/auth/oauth/v2/token
  name: DiscoverApiGatewayOAuth2
  source: https://partner.discoverglobalnetwork.com/going-live-with-discover?tab=developer-guide
- audience: human sign-in to the Discover Partner Product Portal / Developer Center
  flows:
  - authorizationUrl: https://identity.discoverglobalnetwork.com/oauth2/default/v1/authorize
    flow: authorizationCode
    introspectionUrl: https://identity.discoverglobalnetwork.com/oauth2/default/v1/introspect
    issuer: https://identity.discoverglobalnetwork.com/oauth2/default
    revocationUrl: https://identity.discoverglobalnetwork.com/oauth2/default/v1/revoke
    tokenUrl: https://identity.discoverglobalnetwork.com/oauth2/default/v1/token
  name: DiscoverPartnerPortalOkta
  probed: '2026-09-06'
  source: well-known/discover-identity-default-openid-configuration.json
scope_count: 8
scope_names:
- openid
- profile
- email
- address
- phone
- offline_access
- device_sso
- interclient_access
scopes:
- description: OIDC authentication of the portal user
  flows:
  - authorizationCode
  scope: openid
- description: Portal user profile claims
  flows:
  - authorizationCode
  scope: profile
- description: Portal user email claim
  flows:
  - authorizationCode
  scope: email
- description: Portal user address claim
  flows:
  - authorizationCode
  scope: address
- description: Portal user phone claim
  flows:
  - authorizationCode
  scope: phone
- description: Refresh-token issuance for the portal session
  flows:
  - authorizationCode
  scope: offline_access
- description: Okta device single sign-on
  flows:
  - authorizationCode
  scope: device_sso
- description: Okta inter-client token exchange
  flows:
  - authorizationCode
  scope: interclient_access
slug: discover-scopes
source_filename: discover-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: https://partner.discoverglobalnetwork.com/going-live-with-discover?tab=developer-guide\ndocs: https://partner.discoverglobalnetwork.com/going-live-with-discover?tab=developer-guide\nnote: >-\n  Discover documents an OAuth 2.0 client-credentials scope model but does NOT publish a scope\n  catalogue. Section 2.1 of the developer guide states scopes are \"provided in the Discover\n  Developer Center upon review by Discover\" and the request form is literally\n  scope=DISCOVER_SCOPE_NAME - a placeholder. The concrete scope names are issued per partner, per\n  API product and per environment behind the invitation-only Developer Center login, so no scope\n  list is recorded here. The published scopes below belong to the Okta authorization server that\n  signs humans into the partner portal, not to the API gateway.\nschemes:\n- name: DiscoverApiGatewayOAuth2\n  source: https://partner.discoverglobalnetwork.com/going-live-with-discover?tab=developer-guide\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: https://apis.discover.com/auth/oauth/v2/token\n    scopes_published: false\n    scope_parameter: scope=<DISCOVER_SCOPE_NAME>\n    permission_model: 'read, write and delete access levels granted per API resource'\n- name: DiscoverPartnerPortalOkta\n  source: well-known/discover-identity-default-openid-configuration.json\n  probed: '2026-09-06'\n  audience: human sign-in to the Discover Partner Product Portal / Developer Center\n  flows:\n  - flow: authorizationCode\n    issuer: https://identity.discoverglobalnetwork.com/oauth2/default\n    authorizationUrl: https://identity.discoverglobalnetwork.com/oauth2/default/v1/authorize\n    tokenUrl: https://identity.discoverglobalnetwork.com/oauth2/default/v1/token\n    revocationUrl: https://identity.discoverglobalnetwork.com/oauth2/default/v1/revoke\n    introspectionUrl: https://identity.discoverglobalnetwork.com/oauth2/default/v1/introspect\nscopes:\n- scope: openid\n  description: OIDC\
  \ authentication of the portal user\n  flows: [authorizationCode]\n  sources: [well-known/discover-identity-default-openid-configuration.json]\n- scope: profile\n  description: Portal user profile claims\n  flows: [authorizationCode]\n  sources: [well-known/discover-identity-default-openid-configuration.json]\n- scope: email\n  description: Portal user email claim\n  flows: [authorizationCode]\n  sources: [well-known/discover-identity-default-openid-configuration.json]\n- scope: address\n  description: Portal user address claim\n  flows: [authorizationCode]\n  sources: [well-known/discover-identity-default-openid-configuration.json]\n- scope: phone\n  description: Portal user phone claim\n  flows: [authorizationCode]\n  sources: [well-known/discover-identity-default-openid-configuration.json]\n- scope: offline_access\n  description: Refresh-token issuance for the portal session\n  flows: [authorizationCode]\n  sources: [well-known/discover-identity-default-openid-configuration.json]\n\
  - scope: device_sso\n  description: Okta device single sign-on\n  flows: [authorizationCode]\n  sources: [well-known/discover-identity-default-openid-configuration.json]\n- scope: interclient_access\n  description: Okta inter-client token exchange\n  flows: [authorizationCode]\n  sources: [well-known/discover-identity-default-openid-configuration.json]\ngaps:\n- id: api-scope-catalogue-unpublished\n  detail: >-\n    No public list of the DISCOVER_SCOPE_NAME values a partner can request. A prospective\n    integrator cannot see, before signing, what authorization granularity each API product offers.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/discover/refs/heads/main/scopes/discover-scopes.yml
summary_line: 8 scopes · clientCredentials/authorizationCode
tags:
- Credit Cards
- Payments
- Card Network
- Tokenization
- Financial Services
- Fraud
- Fortune 500
token_urls:
- https://apis.discover.com/auth/oauth/v2/token
- https://identity.discoverglobalnetwork.com/oauth2/default/v1/token
---
