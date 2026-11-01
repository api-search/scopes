---
authorization_urls: []
description: Scopes read verbatim from the scopes_supported array of Target's two OpenID Connect discovery documents. Both issuers advertise the same four scopes. These are identity scopes only — Target publishes no anonymous resource-scope reference for its product, inventory, order or store APIs, because those APIs are documented behind the developer.target.com login. Do not read this list as the full permission surface of Target's APIs; it is the full ANONYMOUSLY DISCOVERABLE surface.
docs: https://logonservices.oauth.iam.partnersonline.com/guide/
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Target Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Target publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Target API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Target
provider_slug: target
schemes: []
scope_count: 4
scope_names:
- openid
- email
- profile
- openid_client_registration
scopes:
- description: Request an ID token; required for any OpenID Connect flow.
  flows: []
  scope: openid
- description: Release the subject's email address claim to the client.
  flows: []
  scope: email
- description: Release the subject's profile claims to the client.
  flows: []
  scope: profile
- description: Permits dynamic client registration against the issuer's registration_endpoint (/openid/connect/register). Advertised on both issuers.
  flows: []
  scope: openid_client_registration
slug: target-scopes
source_filename: target-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: https://oauth.iam.target.com/.well-known/openid-configuration\ndocs: https://logonservices.oauth.iam.partnersonline.com/guide/\ndescription: >-\n  Scopes read verbatim from the scopes_supported array of Target's two OpenID Connect discovery\n  documents. Both issuers advertise the same four scopes. These are identity scopes only — Target\n  publishes no anonymous resource-scope reference for its product, inventory, order or store APIs,\n  because those APIs are documented behind the developer.target.com login. Do not read this list as\n  the full permission surface of Target's APIs; it is the full ANONYMOUSLY DISCOVERABLE surface.\nissuers:\n- issuer: https://oauth.iam.target.com\n  discovery: https://oauth.iam.target.com/.well-known/openid-configuration\n  http_status: 200\n- issuer: https://oauth.iam.partnersonline.com\n  discovery: https://oauth.iam.partnersonline.com/.well-known/openid-configuration\n  http_status: 200\n\
  scope_count: 4\nscopes:\n- name: openid\n  description: Request an ID token; required for any OpenID Connect flow.\n  issuers:\n  - https://oauth.iam.target.com\n  - https://oauth.iam.partnersonline.com\n- name: email\n  description: Release the subject's email address claim to the client.\n  issuers:\n  - https://oauth.iam.target.com\n  - https://oauth.iam.partnersonline.com\n- name: profile\n  description: Release the subject's profile claims to the client.\n  issuers:\n  - https://oauth.iam.target.com\n  - https://oauth.iam.partnersonline.com\n- name: openid_client_registration\n  description: >-\n    Permits dynamic client registration against the issuer's registration_endpoint\n    (/openid/connect/register). Advertised on both issuers.\n  issuers:\n  - https://oauth.iam.target.com\n  - https://oauth.iam.partnersonline.com\nclaims_supported:\n- sub\n- iss\n- auth_time\n- acr\n- aud\n- azp\n- exp\n- c_hash\n- at_hash\n- nonce\ngaps:\n- No resource/API scopes are published anonymously;\
  \ the API catalog behind developer.target.com\n  returns HTTP 401 without a key.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://artifacts.apis.io/target/scopes/target-scopes.yml
summary_line: 4 scopes
tags:
- Fortune 100
- E-Commerce
- Retail
- Product
- Inventory
- Stores
- Order
token_bound: false
token_urls: []
---
