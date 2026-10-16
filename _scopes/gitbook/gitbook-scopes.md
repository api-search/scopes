---
api_specs:
- filename: gitbook-change-request-content-api-openapi.yml
  format: yaml
  label: GitBook Change Request Content API
  slug: gitbook-change-request-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-change-request-content-api-openapi.yml
- filename: gitbook-change-request-reviewers-api-openapi.yml
  format: yaml
  label: GitBook Change Request Reviewers API
  slug: gitbook-change-request-reviewers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-change-request-reviewers-api-openapi.yml
- filename: gitbook-change-requests-api-openapi.yml
  format: yaml
  label: GitBook Change Requests API
  slug: gitbook-change-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-change-requests-api-openapi.yml
- filename: gitbook-collections-api-openapi.yml
  format: yaml
  label: GitBook Collections API
  slug: gitbook-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-collections-api-openapi.yml
- filename: gitbook-custom-hostnames-api-openapi.yml
  format: yaml
  label: GitBook Custom Hostnames API
  slug: gitbook-custom-hostnames-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-custom-hostnames-api-openapi.yml
- filename: gitbook-docs-sites-api-openapi.yml
  format: yaml
  label: GitBook Docs Sites API
  slug: gitbook-docs-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-docs-sites-api-openapi.yml
- filename: gitbook-imports-api-openapi.yml
  format: yaml
  label: GitBook Imports API
  slug: gitbook-imports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-imports-api-openapi.yml
- filename: gitbook-integrations-api-openapi.yml
  format: yaml
  label: GitBook Integrations API
  slug: gitbook-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-integrations-api-openapi.yml
- filename: gitbook-openapi-specs-api-openapi.yml
  format: yaml
  label: GitBook OpenAPI Specs API
  slug: gitbook-openapi-specs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-openapi-specs-api-openapi.yml
- filename: gitbook-organization-members-api-openapi.yml
  format: yaml
  label: GitBook Organization Members API
  slug: gitbook-organization-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-organization-members-api-openapi.yml
- filename: gitbook-organization-teams-api-openapi.yml
  format: yaml
  label: GitBook Organization Teams API
  slug: gitbook-organization-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-organization-teams-api-openapi.yml
- filename: gitbook-organizations-api-openapi.yml
  format: yaml
  label: GitBook Organizations API
  slug: gitbook-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-organizations-api-openapi.yml
- filename: gitbook-search-api-openapi.yml
  format: yaml
  label: GitBook Search API
  slug: gitbook-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-search-api-openapi.yml
- filename: gitbook-site-spaces-api-openapi.yml
  format: yaml
  label: GitBook Site Spaces API
  slug: gitbook-site-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-site-spaces-api-openapi.yml
- filename: gitbook-space-content-api-openapi.yml
  format: yaml
  label: GitBook Space Content API
  slug: gitbook-space-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-space-content-api-openapi.yml
- filename: gitbook-space-users-api-openapi.yml
  format: yaml
  label: GitBook Space Users API
  slug: gitbook-space-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-space-users-api-openapi.yml
- filename: gitbook-spaces-api-openapi.yml
  format: yaml
  label: GitBook Spaces API
  slug: gitbook-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-spaces-api-openapi.yml
- filename: gitbook-urls-api-openapi.yml
  format: yaml
  label: GitBook URLs API
  slug: gitbook-urls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-urls-api-openapi.yml
- filename: gitbook-users-api-openapi.yml
  format: yaml
  label: GitBook Users API
  slug: gitbook-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-users-api-openapi.yml
authorization_urls:
- https://oauth.gitbook.com/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Gitbook Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'GitBook publishes 29 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the GitBook API on a user''s behalf.


  Tokens are issued from https://oauth.gitbook.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: GitBook
provider_slug: gitbook
schemes:
- flows:
  - authorizationUrl: https://oauth.gitbook.com/authorize
    flow: authorizationCode
    tokenUrl: https://oauth.gitbook.com/token
  name: oauth
  source: openapi/gitbook-openapi.json
scope_count: 29
scope_names:
- change-request:merge
- integration:delete
- integration:installations:read
- integration:installations:write
- integration:publish
- integration:read
- openapi:read
- openapi:write
- organization:ask
- organization:members:read
- organization:members:write
- organization:read
- organization:search
- organization:write
- site:ask
- site:auth:read
- site:auth:write
- site:insights:read
- site:permissions:read
- site:permissions:write
- site:publish
- site:read
- site:search
- site:write
- space:permissions:read
- space:permissions:write
- space:read
- space:write
- user:read
scopes:
- description: Merge change requests, publishing their changes to the space. Creating, editing and reviewing change requests only requires space:write.
  flows:
  - authorizationCode
  scope: change-request:merge
- description: Unpublish integrations, permanently deleting them and every installation of them.
  flows:
  - authorizationCode
  scope: integration:delete
- description: Read integration installations and their configuration, which can include credentials for third-party services.
  flows:
  - authorizationCode
  scope: integration:installations:read
- description: Install and configure integrations on an organization, its spaces and its sites.
  flows:
  - authorizationCode
  scope: integration:installations:write
- description: Publish integrations, which can request their own permissions on your content, and route their events to a development tunnel.
  flows:
  - authorizationCode
  scope: integration:publish
- description: Read integrations, their status and where they are installed.
  flows:
  - authorizationCode
  scope: integration:read
- description: Read OpenAPI specifications.
  flows:
  - authorizationCode
  scope: openapi:read
- description: Create, update and delete OpenAPI specifications.
  flows:
  - authorizationCode
  scope: openapi:write
- description: Ask AI questions across an organization's content.
  flows:
  - authorizationCode
  scope: organization:ask
- description: Read organization members, teams, invites and link invites.
  flows:
  - authorizationCode
  scope: organization:members:read
- description: Manage organization members, teams, invites and link invites.
  flows:
  - authorizationCode
  scope: organization:members:write
- description: Read the organizations you belong to, their settings and metadata, and their AI agent conversations.
  flows:
  - authorizationCode
  scope: organization:read
- description: Search across an organization's content.
  flows:
  - authorizationCode
  scope: organization:search
- description: Create organizations, and update organization settings and AI agent conversations.
  flows:
  - authorizationCode
  scope: organization:write
- description: Ask AI questions across a site's content.
  flows:
  - authorizationCode
  scope: site:ask
- description: Read how visitors authenticate on a site and its security configuration, including private share links.
  flows:
  - authorizationCode
  scope: site:auth:read
- description: Manage how visitors authenticate on a site and its security configuration, including private share links.
  flows:
  - authorizationCode
  scope: site:auth:write
- description: Read site analytics and insights, including the questions visitors asked Ask AI and the answers they received.
  flows:
  - authorizationCode
  scope: site:insights:read
- description: Read the users and teams who have access to sites.
  flows:
  - authorizationCode
  scope: site:permissions:read
- description: Manage who has access to sites, including inviting users and teams.
  flows:
  - authorizationCode
  scope: site:permissions:write
- description: Publish and unpublish sites, controlling their public exposure.
  flows:
  - authorizationCode
  scope: site:publish
- description: Read sites and their settings, including navigation structure, linked spaces, customization, redirects, topics, AI configuration and documentation issues.
  flows:
  - authorizationCode
  scope: site:read
- description: Search across a site's content.
  flows:
  - authorizationCode
  scope: site:search
- description: Create, update and delete sites and their settings, including navigation structure (sections, linked spaces, external links), customization, redirects, topics and AI configuration.
  flows:
  - authorizationCode
  scope: site:write
- description: Read the users and teams who have access to spaces and collections.
  flows:
  - authorizationCode
  scope: space:permissions:read
- description: Manage who has access to spaces and collections, including inviting users and teams.
  flows:
  - authorizationCode
  scope: space:permissions:write
- description: Read spaces and their content, including pages, change requests and their reviews, comments, files and revision history.
  flows:
  - authorizationCode
  scope: space:read
- description: Create, update and delete spaces and their content, including change requests (create, edit, review), comments, and content imports and exports. Merging a change request also requires change-request:merge.
  flows:
  - authorizationCode
  scope: space:write
- description: Read your GitBook user profile.
  flows:
  - authorizationCode
  scope: user:read
slug: gitbook-scopes
source_filename: gitbook-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-05'\nmethod: derived\nsource: openapi/gitbook-openapi.json\nschemes:\n- name: oauth\n  source: openapi/gitbook-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://oauth.gitbook.com/authorize\n    tokenUrl: https://oauth.gitbook.com/token\nscopes:\n- scope: change-request:merge\n  description: Merge change requests, publishing their changes to the space. Creating, editing\n    and reviewing change requests only requires space:write.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gitbook-openapi.json\n- scope: integration:delete\n  description: Unpublish integrations, permanently deleting them and every installation of them.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gitbook-openapi.json\n- scope: integration:installations:read\n  description: Read integration installations and their configuration, which can include credentials\n    for third-party services.\n  flows:\n  - authorizationCode\n  sources:\n\
  \  - openapi/gitbook-openapi.json\n- scope: integration:installations:write\n  description: Install and configure integrations on an organization, its spaces and its sites.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gitbook-openapi.json\n- scope: integration:publish\n  description: Publish integrations, which can request their own permissions on your content,\n    and route their events to a development tunnel.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gitbook-openapi.json\n- scope: integration:read\n  description: Read integrations, their status and where they are installed.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gitbook-openapi.json\n- scope: openapi:read\n  description: Read OpenAPI specifications.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gitbook-openapi.json\n- scope: openapi:write\n  description: Create, update and delete OpenAPI specifications.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gitbook-openapi.json\n\
  - scope: organization:ask\n  description: Ask AI questions across an organization's content.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gitbook-openapi.json\n- scope: organization:members:read\n  description: Read organization members, teams, invites and link invites.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gitbook-openapi.json\n- scope: organization:members:write\n  description: Manage organization members, teams, invites and link invites.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gitbook-openapi.json\n- scope: organization:read\n  description: Read the organizations you belong to, their settings and metadata, and their\n    AI agent conversations.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gitbook-openapi.json\n- scope: organization:search\n  description: Search across an organization's content.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gitbook-openapi.json\n- scope: organization:write\n  description: Create\
  \ organizations, and update organization settings and AI agent conversations.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gitbook-openapi.json\n- scope: site:ask\n  description: Ask AI questions across a site's content.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gitbook-openapi.json\n- scope: site:auth:read\n  description: Read how visitors authenticate on a site and its security configuration, including\n    private share links.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gitbook-openapi.json\n- scope: site:auth:write\n  description: Manage how visitors authenticate on a site and its security configuration, including\n    private share links.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gitbook-openapi.json\n- scope: site:insights:read\n  description: Read site analytics and insights, including the questions visitors asked Ask\n    AI and the answers they received.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gitbook-openapi.json\n\
  - scope: site:permissions:read\n  description: Read the users and teams who have access to sites.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gitbook-openapi.json\n- scope: site:permissions:write\n  description: Manage who has access to sites, including inviting users and teams.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gitbook-openapi.json\n- scope: site:publish\n  description: Publish and unpublish sites, controlling their public exposure.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gitbook-openapi.json\n- scope: site:read\n  description: Read sites and their settings, including navigation structure, linked spaces,\n    customization, redirects, topics, AI configuration and documentation issues.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gitbook-openapi.json\n- scope: site:search\n  description: Search across a site's content.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gitbook-openapi.json\n- scope: site:write\n\
  \  description: Create, update and delete sites and their settings, including navigation structure\n    (sections, linked spaces, external links), customization, redirects, topics and AI configuration.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gitbook-openapi.json\n- scope: space:permissions:read\n  description: Read the users and teams who have access to spaces and collections.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gitbook-openapi.json\n- scope: space:permissions:write\n  description: Manage who has access to spaces and collections, including inviting users and\n    teams.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gitbook-openapi.json\n- scope: space:read\n  description: Read spaces and their content, including pages, change requests and their reviews,\n    comments, files and revision history.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gitbook-openapi.json\n- scope: space:write\n  description: Create, update and delete\
  \ spaces and their content, including change requests\n    (create, edit, review), comments, and content imports and exports. Merging a change request\n    also requires change-request:merge.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gitbook-openapi.json\n- scope: user:read\n  description: Read your GitBook user profile.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gitbook-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/scopes/gitbook-scopes.yml
summary_line: 29 scopes · authorizationCode
tags:
- Content
- Documentation
- Experience
- Integration
- Platform
- SDK
token_bound: false
token_urls:
- https://oauth.gitbook.com/token
---
