---
api_specs:
- filename: crowddev-advisories-api-openapi.yml
  format: yaml
  label: Crowd.dev Advisories API
  slug: crowddev-advisories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-advisories-api-openapi.yml
- filename: crowddev-affiliations-api-openapi.yml
  format: yaml
  label: Crowd.dev Affiliations API
  slug: crowddev-affiliations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-affiliations-api-openapi.yml
- filename: crowddev-contacts-api-openapi.yml
  format: yaml
  label: Crowd.dev Contacts API
  slug: crowddev-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-contacts-api-openapi.yml
- filename: crowddev-dashboard-api-openapi.yml
  format: yaml
  label: Crowd.dev Dashboard API
  slug: crowddev-dashboard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-dashboard-api-openapi.yml
- filename: crowddev-maintainer-roles-api-openapi.yml
  format: yaml
  label: Crowd.dev Maintainer Roles API
  slug: crowddev-maintainer-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-maintainer-roles-api-openapi.yml
- filename: crowddev-member-affiliations-api-api-openapi.yml
  format: yaml
  label: Crowd.dev Member Affiliations API API
  slug: crowddev-member-affiliations-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-member-affiliations-api-api-openapi.yml
- filename: crowddev-member-identities-api-openapi.yml
  format: yaml
  label: Crowd.dev Member Identities API
  slug: crowddev-member-identities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-member-identities-api-openapi.yml
- filename: crowddev-member-organizations-api-api-openapi.yml
  format: yaml
  label: Crowd.dev Member Organizations API API
  slug: crowddev-member-organizations-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-member-organizations-api-api-openapi.yml
- filename: crowddev-members-api-openapi.yml
  format: yaml
  label: Crowd.dev Members API
  slug: crowddev-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-members-api-openapi.yml
- filename: crowddev-organizations-api-openapi.yml
  format: yaml
  label: Crowd.dev Organizations API
  slug: crowddev-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-organizations-api-openapi.yml
- filename: crowddev-packages-api-openapi.yml
  format: yaml
  label: Crowd.dev Packages API
  slug: crowddev-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-packages-api-openapi.yml
- filename: crowddev-project-affiliations-api-openapi.yml
  format: yaml
  label: Crowd.dev Project Affiliations API
  slug: crowddev-project-affiliations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-project-affiliations-api-openapi.yml
- filename: crowddev-stewardship-actions-api-openapi.yml
  format: yaml
  label: Crowd.dev Stewardship Actions API
  slug: crowddev-stewardship-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-stewardship-actions-api-openapi.yml
- filename: crowddev-stewardship-api-openapi.yml
  format: yaml
  label: Crowd.dev Stewardship API
  slug: crowddev-stewardship-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-stewardship-api-openapi.yml
- filename: crowddev-stewardships-api-openapi.yml
  format: yaml
  label: Crowd.dev Stewardships API
  slug: crowddev-stewardships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-stewardships-api-openapi.yml
- filename: crowddev-work-experiences-api-openapi.yml
  format: yaml
  label: Crowd.dev Work Experiences API
  slug: crowddev-work-experiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-work-experiences-api-openapi.yml
authorization_urls: []
description: ''
docs: https://github.com/linuxfoundation/crowd.dev/blob/main/docs/adr/0016-akrites-cdp-public-api-authentication.md
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Crowddev Scopes
name_suffix: OAuth Scopes
note: 'Upgraded from derived to searched on 2026-08-14. ADR-0016 documents a scope migration the OpenAPI does not yet reflect: three Akrites-namespaced scopes are now defined on the `cdp_public_api` Auth0 API and granted only to the `Akrites Enclave` client, while each /akrites-external subrouter transitionally accepts EITHER the namespaced scope OR its legacy Self Serve equivalent via `requireScopes([...], ''any'')`. The legacy fallbacks are removed once Akrites confirms end-to-end token exchange. The specs in openapi/ still declare only the legacy names, so both sets are recorded below with their status.'
overview: 'Crowd.dev publishes 17 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Crowd.dev API on a user''s behalf.


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
scope_count: 17
scope_names:
- read:akrites-packages
- read:akrites-advisories
- read:akrites-maintainers
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
- write:stewardships
scopes:
- description: Read package detail on the /akrites-external route (Akrites-namespaced target scope)
  flows:
  - clientCredentials
  scope: read:akrites-packages
- description: Read package security advisories on the /akrites-external route (Akrites-namespaced target scope)
  flows:
  - clientCredentials
  scope: read:akrites-advisories
- description: Read package security contacts on the /akrites-external route (Akrites-namespaced target scope)
  flows:
  - clientCredentials
  scope: read:akrites-maintainers
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
- description: Open, assign, escalate and update OSSPREY Program admin stewardship actions
  flows:
  - clientCredentials
  scope: write:stewardships
slug: crowddev-scopes
source_filename: crowddev-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: https://github.com/linuxfoundation/crowd.dev/blob/main/docs/adr/0016-akrites-cdp-public-api-authentication.md\ndocs: https://github.com/linuxfoundation/crowd.dev/blob/main/docs/adr/0016-akrites-cdp-public-api-authentication.md\nderived_from: openapi/crowddev-cdp-akrites-external-openapi.yml, openapi/crowddev-cdp-public-openapi.yml\nnote: >-\n  Upgraded from derived to searched on 2026-08-14. ADR-0016 documents a scope migration the\n  OpenAPI does not yet reflect: three Akrites-namespaced scopes are now defined on the\n  `cdp_public_api` Auth0 API and granted only to the `Akrites Enclave` client, while each\n  /akrites-external subrouter transitionally accepts EITHER the namespaced scope OR its legacy\n  Self Serve equivalent via `requireScopes([...], 'any')`. The legacy fallbacks are removed once\n  Akrites confirms end-to-end token exchange. The specs in openapi/ still declare only the legacy\n  names, so both sets are recorded\
  \ below with their status.\nauth0_api: cdp_public_api\nschemes:\n- name: M2MBearer\n  source: openapi/crowddev-cdp-akrites-external-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://linuxfoundation.auth0.com/oauth/token\n  description: 'Auth0 machine-to-machine client-credentials flow. Akrites exchanges its client\n    ID/secret with Auth0 for a JWT and sends it as `Authorization: Bearer <token>`; CDP only\n    verifies the resulting token.'\n- name: OAuth2Bearer\n  source: openapi/crowddev-cdp-public-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://linuxfoundation.auth0.com/oauth/token\n  description: 'OAuth 2.0 client credentials flow via Auth0. The consuming service obtains a\n    JWT using its client ID and secret, then passes it as `Authorization: Bearer <token>`'\nscopes:\n- scope: read:akrites-packages\n  description: Read package detail on the /akrites-external route (Akrites-namespaced target scope)\n  flows:\n  - clientCredentials\n\
  \  status: target\n  granted_to: Akrites Enclave\n  sources:\n  - https://github.com/linuxfoundation/crowd.dev/blob/main/docs/adr/0016-akrites-cdp-public-api-authentication.md\n  note: >-\n    Defined on cdp_public_api and granted only to the Akrites Enclave client. Not yet declared in\n    openapi/crowddev-cdp-akrites-external-openapi.yml, which still lists the legacy read:packages.\n- scope: read:akrites-advisories\n  description: Read package security advisories on the /akrites-external route (Akrites-namespaced target scope)\n  flows:\n  - clientCredentials\n  status: target\n  granted_to: Akrites Enclave\n  sources:\n  - https://github.com/linuxfoundation/crowd.dev/blob/main/docs/adr/0016-akrites-cdp-public-api-authentication.md\n  note: >-\n    The akrites-external spec still notes the final name was undecided (read:advisories vs\n    cdp:advisories:read); ADR-0016 settles it as read:akrites-advisories.\n- scope: read:akrites-maintainers\n  description: Read package security contacts\
  \ on the /akrites-external route (Akrites-namespaced target scope)\n  flows:\n  - clientCredentials\n  status: target\n  granted_to: Akrites Enclave\n  sources:\n  - https://github.com/linuxfoundation/crowd.dev/blob/main/docs/adr/0016-akrites-cdp-public-api-authentication.md\n  note: >-\n    Gates security-contact PII. Legacy fallback during cut-over is read:maintainer-roles, never\n    read:packages.\n- scope: read:maintainer-roles\n  status: legacy\n  description: Read security contacts (interim scope for Contacts; see the Contacts tag)\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/crowddev-cdp-akrites-external-openapi.yml\n  - openapi/crowddev-cdp-public-openapi.yml\n- scope: read:member-identities\n  description: Read member identities\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/crowddev-cdp-public-openapi.yml\n- scope: read:members\n  description: Read member profiles\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/crowddev-cdp-public-openapi.yml\n\
  - scope: read:organizations\n  description: Look up organizations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/crowddev-cdp-public-openapi.yml\n- scope: read:packages\n  description: Read package detail\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/crowddev-cdp-akrites-external-openapi.yml\n- scope: read:project-affiliations\n  description: Read project affiliations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/crowddev-cdp-public-openapi.yml\n- scope: read:stewardships\n  description: Read package stewardship data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/crowddev-cdp-akrites-external-openapi.yml\n- scope: read:work-experiences\n  description: Read work experiences\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/crowddev-cdp-public-openapi.yml\n- scope: write:member-identities\n  description: Create and verify member identities\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/crowddev-cdp-public-openapi.yml\n- scope:\
  \ write:members\n  description: Create member profiles\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/crowddev-cdp-public-openapi.yml\n- scope: write:organizations\n  description: Create organizations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/crowddev-cdp-public-openapi.yml\n- scope: write:project-affiliations\n  description: Override project affiliations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/crowddev-cdp-public-openapi.yml\n- scope: write:work-experiences\n  description: Create, update, verify, and delete work experiences\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/crowddev-cdp-public-openapi.yml\n- scope: write:stewardships\n  description: Open, assign, escalate and update OSSPREY Program admin stewardship actions\n  flows:\n  - clientCredentials\n  status: declared-not-enforced\n  sources:\n  - openapi/crowddev-cdp-stewardships-openapi.yml\n  note: >-\n    Declared as required on all four stewardship write operations, but\
  \ the spec's own V1 note says\n    the scope \"is not yet added to the Auth0 staging tenant - scope enforcement is temporarily\n    disabled. See CM-1235.\" Recorded as declared, not as enforced.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/scopes/crowddev-scopes.yml
summary_line: 17 scopes · clientCredentials
tags:
- Company
- Community
- Developer Relations
- Developer Data Platform
- Identity Resolution
- Open-Source
- Community Data Platform
- Open Source Intelligence
token_urls:
- https://linuxfoundation.auth0.com/oauth/token
---
