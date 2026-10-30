---
api_specs:
- filename: plainrouter-actiondryrunapi-api-openapi.yml
  format: yaml
  label: Plainrouter Action Dry Run API
  slug: plainrouter-actiondryrunapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plainrouter/refs/heads/main/openapi/plainrouter-actiondryrunapi-api-openapi.yml
- filename: plainrouter-actionproposalapi-api-openapi.yml
  format: yaml
  label: Plainrouter Action Proposal API
  slug: plainrouter-actionproposalapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plainrouter/refs/heads/main/openapi/plainrouter-actionproposalapi-api-openapi.yml
- filename: plainrouter-actionreadapi-api-openapi.yml
  format: yaml
  label: Plainrouter Action Read API
  slug: plainrouter-actionreadapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plainrouter/refs/heads/main/openapi/plainrouter-actionreadapi-api-openapi.yml
- filename: plainrouter-actionruleapi-api-openapi.yml
  format: yaml
  label: Plainrouter Action Rule API
  slug: plainrouter-actionruleapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plainrouter/refs/heads/main/openapi/plainrouter-actionruleapi-api-openapi.yml
- filename: plainrouter-adtestapi-api-openapi.yml
  format: yaml
  label: Plainrouter Ad Test API
  slug: plainrouter-adtestapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plainrouter/refs/heads/main/openapi/plainrouter-adtestapi-api-openapi.yml
- filename: plainrouter-agentcontext-api-openapi.yml
  format: yaml
  label: Plainrouter Agent Context API
  slug: plainrouter-agentcontext-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plainrouter/refs/heads/main/openapi/plainrouter-agentcontext-api-openapi.yml
- filename: plainrouter-cookiedeclaration-api-openapi.yml
  format: yaml
  label: Plainrouter Cookie Declaration API
  slug: plainrouter-cookiedeclaration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plainrouter/refs/heads/main/openapi/plainrouter-cookiedeclaration-api-openapi.yml
- filename: plainrouter-creative-api-openapi.yml
  format: yaml
  label: Plainrouter Creative API
  slug: plainrouter-creative-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plainrouter/refs/heads/main/openapi/plainrouter-creative-api-openapi.yml
- filename: plainrouter-deploymentplan-api-openapi.yml
  format: yaml
  label: Plainrouter Deployment Plan API
  slug: plainrouter-deploymentplan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plainrouter/refs/heads/main/openapi/plainrouter-deploymentplan-api-openapi.yml
- filename: plainrouter-draftbatchfileimport-api-openapi.yml
  format: yaml
  label: Plainrouter Draft Batch File Import API
  slug: plainrouter-draftbatchfileimport-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plainrouter/refs/heads/main/openapi/plainrouter-draftbatchfileimport-api-openapi.yml
- filename: plainrouter-event-api-openapi.yml
  format: yaml
  label: Plainrouter Event API
  slug: plainrouter-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plainrouter/refs/heads/main/openapi/plainrouter-event-api-openapi.yml
- filename: plainrouter-launchpolicy-api-openapi.yml
  format: yaml
  label: Plainrouter Launch Policy API
  slug: plainrouter-launchpolicy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plainrouter/refs/heads/main/openapi/plainrouter-launchpolicy-api-openapi.yml
- filename: plainrouter-metainventoryexposure-api-openapi.yml
  format: yaml
  label: Plainrouter Meta Inventory Exposure API
  slug: plainrouter-metainventoryexposure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plainrouter/refs/heads/main/openapi/plainrouter-metainventoryexposure-api-openapi.yml
- filename: plainrouter-operations-api-openapi.yml
  format: yaml
  label: Plainrouter Operations API
  slug: plainrouter-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plainrouter/refs/heads/main/openapi/plainrouter-operations-api-openapi.yml
- filename: plainrouter-sandbox-api-openapi.yml
  format: yaml
  label: Plainrouter Sandbox API
  slug: plainrouter-sandbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plainrouter/refs/heads/main/openapi/plainrouter-sandbox-api-openapi.yml
authorization_urls:
- https://plainrouter.com/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Plainrouter Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Plainrouter publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Plainrouter API on a user''s behalf.


  Tokens are issued from https://plainrouter.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Plainrouter
provider_slug: plainrouter
schemes:
- description: OAuth access token for an active approved agent principal with mcp:use, ad-account.read and agent.context authorization. Authorization code with PKCE and device authorization tokens are accepted. This scheme applies only to agent context.
  flows:
  - authorizationUrl: https://plainrouter.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://plainrouter.com/oauth2/token
  name: agentContextOAuth
  source: openapi/plainrouter-openapi.json
scope_count: 1
scope_names:
- mcp:use
scopes:
- description: Use the approved agent principal.
  flows:
  - authorizationCode
  scope: mcp:use
slug: plainrouter-scopes
source_filename: plainrouter-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: derived\nsource: openapi/plainrouter-openapi.json\nschemes:\n- name: agentContextOAuth\n  source: openapi/plainrouter-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://plainrouter.com/oauth2/authorize\n    tokenUrl: https://plainrouter.com/oauth2/token\n  description: OAuth access token for an active approved agent principal with mcp:use, ad-account.read\n    and agent.context authorization. Authorization code with PKCE and device authorization tokens\n    are accepted. This scheme applies only to agent context.\nscopes:\n- scope: mcp:use\n  description: Use the approved agent principal.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/plainrouter-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plainrouter/refs/heads/main/scopes/plainrouter-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Advertising
- Developer Tools
- PaidAds
token_bound: false
token_urls:
- https://plainrouter.com/oauth2/token
---
