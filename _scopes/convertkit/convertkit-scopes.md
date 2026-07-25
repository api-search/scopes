---
api_specs:
- filename: convertkit-accounts-api-openapi.yml
  format: yaml
  label: Kit Accounts API
  slug: convertkit-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-accounts-api-openapi.yml
- filename: convertkit-broadcasts-api-openapi.yml
  format: yaml
  label: Kit Broadcasts API
  slug: convertkit-broadcasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-broadcasts-api-openapi.yml
- filename: convertkit-custom-fields-api-openapi.yml
  format: yaml
  label: Kit Custom Fields API
  slug: convertkit-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-custom-fields-api-openapi.yml
- filename: convertkit-email-templates-api-openapi.yml
  format: yaml
  label: Kit Email Templates API
  slug: convertkit-email-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-email-templates-api-openapi.yml
- filename: convertkit-forms-api-openapi.yml
  format: yaml
  label: Kit Forms API
  slug: convertkit-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-forms-api-openapi.yml
- filename: convertkit-posts-api-openapi.yml
  format: yaml
  label: Kit Posts API
  slug: convertkit-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-posts-api-openapi.yml
- filename: convertkit-purchases-api-openapi.yml
  format: yaml
  label: Kit Purchases API
  slug: convertkit-purchases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-purchases-api-openapi.yml
- filename: convertkit-segments-api-openapi.yml
  format: yaml
  label: Kit Segments API
  slug: convertkit-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-segments-api-openapi.yml
- filename: convertkit-sequence-emails-api-openapi.yml
  format: yaml
  label: Kit Sequence Emails API
  slug: convertkit-sequence-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-sequence-emails-api-openapi.yml
- filename: convertkit-sequences-api-openapi.yml
  format: yaml
  label: Kit Sequences API
  slug: convertkit-sequences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-sequences-api-openapi.yml
- filename: convertkit-snippets-api-openapi.yml
  format: yaml
  label: Kit Snippets API
  slug: convertkit-snippets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-snippets-api-openapi.yml
- filename: convertkit-subscribers-api-openapi.yml
  format: yaml
  label: Kit Subscribers API
  slug: convertkit-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-subscribers-api-openapi.yml
- filename: convertkit-tags-api-openapi.yml
  format: yaml
  label: Kit Tags API
  slug: convertkit-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-tags-api-openapi.yml
- filename: convertkit-webhooks-api-openapi.yml
  format: yaml
  label: Kit Webhooks API
  slug: convertkit-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-webhooks-api-openapi.yml
authorization_urls:
- https://api.kit.com/v4/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Convertkit Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Kit publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Kit API on a user''s behalf.


  Tokens are issued from https://api.kit.com/v4/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Kit
provider_slug: convertkit
schemes:
- description: Authenticate API requests via an OAuth token
  flows:
  - authorizationUrl: https://api.kit.com/v4/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.kit.com/v4/oauth/token
  name: OAuth2
  source: openapi/openapi.json
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Read access to Kit API v4
  flows:
  - authorizationCode
  scope: read
- description: Write access to Kit API v4
  flows:
  - authorizationCode
  scope: write
slug: convertkit-scopes
source_filename: convertkit-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json\nschemes:\n- name: OAuth2\n  source: openapi/openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.kit.com/v4/oauth/authorize\n    tokenUrl: https://api.kit.com/v4/oauth/token\n  description: Authenticate API requests via an OAuth token\nscopes:\n- scope: read\n  description: Read access to Kit API v4\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi.json\n- scope: write\n  description: Write access to Kit API v4\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/scopes/convertkit-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Email Marketing
- Creator Economy
- Subscribers
- Automation
- Newsletters
- Sequences
- Forms
- Broadcasts
token_urls:
- https://api.kit.com/v4/oauth/token
---
