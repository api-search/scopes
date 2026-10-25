---
api_specs:
- filename: go1-categories-api-openapi.yml
  format: yaml
  label: Go1 Categories API
  slug: go1-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/go1/refs/heads/main/openapi/go1-categories-api-openapi.yml
- filename: go1-collections-api-openapi.yml
  format: yaml
  label: Go1 Collections API
  slug: go1-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/go1/refs/heads/main/openapi/go1-collections-api-openapi.yml
- filename: go1-compliance-api-openapi.yml
  format: yaml
  label: Go1 Compliance API
  slug: go1-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/go1/refs/heads/main/openapi/go1-compliance-api-openapi.yml
- filename: go1-enrollments-api-openapi.yml
  format: yaml
  label: Go1 Enrollments API
  slug: go1-enrollments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/go1/refs/heads/main/openapi/go1-enrollments-api-openapi.yml
- filename: go1-files-api-openapi.yml
  format: yaml
  label: Go1 Files API
  slug: go1-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/go1/refs/heads/main/openapi/go1-files-api-openapi.yml
- filename: go1-learning-objects-api-openapi.yml
  format: yaml
  label: Go1 Learning objects API
  slug: go1-learning-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/go1/refs/heads/main/openapi/go1-learning-objects-api-openapi.yml
- filename: go1-plans-api-openapi.yml
  format: yaml
  label: Go1 Plans API
  slug: go1-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/go1/refs/heads/main/openapi/go1-plans-api-openapi.yml
- filename: go1-play-links-api-openapi.yml
  format: yaml
  label: Go1 Play links API
  slug: go1-play-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/go1/refs/heads/main/openapi/go1-play-links-api-openapi.yml
- filename: go1-playlists-api-openapi.yml
  format: yaml
  label: Go1 Playlists API
  slug: go1-playlists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/go1/refs/heads/main/openapi/go1-playlists-api-openapi.yml
- filename: go1-portals-api-openapi.yml
  format: yaml
  label: Go1 Portals API
  slug: go1-portals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/go1/refs/heads/main/openapi/go1-portals-api-openapi.yml
- filename: go1-restrictions-api-openapi.yml
  format: yaml
  label: Go1 Restrictions API
  slug: go1-restrictions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/go1/refs/heads/main/openapi/go1-restrictions-api-openapi.yml
- filename: go1-scim-api-openapi.yml
  format: yaml
  label: Go1 SCIM API
  slug: go1-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/go1/refs/heads/main/openapi/go1-scim-api-openapi.yml
- filename: go1-user-accounts-api-openapi.yml
  format: yaml
  label: Go1 User accounts API
  slug: go1-user-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/go1/refs/heads/main/openapi/go1-user-accounts-api-openapi.yml
- filename: go1-webhooks-api-openapi.yml
  format: yaml
  label: Go1 Webhooks API
  slug: go1-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/go1/refs/heads/main/openapi/go1-webhooks-api-openapi.yml
authorization_urls:
- https://auth.go1.com/oauth/authorize
description: ''
docs: https://developers.go1.com/docs/developer-tools/auth/oauth-scopes/
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Go1 Scopes
name_suffix: OAuth Scopes
note: 'Go1 publishes a standalone OAuth Scopes page; descriptions below are taken from it. It advises: "We suggest requesting only those which are necessary for the integration".'
overview: 'Go1 publishes 19 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Go1 API on a user''s behalf.


  Tokens are issued from https://auth.go1.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Go1
provider_slug: go1
schemes:
- description: OAuth 2.0. Server-to-server integrations use the client_credentials flow; user-context integrations use the authorization_code flow. Access tokens are valid for 12 hours.
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.go1.com/oauth/token
  - authorizationUrl: https://auth.go1.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://auth.go1.com/oauth/token
  name: OAuth2
  source: openapi/go1-openapi.yml
scope_count: 19
scope_names:
- enrollment.read
- enrollment.write
- lo.read
- lo.write
- portal.read
- portal.write
- webhook.read
- webhook.write
- assignment.read
- basic.read
- group.read
- group.write
- lo.launch
- plan.read
- plan.write
- user.login
- user.read
- user.write
- wallet.organization.read
scopes:
- description: Read enrollment data.
  flows:
  - authorizationCode
  - clientCredentials
  scope: enrollment.read
- description: Write access to enrollment data.
  flows:
  - authorizationCode
  - clientCredentials
  scope: enrollment.write
- description: Read access to view available learning objects.
  flows:
  - authorizationCode
  - clientCredentials
  scope: lo.read
- description: Write access to create and modify learning objects.
  flows:
  - authorizationCode
  - clientCredentials
  scope: lo.write
- description: Read access to portal integrations.
  flows:
  - authorizationCode
  - clientCredentials
  scope: portal.read
- description: Create and update portals.
  flows:
  - authorizationCode
  - clientCredentials
  scope: portal.write
- description: Read configured webhooks.
  flows:
  - authorizationCode
  - clientCredentials
  scope: webhook.read
- description: Create and update webhooks.
  flows:
  - authorizationCode
  - clientCredentials
  scope: webhook.write
- description: Read assignment data.
  flows: []
  scope: assignment.read
- description: Generic read access.
  flows: []
  scope: basic.read
- description: Read user group membership and assignment information.
  flows: []
  scope: group.read
- description: Manage user group membership and assignment information.
  flows: []
  scope: group.write
- description: Access to play content via authenticated play links.
  flows: []
  scope: lo.launch
- description: Read plans.
  flows: []
  scope: plan.read
- description: Create and update plans.
  flows: []
  scope: plan.write
- description: Generate single-use login tokens. This scope is restricted and must be enabled on your developer app by Go1. Please contact support to request access.
  flows: []
  scope: user.login
- description: Read user data.
  flows: []
  scope: user.read
- description: Create and update user accounts.
  flows: []
  scope: user.write
- description: Read wallet organization data.
  flows: []
  scope: wallet.organization.read
slug: go1-scopes
source_filename: go1-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: searched\nsource: https://developers.go1.com/docs/developer-tools/auth/oauth-scopes/\ndocs: https://developers.go1.com/docs/developer-tools/auth/oauth-scopes/\nnote: 'Go1 publishes a standalone OAuth Scopes page; descriptions below are taken from it. It advises: \"We suggest\n  requesting only those which are necessary for the integration\".'\nschemes:\n- name: OAuth2\n  source: openapi/go1-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.go1.com/oauth/token\n  - flow: authorizationCode\n    authorizationUrl: https://auth.go1.com/oauth/authorize\n    tokenUrl: https://auth.go1.com/oauth/token\n  description: OAuth 2.0. Server-to-server integrations use the client_credentials flow; user-context integrations\n    use the authorization_code flow. Access tokens are valid for 12 hours.\nscopes:\n- scope: enrollment.read\n  description: Read enrollment data.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n\
  \  - openapi/go1-openapi.yml\n- scope: enrollment.write\n  description: Write access to enrollment data.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/go1-openapi.yml\n- scope: lo.read\n  description: Read access to view available learning objects.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/go1-openapi.yml\n- scope: lo.write\n  description: Write access to create and modify learning objects.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/go1-openapi.yml\n- scope: portal.read\n  description: Read access to portal integrations.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/go1-openapi.yml\n- scope: portal.write\n  description: Create and update portals.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/go1-openapi.yml\n- scope: webhook.read\n  description: Read configured webhooks.\n  flows:\n  - authorizationCode\n \
  \ - clientCredentials\n  sources:\n  - openapi/go1-openapi.yml\n- scope: webhook.write\n  description: Create and update webhooks.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/go1-openapi.yml\n- scope: assignment.read\n  description: Read assignment data.\n  source: docs (not in OpenAPI security requirements)\n- scope: basic.read\n  description: Generic read access.\n  source: docs (not in OpenAPI security requirements)\n- scope: group.read\n  description: Read user group membership and assignment information.\n  source: docs (not in OpenAPI security requirements)\n- scope: group.write\n  description: Manage user group membership and assignment information.\n  source: docs (not in OpenAPI security requirements)\n- scope: lo.launch\n  description: Access to play content via authenticated play links.\n  source: docs (not in OpenAPI security requirements)\n- scope: plan.read\n  description: Read plans.\n  source: docs (not in OpenAPI security requirements)\n\
  - scope: plan.write\n  description: Create and update plans.\n  source: docs (not in OpenAPI security requirements)\n- scope: user.login\n  description: Generate single-use login tokens. This scope is restricted and must be enabled on your developer\n    app by Go1. Please contact support to request access.\n  source: docs (not in OpenAPI security requirements)\n  restricted: true\n- scope: user.read\n  description: Read user data.\n  source: docs (not in OpenAPI security requirements)\n- scope: user.write\n  description: Create and update user accounts.\n  source: docs (not in OpenAPI security requirements)\n- scope: wallet.organization.read\n  description: Read wallet organization data.\n  source: docs (not in OpenAPI security requirements)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/go1/refs/heads/main/scopes/go1-scopes.yml
summary_line: 19 scopes · clientCredentials/authorizationCode
tags:
- Company
- EdTech
- Learning
- E-Learning
- Corporate Training
- Content
- LMS
- Education
- Webhook
token_bound: false
token_urls:
- https://auth.go1.com/oauth/token
---
