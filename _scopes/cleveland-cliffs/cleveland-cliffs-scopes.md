---
authorization_urls:
- https://login.clevelandcliffs.com/oauth2/v1/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Cleveland Cliffs Scopes
name_suffix: OAuth Scopes
note: Read from the anonymous discovery documents on Cleveland-Cliffs' own Okta tenant. The seven scopes below are the standard OIDC/OAuth 2.0 set the org authorization server advertises. The RFC 8414 document additionally advertises the full Okta org-management scope family (okta.users.*, okta.groups.*, okta.apps.* and ~40 more); those are the Okta product's own administrative scopes, not scopes Cleveland-Cliffs defined for a business API, so they are recorded as vendor_platform_scopes rather than as the company's scope surface. Cleveland-Cliffs publishes no public API and therefore no business-domain scope reference page.
overview: 'Cleveland-Cliffs publishes 7 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cleveland-Cliffs API on a user''s behalf.


  Tokens are issued from https://login.clevelandcliffs.com/oauth2/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cleveland-Cliffs
provider_slug: cleveland-cliffs
schemes:
- flows:
  - authorizationUrl: https://login.clevelandcliffs.com/oauth2/v1/authorize
    flow: authorizationCode
    tokenUrl: https://login.clevelandcliffs.com/oauth2/v1/token
  issuer: https://login.clevelandcliffs.com
  name: cleveland-cliffs-okta-oidc
  source: well-known/cleveland-cliffs-openid-configuration.json
scope_count: 7
scope_names:
- openid
- profile
- email
- address
- phone
- offline_access
- groups
scopes:
- description: OIDC authentication; issue an ID token for the authenticated subject.
  flows:
  - authorizationCode
  - implicit
  scope: openid
- description: Standard OIDC profile claims (name, preferred_username, locale, updated_at).
  flows:
  - authorizationCode
  - implicit
  scope: profile
- description: Email address and email_verified claim.
  flows:
  - authorizationCode
  - implicit
  scope: email
- description: Postal address claim.
  flows:
  - authorizationCode
  - implicit
  scope: address
- description: Phone number and phone_number_verified claims.
  flows:
  - authorizationCode
  - implicit
  scope: phone
- description: Issue a refresh token so the client can renew access without user presence.
  flows:
  - authorizationCode
  scope: offline_access
- description: Group membership claim for the authenticated subject.
  flows:
  - authorizationCode
  - implicit
  scope: groups
slug: cleveland-cliffs-scopes
source_filename: cleveland-cliffs-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: https://login.clevelandcliffs.com/.well-known/openid-configuration\nnote: >-\n  Read from the anonymous discovery documents on Cleveland-Cliffs' own Okta tenant. The seven\n  scopes below are the standard OIDC/OAuth 2.0 set the org authorization server advertises.\n  The RFC 8414 document additionally advertises the full Okta org-management scope family\n  (okta.users.*, okta.groups.*, okta.apps.* and ~40 more); those are the Okta product's own\n  administrative scopes, not scopes Cleveland-Cliffs defined for a business API, so they are\n  recorded as vendor_platform_scopes rather than as the company's scope surface. Cleveland-Cliffs\n  publishes no public API and therefore no business-domain scope reference page.\ndocs: null\nschemes:\n  - name: cleveland-cliffs-okta-oidc\n    source: well-known/cleveland-cliffs-openid-configuration.json\n    issuer: https://login.clevelandcliffs.com\n    flows:\n      - flow: authorizationCode\n\
  \        authorizationUrl: https://login.clevelandcliffs.com/oauth2/v1/authorize\n        tokenUrl: https://login.clevelandcliffs.com/oauth2/v1/token\nscopes:\n  - scope: openid\n    description: OIDC authentication; issue an ID token for the authenticated subject.\n    flows: [authorizationCode, implicit]\n    sources: [well-known/cleveland-cliffs-openid-configuration.json]\n  - scope: profile\n    description: Standard OIDC profile claims (name, preferred_username, locale, updated_at).\n    flows: [authorizationCode, implicit]\n    sources: [well-known/cleveland-cliffs-openid-configuration.json]\n  - scope: email\n    description: Email address and email_verified claim.\n    flows: [authorizationCode, implicit]\n    sources: [well-known/cleveland-cliffs-openid-configuration.json]\n  - scope: address\n    description: Postal address claim.\n    flows: [authorizationCode, implicit]\n    sources: [well-known/cleveland-cliffs-openid-configuration.json]\n  - scope: phone\n    description:\
  \ Phone number and phone_number_verified claims.\n    flows: [authorizationCode, implicit]\n    sources: [well-known/cleveland-cliffs-openid-configuration.json]\n  - scope: offline_access\n    description: Issue a refresh token so the client can renew access without user presence.\n    flows: [authorizationCode]\n    sources: [well-known/cleveland-cliffs-openid-configuration.json]\n  - scope: groups\n    description: Group membership claim for the authenticated subject.\n    flows: [authorizationCode, implicit]\n    sources: [well-known/cleveland-cliffs-openid-configuration.json]\nvendor_platform_scopes:\n  count: 76\n  source: well-known/cleveland-cliffs-oauth-authorization-server.json\n  note: >-\n    Okta org-management scopes (okta.*) advertised by the tenant's RFC 8414 metadata. These\n    belong to the Okta platform, not to a Cleveland-Cliffs business API, and are listed here\n    only so the discovery document is faithfully represented.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cleveland-cliffs/refs/heads/main/scopes/cleveland-cliffs-scopes.yml
summary_line: 7 scopes · authorizationCode
tags:
- Automotive
- Iron Ore
- Manufacturing
- Mining
- Steel
- Steelmaking
- Supply Chain
token_urls:
- https://login.clevelandcliffs.com/oauth2/v1/token
---
