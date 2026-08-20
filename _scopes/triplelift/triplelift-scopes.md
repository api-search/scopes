---
authorization_urls: []
description: 'TripleLift publishes no scopes reference page. This catalog was read off two live, anonymous, unauthenticated responses: the Auth0 authorize redirect emitted by https://app.triplelift.com/ (which carries the platform''s full requested scope set in its Location query string), and the two OAuth metadata documents served on auth.triplelift.net and triplelift.com. Every scope string below appears verbatim in one of those responses. Descriptions are DERIVED from the scope naming convention (<service>:<resource>.<action>) and are labelled as such — TripleLift documents none of them.'
docs: none published
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Triplelift Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'TripleLift publishes 51 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the TripleLift API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: TripleLift
provider_slug: triplelift
schemes: []
scope_count: 51
scope_names:
- openid
- profile
- email
- offline_access
- members.read
- users
- users.read
- member_read
- legacy-tool-access
- read_client_secret
- avails_read
- read:segments
- read:publisher_segments
- block:publisher_segments
- unblock:publisher_segments
- read:segment_blockers
- add:segment_blockers
- remove:segment_blockers
- read:domains
- create:domains
- sitelists
- sitelists.read
- sitelists.read.all
- deals-api:graphql.read
- deals-api:deal.*
- buyer-api:buyers.read
- buyer-api:seats.read
- buyer-api:members.read
- creative-service-api:graphql.read
- creative-service-api:campaign.manage
- user-mgmt-api:members.read
- user-mgmt-api:*.*
- reporting-api:report.*
- advertiser-connect:advertiser.read
- advertiser-connect:advertiser.update
- advertiser-connect:segment.read
- advertiser-connect:connect-request.*
- advertiser-connect:data-connection.read
- margin-management-api:deal_fee.read
- margin-management-api:fee.create
- margin-management-api:fee.update
- margin-management-api:fee.delete
- margin-management-api:fee_model_value.read
- margin-management-api:fee_model_value.create
- margin-management-api:fee_model_value.update
- margin-management-api:fee_model_value.delete
- tlsuite:access
- tlsuite:segments_reporting
- tlsuite:onboarded_data
- tlsuite:custom_segments
- mcp
scopes:
- description: Standard OpenID Connect scope; requests an ID token.
  flows: []
  scope: openid
- description: Standard OIDC profile claims.
  flows: []
  scope: profile
- description: Standard OIDC email claim.
  flows: []
  scope: email
- description: Standard OIDC scope requesting a refresh token.
  flows: []
  scope: offline_access
- description: 'DERIVED: read TripleLift member (account) records.'
  flows: []
  scope: members.read
- description: 'DERIVED: user administration.'
  flows: []
  scope: users
- description: 'DERIVED: read user records.'
  flows: []
  scope: users.read
- description: 'DERIVED: legacy member read scope, coexisting with members.read.'
  flows: []
  scope: member_read
- description: 'DERIVED: access to superseded TripleLift tooling retained for compatibility.'
  flows: []
  scope: legacy-tool-access
- description: 'DERIVED: read an application client secret.'
  flows: []
  scope: read_client_secret
- description: 'DERIVED: read inventory availability (avails) forecasts.'
  flows: []
  scope: avails_read
- description: 'DERIVED: read audience segments.'
  flows: []
  scope: read:segments
- description: 'DERIVED: read publisher-owned segments.'
  flows: []
  scope: read:publisher_segments
- description: 'DERIVED: block a publisher segment.'
  flows: []
  scope: block:publisher_segments
- description: 'DERIVED: unblock a publisher segment.'
  flows: []
  scope: unblock:publisher_segments
- description: 'DERIVED: read segment blocking rules.'
  flows: []
  scope: read:segment_blockers
- description: 'DERIVED: create segment blocking rules.'
  flows: []
  scope: add:segment_blockers
- description: 'DERIVED: delete segment blocking rules.'
  flows: []
  scope: remove:segment_blockers
- description: 'DERIVED: read domain records.'
  flows: []
  scope: read:domains
- description: 'DERIVED: create domain records.'
  flows: []
  scope: create:domains
- description: 'DERIVED: full access to site lists (inventory allow/block lists).'
  flows: []
  scope: sitelists
- description: 'DERIVED: read the caller''s site lists.'
  flows: []
  scope: sitelists.read
- description: 'DERIVED: read all site lists, not only the caller''s.'
  flows: []
  scope: sitelists.read.all
- description: 'DERIVED: read access to the deals GraphQL subgraph.'
  flows: []
  scope: deals-api:graphql.read
- description: 'DERIVED: full CRUD on deals (PMP/programmatic guaranteed).'
  flows: []
  scope: deals-api:deal.*
- description: 'DERIVED: read buyer records.'
  flows: []
  scope: buyer-api:buyers.read
- description: 'DERIVED: read DSP seat records.'
  flows: []
  scope: buyer-api:seats.read
- description: 'DERIVED: read buyer-side member records.'
  flows: []
  scope: buyer-api:members.read
- description: 'DERIVED: read access to the creative GraphQL subgraph.'
  flows: []
  scope: creative-service-api:graphql.read
- description: 'DERIVED: create and manage creative campaigns.'
  flows: []
  scope: creative-service-api:campaign.manage
- description: 'DERIVED: read members through the user-management service.'
  flows: []
  scope: user-mgmt-api:members.read
- description: 'DERIVED: wildcard — every resource and every action on the user-management service.'
  flows: []
  scope: user-mgmt-api:*.*
- description: 'DERIVED: full access to reports. This is the platform-token equivalent of the X-API-Key + JWT pair used on reporting-api.triplelift.net.'
  flows: []
  scope: reporting-api:report.*
- description: 'DERIVED: read advertiser records.'
  flows: []
  scope: advertiser-connect:advertiser.read
- description: 'DERIVED: update advertiser records.'
  flows: []
  scope: advertiser-connect:advertiser.update
- description: 'DERIVED: read advertiser-connect segments.'
  flows: []
  scope: advertiser-connect:segment.read
- description: 'DERIVED: full CRUD on data-connection requests.'
  flows: []
  scope: advertiser-connect:connect-request.*
- description: 'DERIVED: read established data connections.'
  flows: []
  scope: advertiser-connect:data-connection.read
- description: 'DERIVED: read per-deal fees.'
  flows: []
  scope: margin-management-api:deal_fee.read
- description: 'DERIVED: create fees.'
  flows: []
  scope: margin-management-api:fee.create
- description: 'DERIVED: update fees.'
  flows: []
  scope: margin-management-api:fee.update
- description: 'DERIVED: delete fees.'
  flows: []
  scope: margin-management-api:fee.delete
- description: 'DERIVED: read fee-model values.'
  flows: []
  scope: margin-management-api:fee_model_value.read
- description: 'DERIVED: create fee-model values.'
  flows: []
  scope: margin-management-api:fee_model_value.create
- description: 'DERIVED: update fee-model values.'
  flows: []
  scope: margin-management-api:fee_model_value.update
- description: 'DERIVED: delete fee-model values.'
  flows: []
  scope: margin-management-api:fee_model_value.delete
- description: 'DERIVED: baseline access to TripleLift Suite.'
  flows: []
  scope: tlsuite:access
- description: 'DERIVED: segment reporting in TripleLift Suite.'
  flows: []
  scope: tlsuite:segments_reporting
- description: 'DERIVED: access onboarded first-party data.'
  flows: []
  scope: tlsuite:onboarded_data
- description: 'DERIVED: manage custom segments.'
  flows: []
  scope: tlsuite:custom_segments
- description: Access the MCP server on the triplelift.com WordPress site. Published in that host's own authorization-server metadata.
  flows: []
  scope: mcp
slug: triplelift-scopes
source_filename: triplelift-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "name: TripleLift OAuth Scopes\ndescription: >-\n  TripleLift publishes no scopes reference page. This catalog was read off two\n  live, anonymous, unauthenticated responses: the Auth0 authorize redirect emitted\n  by https://app.triplelift.com/ (which carries the platform's full requested scope\n  set in its Location query string), and the two OAuth metadata documents served on\n  auth.triplelift.net and triplelift.com. Every scope string below appears verbatim\n  in one of those responses. Descriptions are DERIVED from the scope naming\n  convention (<service>:<resource>.<action>) and are labelled as such — TripleLift\n  documents none of them.\ngenerated: '2026-08-12'\nmethod: probed\nsource: https://app.triplelift.com/ (302 Location -> https://auth.triplelift.net/authorize?...&scope=...)\ndocs: none published\nauthorization_servers:\n  - issuer: https://auth.triplelift.net/\n    audience: https://federated-api.prod.triplelift.net\n    metadata: https://auth.triplelift.net/.well-known/openid-configuration\n\
  \    provider: Auth0\n    standard_scopes_supported:\n      - openid\n      - profile\n      - offline_access\n      - name\n      - given_name\n      - family_name\n      - nickname\n      - email\n      - email_verified\n      - picture\n      - created_at\n      - identities\n      - phone\n      - address\n  - issuer: https://triplelift.com\n    metadata: https://triplelift.com/.well-known/oauth-authorization-server\n    resource: https://triplelift.com/wp-json/mcp/mcp-oauth-server\n    scopes_supported:\n      - mcp\nscopes:\n  - scope: openid\n    service: auth0\n    description: Standard OpenID Connect scope; requests an ID token.\n    method: probed\n  - scope: profile\n    service: auth0\n    description: Standard OIDC profile claims.\n    method: probed\n  - scope: email\n    service: auth0\n    description: Standard OIDC email claim.\n    method: probed\n  - scope: offline_access\n    service: auth0\n    description: Standard OIDC scope requesting a refresh token.\n    method:\
  \ probed\n  - scope: members.read\n    service: platform\n    description: 'DERIVED: read TripleLift member (account) records.'\n  - scope: users\n    service: platform\n    description: 'DERIVED: user administration.'\n  - scope: users.read\n    service: platform\n    description: 'DERIVED: read user records.'\n  - scope: member_read\n    service: platform\n    description: 'DERIVED: legacy member read scope, coexisting with members.read.'\n  - scope: legacy-tool-access\n    service: platform\n    description: 'DERIVED: access to superseded TripleLift tooling retained for compatibility.'\n  - scope: read_client_secret\n    service: platform\n    description: 'DERIVED: read an application client secret.'\n  - scope: avails_read\n    service: platform\n    description: 'DERIVED: read inventory availability (avails) forecasts.'\n  - scope: 'read:segments'\n    service: segments\n    description: 'DERIVED: read audience segments.'\n  - scope: 'read:publisher_segments'\n    service: segments\n\
  \    description: 'DERIVED: read publisher-owned segments.'\n  - scope: 'block:publisher_segments'\n    service: segments\n    description: 'DERIVED: block a publisher segment.'\n  - scope: 'unblock:publisher_segments'\n    service: segments\n    description: 'DERIVED: unblock a publisher segment.'\n  - scope: 'read:segment_blockers'\n    service: segments\n    description: 'DERIVED: read segment blocking rules.'\n  - scope: 'add:segment_blockers'\n    service: segments\n    description: 'DERIVED: create segment blocking rules.'\n  - scope: 'remove:segment_blockers'\n    service: segments\n    description: 'DERIVED: delete segment blocking rules.'\n  - scope: 'read:domains'\n    service: domains\n    description: 'DERIVED: read domain records.'\n  - scope: 'create:domains'\n    service: domains\n    description: 'DERIVED: create domain records.'\n  - scope: sitelists\n    service: sitelists\n    description: 'DERIVED: full access to site lists (inventory allow/block lists).'\n  - scope:\
  \ sitelists.read\n    service: sitelists\n    description: 'DERIVED: read the caller''s site lists.'\n  - scope: sitelists.read.all\n    service: sitelists\n    description: 'DERIVED: read all site lists, not only the caller''s.'\n  - scope: 'deals-api:graphql.read'\n    service: deals-api\n    description: 'DERIVED: read access to the deals GraphQL subgraph.'\n  - scope: 'deals-api:deal.*'\n    service: deals-api\n    description: 'DERIVED: full CRUD on deals (PMP/programmatic guaranteed).'\n  - scope: 'buyer-api:buyers.read'\n    service: buyer-api\n    description: 'DERIVED: read buyer records.'\n  - scope: 'buyer-api:seats.read'\n    service: buyer-api\n    description: 'DERIVED: read DSP seat records.'\n  - scope: 'buyer-api:members.read'\n    service: buyer-api\n    description: 'DERIVED: read buyer-side member records.'\n  - scope: 'creative-service-api:graphql.read'\n    service: creative-service-api\n    description: 'DERIVED: read access to the creative GraphQL subgraph.'\n \
  \ - scope: 'creative-service-api:campaign.manage'\n    service: creative-service-api\n    description: 'DERIVED: create and manage creative campaigns.'\n  - scope: 'user-mgmt-api:members.read'\n    service: user-mgmt-api\n    description: 'DERIVED: read members through the user-management service.'\n  - scope: 'user-mgmt-api:*.*'\n    service: user-mgmt-api\n    description: 'DERIVED: wildcard — every resource and every action on the user-management service.'\n  - scope: 'reporting-api:report.*'\n    service: reporting-api\n    description: 'DERIVED: full access to reports. This is the platform-token equivalent of the X-API-Key + JWT pair used on reporting-api.triplelift.net.'\n  - scope: 'advertiser-connect:advertiser.read'\n    service: advertiser-connect\n    description: 'DERIVED: read advertiser records.'\n  - scope: 'advertiser-connect:advertiser.update'\n    service: advertiser-connect\n    description: 'DERIVED: update advertiser records.'\n  - scope: 'advertiser-connect:segment.read'\n\
  \    service: advertiser-connect\n    description: 'DERIVED: read advertiser-connect segments.'\n  - scope: 'advertiser-connect:connect-request.*'\n    service: advertiser-connect\n    description: 'DERIVED: full CRUD on data-connection requests.'\n  - scope: 'advertiser-connect:data-connection.read'\n    service: advertiser-connect\n    description: 'DERIVED: read established data connections.'\n  - scope: 'margin-management-api:deal_fee.read'\n    service: margin-management-api\n    description: 'DERIVED: read per-deal fees.'\n  - scope: 'margin-management-api:fee.create'\n    service: margin-management-api\n    description: 'DERIVED: create fees.'\n  - scope: 'margin-management-api:fee.update'\n    service: margin-management-api\n    description: 'DERIVED: update fees.'\n  - scope: 'margin-management-api:fee.delete'\n    service: margin-management-api\n    description: 'DERIVED: delete fees.'\n  - scope: 'margin-management-api:fee_model_value.read'\n    service: margin-management-api\n\
  \    description: 'DERIVED: read fee-model values.'\n  - scope: 'margin-management-api:fee_model_value.create'\n    service: margin-management-api\n    description: 'DERIVED: create fee-model values.'\n  - scope: 'margin-management-api:fee_model_value.update'\n    service: margin-management-api\n    description: 'DERIVED: update fee-model values.'\n  - scope: 'margin-management-api:fee_model_value.delete'\n    service: margin-management-api\n    description: 'DERIVED: delete fee-model values.'\n  - scope: 'tlsuite:access'\n    service: tlsuite\n    description: 'DERIVED: baseline access to TripleLift Suite.'\n  - scope: 'tlsuite:segments_reporting'\n    service: tlsuite\n    description: 'DERIVED: segment reporting in TripleLift Suite.'\n  - scope: 'tlsuite:onboarded_data'\n    service: tlsuite\n    description: 'DERIVED: access onboarded first-party data.'\n  - scope: 'tlsuite:custom_segments'\n    service: tlsuite\n    description: 'DERIVED: manage custom segments.'\n  - scope: mcp\n\
  \    service: wordpress-mcp\n    description: Access the MCP server on the triplelift.com WordPress site. Published in that host's own authorization-server metadata.\n    method: probed\nscope_count: 51\nnotes:\n  - >-\n    Two wildcard scopes are requested by the first-party console on every login —\n    user-mgmt-api:*.* and deals-api:deal.* — alongside advertiser-connect:connect-request.*\n    and reporting-api:report.*. Wildcards in a requested scope set mean the token\n    the console holds is materially broader than any documented least-privilege\n    grant, and there is no published scope reference a partner could consult to\n    request less.\n  - >-\n    None of these scopes appear in TripleLift's public documentation. The Reporting\n    API — the one API TripleLift does document — does not use OAuth at all, so a\n    documented partner never encounters this catalog.\nx-evidence:\n  - url: https://app.triplelift.com/\n    http_status: 302\n    fetched: '2026-08-12'\n  - url: https://auth.triplelift.net/.well-known/openid-configuration\n\
  \    http_status: 200\n    fetched: '2026-08-12'\n  - url: https://triplelift.com/.well-known/oauth-authorization-server\n    http_status: 200\n    fetched: '2026-08-12'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/triplelift/refs/heads/main/scopes/triplelift-scopes.yml
summary_line: 51 scopes
tags:
- Programmatic Advertising
- Native Advertising
- Ad Exchange
- OpenRTB
- Header Bidding
- Connected TV
- Supply Side Platform
- Demand-Side Platform
- GraphQL
- AdTech
- Publisher Reporting
- Real-Time Bidding
token_urls: []
---
