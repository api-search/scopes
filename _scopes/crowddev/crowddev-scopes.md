---
api_specs:
- filename: crowddev-cdp-public-openapi.yml
  format: yaml
  label: CDP Public API
  slug: cdp-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-cdp-public-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Crowddev Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Crowd.dev publishes 13 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Crowd.dev API on a user''s behalf.


  Tokens are issued from https://linuxfoundation.auth0.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Crowd.dev
provider_slug: crowddev
schemes:
- description: 'Auth0 machine-to-machine client-credentials flow. Akrites exchanges its client ID/secret with Auth0 for a JWT and sends it as `Authorization: Bearer <token>`; CDP only verifies the resulting token.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://linuxfoundation.auth0.com/oauth/token
  name: M2MBearer
  source: openapi/crowddev-cdp-akrites-external-openapi.yml
- description: 'OAuth 2.0 client credentials flow via Auth0. The consuming service obtains a JWT using its client ID and secret, then passes it as `Authorization: Bearer <token>`'
  flows:
  - flow: clientCredentials
    tokenUrl: https://linuxfoundation.auth0.com/oauth/token
  name: OAuth2Bearer
  source: openapi/crowddev-cdp-public-openapi.yml
scope_count: 13
scope_names:
- read:maintainer-roles
- read:member-identities
- read:members
- read:organizations
- read:packages
- read:project-affiliations
- read:stewardships
- read:work-experiences
- write:member-identities
- write:members
- write:organizations
- write:project-affiliations
- write:work-experiences
scopes:
- description: Read security contacts (interim scope for Contacts; see the Contacts tag)
  flows:
  - clientCredentials
  scope: read:maintainer-roles
- description: Read member identities
  flows:
  - clientCredentials
  scope: read:member-identities
- description: Read member profiles
  flows:
  - clientCredentials
  scope: read:members
- description: Look up organizations
  flows:
  - clientCredentials
  scope: read:organizations
- description: Read package detail
  flows:
  - clientCredentials
  scope: read:packages
- description: Read project affiliations
  flows:
  - clientCredentials
  scope: read:project-affiliations
- description: Read package stewardship data
  flows:
  - clientCredentials
  scope: read:stewardships
- description: Read work experiences
  flows:
  - clientCredentials
  scope: read:work-experiences
- description: Create and verify member identities
  flows:
  - clientCredentials
  scope: write:member-identities
- description: Create member profiles
  flows:
  - clientCredentials
  scope: write:members
- description: Create organizations
  flows:
  - clientCredentials
  scope: write:organizations
- description: Override project affiliations
  flows:
  - clientCredentials
  scope: write:project-affiliations
- description: Create, update, verify, and delete work experiences
  flows:
  - clientCredentials
  scope: write:work-experiences
slug: crowddev-scopes
source_filename: crowddev-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/crowddev-cdp-akrites-external-openapi.yml, openapi/crowddev-cdp-public-openapi.yml\nschemes:\n- name: M2MBearer\n  source: openapi/crowddev-cdp-akrites-external-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://linuxfoundation.auth0.com/oauth/token\n  description: 'Auth0 machine-to-machine client-credentials flow. Akrites exchanges its client\n    ID/secret with Auth0 for a JWT and sends it as `Authorization: Bearer <token>`; CDP only\n    verifies the resulting token.'\n- name: OAuth2Bearer\n  source: openapi/crowddev-cdp-public-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://linuxfoundation.auth0.com/oauth/token\n  description: 'OAuth 2.0 client credentials flow via Auth0. The consuming service obtains a\n    JWT using its client ID and secret, then passes it as `Authorization: Bearer <token>`'\nscopes:\n- scope: read:maintainer-roles\n  description: Read security contacts\
  \ (interim scope for Contacts; see the Contacts tag)\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/crowddev-cdp-akrites-external-openapi.yml\n  - openapi/crowddev-cdp-public-openapi.yml\n- scope: read:member-identities\n  description: Read member identities\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/crowddev-cdp-public-openapi.yml\n- scope: read:members\n  description: Read member profiles\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/crowddev-cdp-public-openapi.yml\n- scope: read:organizations\n  description: Look up organizations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/crowddev-cdp-public-openapi.yml\n- scope: read:packages\n  description: Read package detail\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/crowddev-cdp-akrites-external-openapi.yml\n- scope: read:project-affiliations\n  description: Read project affiliations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/crowddev-cdp-public-openapi.yml\n- scope:\
  \ read:stewardships\n  description: Read package stewardship data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/crowddev-cdp-akrites-external-openapi.yml\n- scope: read:work-experiences\n  description: Read work experiences\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/crowddev-cdp-public-openapi.yml\n- scope: write:member-identities\n  description: Create and verify member identities\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/crowddev-cdp-public-openapi.yml\n- scope: write:members\n  description: Create member profiles\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/crowddev-cdp-public-openapi.yml\n- scope: write:organizations\n  description: Create organizations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/crowddev-cdp-public-openapi.yml\n- scope: write:project-affiliations\n  description: Override project affiliations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/crowddev-cdp-public-openapi.yml\n- scope: write:work-experiences\n\
  \  description: Create, update, verify, and delete work experiences\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/crowddev-cdp-public-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/scopes/crowddev-scopes.yml
summary_line: 13 scopes · clientCredentials
tags:
- Company
- Community
- Developer Relations
- Developer Data Platform
- Identity Resolution
- Open Source
- Community Data Platform
- Open Source Intelligence
token_urls:
- https://linuxfoundation.auth0.com/oauth/token
---
