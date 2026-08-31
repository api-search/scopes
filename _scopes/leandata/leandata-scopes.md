---
api_specs:
- filename: leandata-availability-api-openapi.yml
  format: yaml
  label: LeanData 🗓️ Availability API
  slug: leandata-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leandata/refs/heads/main/openapi/leandata-availability-api-openapi.yml
- filename: leandata-legacy-still-supported-api-openapi.yml
  format: yaml
  label: LeanData Legacy (still supported) API
  slug: leandata-legacy-still-supported-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leandata/refs/heads/main/openapi/leandata-legacy-still-supported-api-openapi.yml
- filename: leandata-matching-api-openapi.yml
  format: yaml
  label: LeanData Matching API
  slug: leandata-matching-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leandata/refs/heads/main/openapi/leandata-matching-api-openapi.yml
- filename: leandata-meetings-create-api-openapi.yml
  format: yaml
  label: LeanData 📆 Meetings > Create API
  slug: leandata-meetings-create-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leandata/refs/heads/main/openapi/leandata-meetings-create-api-openapi.yml
- filename: leandata-meetings-manage-api-openapi.yml
  format: yaml
  label: LeanData 📆 Meetings > Manage API
  slug: leandata-meetings-manage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leandata/refs/heads/main/openapi/leandata-meetings-manage-api-openapi.yml
- filename: leandata-meetings-retrieve-api-openapi.yml
  format: yaml
  label: LeanData 📆 Meetings > Retrieve API
  slug: leandata-meetings-retrieve-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leandata/refs/heads/main/openapi/leandata-meetings-retrieve-api-openapi.yml
- filename: leandata-one-time-routing-api-openapi.yml
  format: yaml
  label: LeanData One Time Routing API
  slug: leandata-one-time-routing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leandata/refs/heads/main/openapi/leandata-one-time-routing-api-openapi.yml
- filename: leandata-retrieve-routing-graphs-information-api-openapi.yml
  format: yaml
  label: LeanData Retrieve Routing Graphs Information API
  slug: leandata-retrieve-routing-graphs-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leandata/refs/heads/main/openapi/leandata-retrieve-routing-graphs-information-api-openapi.yml
- filename: leandata-scheduling-inputs-api-openapi.yml
  format: yaml
  label: LeanData 🧠 Scheduling Inputs API
  slug: leandata-scheduling-inputs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leandata/refs/heads/main/openapi/leandata-scheduling-inputs-api-openapi.yml
authorization_urls:
- https://mcp.leandata.com/authorize
description: LeanData's only OAuth scope surface belongs to the BookIt MCP server. The REST APIs on api.leandata.com use an unscoped X-Api-Key, and the Matching / Round Robin API borrows the customer's Salesforce Connected App session, so neither has scopes of its own. The four scopes below were read from the RFC 9728 protected-resource metadata LeanData serves at mcp.leandata.com — they are published values, not inferred ones. LeanData does not publish a scopes reference page, so the descriptions are the documented role model from the BookIt MCP release material mapped onto the scope names, and are marked as such.
docs: https://www.leandata.com/resources/leandatas-bookit-mcp/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Leandata Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'LeanData publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the LeanData API on a user''s behalf.


  Tokens are issued from https://mcp.leandata.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: LeanData
provider_slug: leandata
schemes:
- flows:
  - authorizationUrl: https://mcp.leandata.com/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    tokenUrl: https://mcp.leandata.com/token
  name: BookItMcpOAuth
  registration_endpoint: https://mcp.leandata.com/register
  source: https://mcp.leandata.com/.well-known/oauth-authorization-server
scope_count: 4
scope_names:
- admin
- user
- partner
- offline_access
scopes:
- description: Administrator-level access to the BookIt MCP tool set. LeanData documents the admin role as able to view cancelled meetings by pool / reason / date range, check real-time availability across users and pools by meeting type, identify reps who have not connected their calendars, and manage cancellations, rescheduling and host swaps.
  flows:
  - authorizationCode
  scope: admin
- description: Rep-level access. LeanData documents the rep role as able to look up their upcoming meetings and conference details, view their own meetings and pipeline, check their own availability, access their own profile and conferencing setup, and mark no-shows to trigger the credit-back process.
  flows:
  - authorizationCode
  scope: user
- description: External partner / agent access. Corresponds to the one-time-code onboarding path for partners and AI agents that have no Salesforce credentials in the customer's org; an email address and a permission set are assigned in advance.
  flows:
  - authorizationCode
  scope: partner
- description: Standard OAuth offline access — issues a refresh token so an agent can keep a long-lived session. refresh_token is one of the two grant types the authorization-server metadata advertises.
  flows:
  - authorizationCode
  scope: offline_access
slug: leandata-scopes
source_filename: leandata-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://mcp.leandata.com/.well-known/oauth-protected-resource\ndocs: https://www.leandata.com/resources/leandatas-bookit-mcp/\ndescription: >-\n  LeanData's only OAuth scope surface belongs to the BookIt MCP server. The REST APIs on\n  api.leandata.com use an unscoped X-Api-Key, and the Matching / Round Robin API borrows the\n  customer's Salesforce Connected App session, so neither has scopes of its own. The four\n  scopes below were read from the RFC 9728 protected-resource metadata LeanData serves at\n  mcp.leandata.com — they are published values, not inferred ones. LeanData does not publish\n  a scopes reference page, so the descriptions are the documented role model from the BookIt\n  MCP release material mapped onto the scope names, and are marked as such.\n\nresource: https://mcp.leandata.com\nauthorization_server: https://mcp.leandata.com\nschemes:\n  - name: BookItMcpOAuth\n    source: https://mcp.leandata.com/.well-known/oauth-authorization-server\n\
  \    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://mcp.leandata.com/authorize\n        tokenUrl: https://mcp.leandata.com/token\n        code_challenge_methods: [S256]\n    registration_endpoint: https://mcp.leandata.com/register\n\nscopes:\n  - scope: admin\n    description: >-\n      Administrator-level access to the BookIt MCP tool set. LeanData documents the admin role\n      as able to view cancelled meetings by pool / reason / date range, check real-time\n      availability across users and pools by meeting type, identify reps who have not connected\n      their calendars, and manage cancellations, rescheduling and host swaps.\n    description_source: role-model-mapping\n    flows: [authorizationCode]\n    sources: [https://mcp.leandata.com/.well-known/oauth-protected-resource]\n  - scope: user\n    description: >-\n      Rep-level access. LeanData documents the rep role as able to look up their upcoming\n      meetings and conference details, view their\
  \ own meetings and pipeline, check their own\n      availability, access their own profile and conferencing setup, and mark no-shows to\n      trigger the credit-back process.\n    description_source: role-model-mapping\n    flows: [authorizationCode]\n    sources: [https://mcp.leandata.com/.well-known/oauth-protected-resource]\n  - scope: partner\n    description: >-\n      External partner / agent access. Corresponds to the one-time-code onboarding path for\n      partners and AI agents that have no Salesforce credentials in the customer's org; an\n      email address and a permission set are assigned in advance.\n    description_source: role-model-mapping\n    flows: [authorizationCode]\n    sources: [https://mcp.leandata.com/.well-known/oauth-protected-resource]\n  - scope: offline_access\n    description: >-\n      Standard OAuth offline access — issues a refresh token so an agent can keep a long-lived\n      session. refresh_token is one of the two grant types the authorization-server\
  \ metadata\n      advertises.\n    description_source: oauth-standard\n    flows: [authorizationCode]\n    sources: [https://mcp.leandata.com/.well-known/oauth-authorization-server]\n\nenforcement:\n  note: >-\n    LeanData states that once a client is connected, the tools available to each caller are\n    automatically filtered by their BookIt permission set, and every action taken through the\n    MCP server respects the org's routing rules, pool fairness settings and SLA logic. Scope is\n    therefore an outer bound; the effective permission comes from Salesforce.\n\ngaps:\n  - >-\n    No public scopes reference page. The scope NAMES are machine-discoverable but their exact\n    grants are not published, so a client cannot request least privilege with confidence.\n  - >-\n    No scope surface on the REST APIs; a BookIt X-Api-Key is all-or-nothing.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leandata/refs/heads/main/scopes/leandata-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Revenue Operations
- Lead Routing
- Lead to Account Matching
- Salesforce
- Sales Engagement
- Sales Productivity
- Marketing Operations
- Scheduling
- Meeting Booking
- Account Based Marketing
- Buying Groups
- Signal Orchestration
- Go to Market
- GTM
- CRM
- AppExchange
token_urls:
- https://mcp.leandata.com/token
---
