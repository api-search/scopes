---
api_specs:
- filename: keller-williams-listings-search-openapi.json
  format: json
  label: KW Worldwide Listings Search API
  slug: keller-williams-worldwide-listings-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keller-williams/refs/heads/main/openapi/keller-williams-listings-search-openapi.json
authorization_urls:
- https://partners.api.kw.com/idp/authorize
description: ''
docs: https://developer.kw.com/getting-started
flows:
- authorizationCode
- implicit
- clientCredentials
- tokenExchange
- jwtBearer
kind: oauth-scopes
layout: scope
method: searched
name: Keller Williams Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Keller Williams publishes 40 OAuth 2.0 scopes via the authorizationCode, implicit, clientCredentials, tokenExchange, and jwtBearer flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Keller Williams API on a user''s behalf.


  Tokens are issued from https://partners.api.kw.com/idp/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Keller Williams
provider_slug: keller-williams
schemes:
- device_authorization_endpoint: https://partners.api.kw.com/idp/device_authorization
  discovery: https://partners.api.kw.com/idp/.well-known/openid-configuration
  end_session_endpoint: https://partners.api.kw.com/idp/end_session
  flows:
  - authorizationUrl: https://partners.api.kw.com/idp/authorize
    flow: authorizationCode
    pkce: S256
    refreshUrl: https://partners.api.kw.com/idp/token
    tokenUrl: https://partners.api.kw.com/idp/token
  - authorizationUrl: https://partners.api.kw.com/idp/authorize
    flow: implicit
  - flow: clientCredentials
    tokenUrl: https://partners.api.kw.com/idp/token
  - flow: tokenExchange
    grant_type: urn:ietf:params:oauth:grant-type:token-exchange
    tokenUrl: https://partners.api.kw.com/idp/token
  - flow: jwtBearer
    grant_type: urn:ietf:params:oauth:grant-type:jwt-bearer
    tokenUrl: https://partners.api.kw.com/idp/token
  introspection_endpoint: https://partners.api.kw.com/idp/introspect
  issuer: https://partners.api.kw.com
  name: OpenIDConnect
  revocation_endpoint: https://partners.api.kw.com/idp/revoke
  type: openIdConnect
  userinfo_endpoint: https://partners.api.kw.com/idp/userinfo
scope_count: 40
scope_names:
- openid
- profile
- email
- offline_access
- read_contact
- write_contact
- read_contact_setting
- write_custom_field
- read_organization
- read_task
- write_task
- listings_get
- listings_post
- listings_details_patch
- listings_details_delete
- listings_lookup_table_get
- listings_region_details_get
- listings_orgs_people_get
- listings_people_orgs_get
- read_all_listings
- read_all_listings_cors
- read_all_listings_zendesk
- read_user_listings
- read_syndicated_listings
- delete_task
- read_all_task_productive
- write_all_task_productive
- read_all_contact_productive
- write_all_contact_productive
- read_all_user
- read_all_users_lw
- read_all_associates
- read_all_organization
- read_opportunity
- read_recruit
- write_recruit
- read_agent_marketing_profile
- read_user_marketing_profile
- read_all_orgs_marketing_profile
- webrand
scopes:
- description: Required on every /authorize request; enables the OpenID Connect identity layer.
  flows: []
  scope: openid
- description: Required default scope; basic profile claims (name, family_name, given_name, locale, preferred_username).
  flows: []
  scope: profile
- description: Email and email_verified claims.
  flows: []
  scope: email
- description: Issues a refresh token (365-day lifetime) alongside the access token.
  flows: []
  scope: offline_access
- description: Read Contact Data.
  flows: []
  scope: read_contact
- description: Create or Update Contact Data.
  flows: []
  scope: write_contact
- description: Read Command Contact Settings.
  flows: []
  scope: read_contact_setting
- description: Create Contact Custom Fields.
  flows: []
  scope: write_custom_field
- description: Read KW Organizational Information.
  flows: []
  scope: read_organization
- description: Read Task Information.
  flows: []
  scope: read_task
- description: Create or Edit Tasks.
  flows: []
  scope: write_task
- description: ''
  flows: []
  scope: listings_get
- description: ''
  flows: []
  scope: listings_post
- description: ''
  flows: []
  scope: listings_details_patch
- description: ''
  flows: []
  scope: listings_details_delete
- description: ''
  flows: []
  scope: listings_lookup_table_get
- description: ''
  flows: []
  scope: listings_region_details_get
- description: ''
  flows: []
  scope: listings_orgs_people_get
- description: ''
  flows: []
  scope: listings_people_orgs_get
- description: ''
  flows: []
  scope: read_all_listings
- description: ''
  flows: []
  scope: read_all_listings_cors
- description: ''
  flows: []
  scope: read_all_listings_zendesk
- description: ''
  flows: []
  scope: read_user_listings
- description: ''
  flows: []
  scope: read_syndicated_listings
- description: ''
  flows: []
  scope: delete_task
- description: ''
  flows: []
  scope: read_all_task_productive
- description: ''
  flows: []
  scope: write_all_task_productive
- description: ''
  flows: []
  scope: read_all_contact_productive
- description: ''
  flows: []
  scope: write_all_contact_productive
- description: ''
  flows: []
  scope: read_all_user
- description: ''
  flows: []
  scope: read_all_users_lw
- description: ''
  flows: []
  scope: read_all_associates
- description: ''
  flows: []
  scope: read_all_organization
- description: ''
  flows: []
  scope: read_opportunity
- description: ''
  flows: []
  scope: read_recruit
- description: ''
  flows: []
  scope: write_recruit
- description: ''
  flows: []
  scope: read_agent_marketing_profile
- description: ''
  flows: []
  scope: read_user_marketing_profile
- description: ''
  flows: []
  scope: read_all_orgs_marketing_profile
- description: ''
  flows: []
  scope: webrand
slug: keller-williams-scopes
source_filename: keller-williams-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: https://partners.api.kw.com/idp/.well-known/openid-configuration\ndocs: https://developer.kw.com/getting-started\nlocal_source: authentication/keller-williams-openid-configuration.json\nsummary:\n  scopes_total: 40\n  advertised_by_discovery: 40\n  documented_in_portal: 8\n  documented_but_not_advertised: 1\n  oidc_standard: 4\n  note: >-\n    Keller Williams advertises 40 OAuth 2.0 / OpenID Connect scopes in its\n    public discovery document, but the DevHub \"Getting Started\" guide only\n    describes 8 of them as selectable products at application-creation\n    time. The remaining 32 exist on the authorization server and are\n    granted by KWRI on a per-partnership basis; there is no published\n    scope reference page enumerating them. One scope named in the docs\n    (`read_user`) is NOT advertised by the discovery document, which\n    instead exposes `read_all_user` and `read_all_users_lw` — a real\n    docs/server\
  \ divergence, recorded rather than reconciled.\n    Scope selection happens in the DevHub app-creation UI, and the chosen\n    scopes are what the end user sees on the Command consent screen.\n    `openid` and `profile` are required defaults on every /authorize call.\nschemes:\n  - name: OpenIDConnect\n    type: openIdConnect\n    issuer: https://partners.api.kw.com\n    discovery: https://partners.api.kw.com/idp/.well-known/openid-configuration\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://partners.api.kw.com/idp/authorize\n        tokenUrl: https://partners.api.kw.com/idp/token\n        refreshUrl: https://partners.api.kw.com/idp/token\n        pkce: S256\n      - flow: implicit\n        authorizationUrl: https://partners.api.kw.com/idp/authorize\n      - flow: clientCredentials\n        tokenUrl: https://partners.api.kw.com/idp/token\n      - flow: tokenExchange\n        tokenUrl: https://partners.api.kw.com/idp/token\n        grant_type: urn:ietf:params:oauth:grant-type:token-exchange\n\
  \      - flow: jwtBearer\n        tokenUrl: https://partners.api.kw.com/idp/token\n        grant_type: urn:ietf:params:oauth:grant-type:jwt-bearer\n    revocation_endpoint: https://partners.api.kw.com/idp/revoke\n    introspection_endpoint: https://partners.api.kw.com/idp/introspect\n    userinfo_endpoint: https://partners.api.kw.com/idp/userinfo\n    end_session_endpoint: https://partners.api.kw.com/idp/end_session\n    device_authorization_endpoint: https://partners.api.kw.com/idp/device_authorization\nscopes:\n  # --- OIDC standard scopes -------------------------------------------\n  - scope: openid\n    description: Required on every /authorize request; enables the OpenID Connect identity layer.\n    family: oidc\n    documented: true\n    required: true\n  - scope: profile\n    description: Required default scope; basic profile claims (name, family_name, given_name, locale, preferred_username).\n    family: oidc\n    documented: true\n    required: true\n  - scope: email\n    description:\
  \ Email and email_verified claims.\n    family: oidc\n    documented: false\n  - scope: offline_access\n    description: Issues a refresh token (365-day lifetime) alongside the access token.\n    family: oidc\n    documented: false\n  # --- Documented DevHub products -------------------------------------\n  - scope: read_contact\n    description: Read Contact Data.\n    family: contacts\n    documented: true\n    product: Read Contact Data\n  - scope: write_contact\n    description: Create or Update Contact Data.\n    family: contacts\n    documented: true\n    product: Create or Update Contact Data\n  - scope: read_contact_setting\n    description: Read Command Contact Settings.\n    family: contacts\n    documented: true\n    product: Read Command Contact Settings\n  - scope: write_custom_field\n    description: Create Contact Custom Fields.\n    family: contacts\n    documented: true\n    product: Create Contact Custom Fields\n  - scope: read_organization\n    description: Read KW Organizational\
  \ Information.\n    family: organizations\n    documented: true\n    product: Read KW Organizational Information\n  - scope: read_task\n    description: Read Task Information.\n    family: tasks\n    documented: true\n    product: Read Task Information\n  - scope: write_task\n    description: Create or Edit Tasks.\n    family: tasks\n    documented: true\n    product: Create or Edit Tasks\n  # --- Listings scopes (bindable to the published OpenAPI) -------------\n  - scope: listings_get\n    family: listings\n    documented: false\n    binds_to: openapi/keller-williams-listings-search-openapi.json#listings-read\n  - scope: listings_post\n    family: listings\n    documented: false\n    binds_to: openapi/keller-williams-listings-search-openapi.json#listings-create\n  - scope: listings_details_patch\n    family: listings\n    documented: false\n    binds_to: openapi/keller-williams-listings-search-openapi.json#listings-details-update\n  - scope: listings_details_delete\n    family: listings\n\
  \    documented: false\n    binds_to: openapi/keller-williams-listings-search-openapi.json#listings-details-delete\n  - scope: listings_lookup_table_get\n    family: listings\n    documented: false\n    binds_to: openapi/keller-williams-listings-search-openapi.json#listings-read-by-table\n  - scope: listings_region_details_get\n    family: listings\n    documented: false\n    binds_to: openapi/keller-williams-listings-search-openapi.json#listings-region-details-read\n  - scope: listings_orgs_people_get\n    family: listings\n    documented: false\n    binds_to: openapi/keller-williams-listings-search-openapi.json#listings-region-people-read\n  - scope: listings_people_orgs_get\n    family: listings\n    documented: false\n    note: No corresponding operation in the published Listings OpenAPI; the inverse people-to-orgs lookup is behind the login-gated catalog.\n  - scope: read_all_listings\n    family: listings\n    documented: false\n  - scope: read_all_listings_cors\n    family: listings\n\
  \    documented: false\n    note: Browser/CORS-flavoured variant of read_all_listings.\n  - scope: read_all_listings_zendesk\n    family: listings\n    documented: false\n    note: Zendesk-integration variant of read_all_listings.\n  - scope: read_user_listings\n    family: listings\n    documented: false\n  - scope: read_syndicated_listings\n    family: listings\n    documented: false\n  # --- Remaining server-advertised scopes -----------------------------\n  - scope: delete_task\n    family: tasks\n    documented: false\n  - scope: read_all_task_productive\n    family: tasks\n    documented: false\n  - scope: write_all_task_productive\n    family: tasks\n    documented: false\n  - scope: read_all_contact_productive\n    family: contacts\n    documented: false\n  - scope: write_all_contact_productive\n    family: contacts\n    documented: false\n  - scope: read_all_user\n    family: users\n    documented: false\n  - scope: read_all_users_lw\n    family: users\n    documented: false\n\
  \    note: >-\n      The \"lw\" variant, presumed Livian / LW line of business.\n  - scope: read_all_associates\n    family: users\n    documented: false\n  - scope: read_all_organization\n    family: organizations\n    documented: false\n  - scope: read_opportunity\n    family: opportunities\n    documented: false\n  - scope: read_recruit\n    family: recruiting\n    documented: false\n  - scope: write_recruit\n    family: recruiting\n    documented: false\n  - scope: read_agent_marketing_profile\n    family: marketing\n    documented: false\n  - scope: read_user_marketing_profile\n    family: marketing\n    documented: false\n  - scope: read_all_orgs_marketing_profile\n    family: marketing\n    documented: false\n  - scope: webrand\n    family: marketing\n    documented: false\n    note: Undocumented; name suggests the KW web-branding/agent-site surface.\ndocumented_but_not_advertised:\n  - scope: read_user\n    description: \"Read KW User Information — named in the DevHub Getting Started\
  \ product list, but absent from the discovery document's scopes_supported.\"\n    docs: https://developer.kw.com/getting-started\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keller-williams/refs/heads/main/scopes/keller-williams-scopes.yml
summary_line: 40 scopes · authorizationCode/implicit/clientCredentials/tokenExchange/jwtBearer
tags:
- Real-Estate
- United States
- Residential Real Estate
- Brokerage
- Franchise
- Property Listings
- PropTech
- Agent Platform
- CRM
- Partner APIs
- Marketplace
- Austin Texas
token_urls:
- https://partners.api.kw.com/idp/token
---
