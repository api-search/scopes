---
api_specs:
- filename: kit-openapi.yml
  format: yaml
  label: Kit API V4
  slug: kit-api-v4
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kit/refs/heads/main/openapi/kit-openapi.yml
authorization_urls:
- https://app.kit.com/oauth/authorize
description: ''
docs: https://developers.kit.com/api-reference/oauth-proof-key-for-code-exchange-flow
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Kit Scopes
name_suffix: OAuth Scopes
note: Kit API V4 OAuth currently exposes a single default scope (public); the docs state "Fine-grained access control via scopes coming soon" (https://developers.kit.com/api-reference/oauth-proof-key-for-code-exchange-flow).
overview: 'Kit publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Kit API on a user''s behalf.


  Tokens are issued from https://api.kit.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Kit
provider_slug: kit
schemes:
- flows:
  - authorizationUrl: https://app.kit.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.kit.com/oauth/token
  name: OAuth2
  source: openapi/kit-openapi.yml
scope_count: 1
scope_names:
- public
scopes:
- description: Default (and currently only) scope for Kit API V4 OAuth apps, granting API access on behalf of the authorizing account; fine-grained access control via scopes is documented as coming soon.
  flows: []
  scope: public
slug: kit-scopes
source_filename: kit-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\nsource: openapi/kit-openapi.yml\ndocs: https://developers.kit.com/api-reference/oauth-proof-key-for-code-exchange-flow\nnote: >-\n  Kit API V4 OAuth currently exposes a single default scope (public); the docs\n  state \"Fine-grained access control via scopes coming soon\"\n  (https://developers.kit.com/api-reference/oauth-proof-key-for-code-exchange-flow).\nschemes:\n- name: OAuth2\n  source: openapi/kit-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.kit.com/oauth/authorize\n    tokenUrl: https://api.kit.com/oauth/token\nscopes:\n- scope: public\n  description: >-\n    Default (and currently only) scope for Kit API V4 OAuth apps, granting API\n    access on behalf of the authorizing account; fine-grained access control\n    via scopes is documented as coming soon.\n  sources:\n  - https://developers.kit.com/api-reference/oauth-proof-key-for-code-exchange-flow\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kit/refs/heads/main/scopes/kit-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Email Marketing
- Creator Economy
- Newsletters
- Automation
- Subscribers
token_urls:
- https://api.kit.com/oauth/token
---
