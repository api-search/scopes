---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Great West Lifeco Scopes
name_suffix: OAuth Scopes
note: Both OAuth surfaces in the group are real and both withhold their scope vocabulary. This artifact records the authorization-server metadata that IS published and states plainly that no scope names are. Nothing is invented - the scopes list is empty because the providers publish an empty one.
overview: 'Great-West Lifeco uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.canadalife.com/oauth2/v1/generate.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Great-West Lifeco
provider_slug: great-west-lifeco
schemes:
- entity: Canada Life
  flows:
  - authorizationUrl: null
    flow: clientCredentials
    note: authorization_endpoint is published as https://api.canadalife.com/oauth2/v1/authorize-NOT-SUPPORTED - the interactive flow is explicitly disabled.
    tokenUrl: https://api.canadalife.com/oauth2/v1/generate
  name: CanadaLifeGatewayOIDC
  scopes_supported: []
  scopes_supported_note: 'The discovery document advertises "scopes_supported": [] - an empty array. Scopes are provisioned per client profile rather than advertised.'
  source: well-known/great-west-lifeco-openid-configuration.json
- entity: Empower (U.S. retirement subsidiary)
  flows:
  - flow: clientCredentials
    note: The OAuth 2.0 API catalog entry documents /token and /auth endpoint paths but never their host; the authorization service endpoint is emailed to approved partners only.
    tokenUrl: null
  name: EmpowerOAuth2
  scopes_supported: []
  scopes_supported_note: Scopes demonstrably exist and are enforced - the public release notes for version 1.3.1 state that the "/token endpoint can result 400 status code with 'invalid_grant' error message if requested oauth scope is not configured in oauth client profile" - but no scope name is published anywhere on the portal. Scopes are configured per OAuth client profile during the approval process.
  source: https://developer.empower.com/api-catalog/oauth2-api
scope_count: 0
scope_names: []
scopes: []
slug: great-west-lifeco-scopes
source_filename: great-west-lifeco-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: >-\n  https://api.canadalife.com/.well-known/openid-configuration (HTTP 200);\n  https://developer.empower.com/api-catalog/oauth2-api;\n  https://developer.empower.com/docs/get-started\ndocs: null\nnote: >-\n  Both OAuth surfaces in the group are real and both withhold their scope\n  vocabulary. This artifact records the authorization-server metadata that IS\n  published and states plainly that no scope names are. Nothing is invented -\n  the scopes list is empty because the providers publish an empty one.\nschemes:\n- name: CanadaLifeGatewayOIDC\n  entity: Canada Life\n  source: well-known/great-west-lifeco-openid-configuration.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.canadalife.com/oauth2/v1/generate\n    authorizationUrl: null\n    note: >-\n      authorization_endpoint is published as\n      https://api.canadalife.com/oauth2/v1/authorize-NOT-SUPPORTED - the\n      interactive flow is explicitly\
  \ disabled.\n  scopes_supported: []\n  scopes_supported_note: >-\n    The discovery document advertises \"scopes_supported\": [] - an empty array.\n    Scopes are provisioned per client profile rather than advertised.\n- name: EmpowerOAuth2\n  entity: Empower (U.S. retirement subsidiary)\n  source: https://developer.empower.com/api-catalog/oauth2-api\n  flows:\n  - flow: clientCredentials\n    tokenUrl: null\n    note: >-\n      The OAuth 2.0 API catalog entry documents /token and /auth endpoint paths\n      but never their host; the authorization service endpoint is emailed to\n      approved partners only.\n  scopes_supported: []\n  scopes_supported_note: >-\n    Scopes demonstrably exist and are enforced - the public release notes for\n    version 1.3.1 state that the \"/token endpoint can result 400 status code\n    with 'invalid_grant' error message if requested oauth scope is not\n    configured in oauth client profile\" - but no scope name is published\n    anywhere on the portal.\
  \ Scopes are configured per OAuth client profile\n    during the approval process.\nscopes: []\nscope_count: 0\nenforcement:\n  model: per-client-profile\n  evidence: >-\n    Empower OAuth 2.0 API release notes v1.3.1 - a requested scope that is not\n    configured on the client profile is rejected with HTTP 400 invalid_grant.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/great-west-lifeco/refs/heads/main/scopes/great-west-lifeco-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Insurance
- Canada
- Life Insurance
- Health Insurance
- Employee Benefits
- Retirement
- Wealth Management
- Reinsurance
- Annuities
- Partner Gated
token_urls:
- https://api.canadalife.com/oauth2/v1/generate
---
