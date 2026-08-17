---
api_specs:
- filename: hootsuite-rest-api-openapi.yml
  format: yaml
  label: Hootsuite REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hootsuite/refs/heads/main/openapi/hootsuite-rest-api-openapi.yml
- filename: hootsuite-analytics-api-openapi.yml
  format: yaml
  label: Hootsuite Analytics REST API
  slug: analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hootsuite/refs/heads/main/openapi/hootsuite-analytics-api-openapi.yml
- filename: hootsuite-inbox-api-openapi.yml
  format: yaml
  label: Hootsuite Inbox 2.0 API
  slug: inbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hootsuite/refs/heads/main/openapi/hootsuite-inbox-api-openapi.yml
- filename: hootsuite-amplify-api-openapi.yml
  format: yaml
  label: Hootsuite Amplify REST API
  slug: amplify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hootsuite/refs/heads/main/openapi/hootsuite-amplify-api-openapi.yml
authorization_urls:
- https://platform.hootsuite.com/oauth2/auth
description: Hootsuite's OAuth scope surface is deliberately tiny - the authorization server advertises exactly two scopes - because scopes are not how Hootsuite authorizes. Access is decided by the caller's dashboard role (organization / team / social-network permissions), which Hootsuite publishes as a separate operation-by-operation permissions matrix. Both layers are recorded here, because holding the right scope is necessary and not sufficient.
docs: https://developer.hootsuite.com/docs/api-permissions-matrix
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Hootsuite Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Hootsuite publishes 2 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Hootsuite API on a user''s behalf.


  Tokens are issued from https://platform.hootsuite.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Hootsuite
provider_slug: hootsuite
schemes:
- flows:
  - authorizationUrl: https://platform.hootsuite.com/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://platform.hootsuite.com/oauth2/token
  name: OAuth2
  source: openapi/hootsuite-rest-api-openapi.yml
- flows:
  - authorizationUrl: https://platform.hootsuite.com/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://platform.hootsuite.com/oauth2/token
  name: OAuth2
  source: openapi/hootsuite-analytics-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: TO_BE_CONFIGURED_IN_INBOX_2_0
  name: Oauth2ClientCredentials
  source: openapi/hootsuite-inbox-api-openapi.yml
scope_count: 2
scope_names:
- offline
- analytics:read
scopes:
- description: Request refresh tokens. Without it the authorization-code exchange returns an access token only, and the integration must re-prompt the user every hour.
  flows:
  - authorizationCode
  scope: offline
- description: Request analytics API access.
  flows:
  - authorizationCode
  - member_app
  scope: analytics:read
slug: hootsuite-scopes
source_filename: hootsuite-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://platform.hootsuite.com/.well-known/oauth-authorization-server,\n  https://developer.hootsuite.com/docs/using-the-api,\n  https://developer.hootsuite.com/docs/api-permissions-matrix,\n  openapi/hootsuite-rest-api-openapi.yml, openapi/hootsuite-analytics-api-openapi.yml,\n  openapi/hootsuite-inbox-api-openapi.yml\ndocs: https://developer.hootsuite.com/docs/api-permissions-matrix\ndescription: >-\n  Hootsuite's OAuth scope surface is deliberately tiny - the authorization server advertises exactly\n  two scopes - because scopes are not how Hootsuite authorizes. Access is decided by the caller's\n  dashboard role (organization / team / social-network permissions), which Hootsuite publishes as a\n  separate operation-by-operation permissions matrix. Both layers are recorded here, because holding\n  the right scope is necessary and not sufficient.\nscope_count: 2\nauthoritative_source: https://platform.hootsuite.com/.well-known/oauth-authorization-server\n\
  schemes:\n- name: OAuth2\n  source: openapi/hootsuite-rest-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://platform.hootsuite.com/oauth2/auth\n    tokenUrl: https://platform.hootsuite.com/oauth2/token\n- name: OAuth2\n  source: openapi/hootsuite-analytics-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://platform.hootsuite.com/oauth2/auth\n    tokenUrl: https://platform.hootsuite.com/oauth2/token\n- name: Oauth2ClientCredentials\n  source: openapi/hootsuite-inbox-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: TO_BE_CONFIGURED_IN_INBOX_2_0\nscopes:\n- scope: offline\n  description: >-\n    Request refresh tokens. Without it the authorization-code exchange returns an access token only,\n    and the integration must re-prompt the user every hour.\n  flows:\n  - authorizationCode\n  grants_access_to: nothing on its own - it is a token-lifetime scope, not a data scope\n  sources:\n  - https://platform.hootsuite.com/.well-known/oauth-authorization-server\n\
  \  - openapi/hootsuite-rest-api-openapi.yml\n  - openapi/hootsuite-analytics-api-openapi.yml\n- scope: analytics:read\n  description: Request analytics API access.\n  flows:\n  - authorizationCode\n  - member_app\n  grants_access_to:\n  - POST /v1/analytics/posts (listPosts)\n  - POST /v1/analytics/profiles (listProfilesMetrics)\n  - POST /v1/analytics/paid/{adEntityCollection} (listPaid)\n  - POST /v1/analytics/paid/{adEntityCollection}/metrics (listPaidMetrics)\n  enablement: >-\n    Must be enabled on the app itself before it can be requested - App directory -> Developer apps\n    -> [app] -> Security -> Rest API tab -> tick analytics:read -> Save.\n  sources:\n  - https://platform.hootsuite.com/.well-known/oauth-authorization-server\n  - https://developer.hootsuite.com/docs/using-the-api\n  - openapi/hootsuite-analytics-api-openapi.yml\nnot_a_scope:\n- value: some_scope\n  found_in: openapi/hootsuite-inbox-api-openapi.yml (Oauth2ClientCredentials.scopes)\n  description_in_spec: TO_BE_CONFIGURED_IN_INBOX_2_0\n\
  \  note: >-\n    Placeholder text left in the published Inbox 2.0 specification, not a real scope. Recorded here\n    so a later derive pass does not promote it into the scopes[] list. Inbox 2.0 client-credentials\n    scope is provisioned per customer as a CRM-Instance-URL value, per\n    https://developer.hootsuite.com/reference/oauth2token.\ncoverage:\n  operations_total: 76\n  operations_covered_by_a_data_scope: 4\n  note: >-\n    Only the four Analytics operations sit behind a data scope. The other 72 published operations -\n    including scheduling messages, deleting messages, creating members, removing members from\n    organizations and the full SCIM 2.0 provisioning surface - are reachable with a token carrying\n    no data scope at all. There is no publish scope, no read-only scope and no admin scope.\npermission_model:\n  note: >-\n    The real authorization boundary. Hootsuite publishes required permissions per operation at\n    https://developer.hootsuite.com/docs/api-permissions-matrix.\n\
  \  organization_levels:\n  - Admin or above\n  custom_organization_permissions:\n  - Manage Members\n  - Manage Teams\n  team_permissions:\n  - Admin OR Member in Team\n  custom_team_permissions:\n  - Manage Social Networks in the Team\n  social_network_levels:\n  - Limited or above\n  - Editor or above\n  custom_social_network_permissions:\n  - Basic Usage\n  - Publish Message\n  - Publish Message with Approval\n  examples:\n  - operation: POST /v1/messages\n    social_network_permission: Limited or above\n    custom: Publish Message OR Publish Message with Approval\n  - operation: DELETE /v1/messages/{messageId}\n    social_network_permission: Editor or above\n    custom: Publish Message (Scheduled) OR Publish Message with Approval (Pending)\n  - operation: POST /v1/members\n    organization_permission: Admin or above\n    custom: Manage Members\n  - operation: GET /v1/socialProfiles\n    social_network_permission: Limited or above\n    custom: Basic Usage\n  - operation: GET /v1/organizations/{organizationId}/teams\n\
  \    organization_permission: Admin or above\n    custom: Manage Teams\n  failure_codes:\n  - 4002 Insufficient permissions to view organization members\n  - 4003 Insufficient permissions to view member permissions\n  - 4004 Insufficient permissions to view member organizations\n  - 4005 Insufficient permissions to view team members\n  - 4006 Insufficient permissions to view team\n  - 4007 Insufficient permissions to create team\n  - 4008 Insufficient permissions to view team social profile\n  - 4009 Insufficient organization permissions\n  - 4010 Insufficient permissions to view organization teams\n  - 1037 The required scope to access this endpoint was not granted by the user\n  - 1201 Not authorized to make changes to organization\nmetadata_caveat: >-\n  https://platform.hootsuite.com/.well-known/oauth-protected-resource publishes scopes_supported as\n  a single string \"offline analytics:read\" rather than a two-element JSON array. A strict RFC 9728\n  client reads that as ONE scope\
  \ named \"offline analytics:read\" and will request it verbatim.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hootsuite/refs/heads/main/scopes/hootsuite-scopes.yml
summary_line: 2 scopes · authorizationCode/clientCredentials
tags:
- Social Media
- Social Media Management
- Marketing
- Content Scheduling
- Analytics
- Engagement
- Social Listening
- Employee Advocacy
- Customer Service
- SCIM
- OAuth 2.0
- Webhooks
token_urls:
- https://platform.hootsuite.com/oauth2/token
- TO_BE_CONFIGURED_IN_INBOX_2_0
---
