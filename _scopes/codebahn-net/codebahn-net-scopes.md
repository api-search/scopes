---
api_specs:
- filename: codebahn-net-activitypub-api-openapi.yml
  format: yaml
  label: Codebahn Activitypub API
  slug: codebahn-net-activitypub-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebahn-net/openapi/codebahn-net-activitypub-api-openapi.yml
- filename: codebahn-net-admin-api-openapi.yml
  format: yaml
  label: Codebahn Admin API
  slug: codebahn-net-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebahn-net/openapi/codebahn-net-admin-api-openapi.yml
- filename: codebahn-net-issue-api-openapi.yml
  format: yaml
  label: Codebahn Issue API
  slug: codebahn-net-issue-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebahn-net/openapi/codebahn-net-issue-api-openapi.yml
- filename: codebahn-net-miscellaneous-api-openapi.yml
  format: yaml
  label: Codebahn Miscellaneous API
  slug: codebahn-net-miscellaneous-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebahn-net/openapi/codebahn-net-miscellaneous-api-openapi.yml
- filename: codebahn-net-notification-api-openapi.yml
  format: yaml
  label: Codebahn Notification API
  slug: codebahn-net-notification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebahn-net/openapi/codebahn-net-notification-api-openapi.yml
- filename: codebahn-net-organization-api-openapi.yml
  format: yaml
  label: Codebahn Organization API
  slug: codebahn-net-organization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebahn-net/openapi/codebahn-net-organization-api-openapi.yml
- filename: codebahn-net-package-api-openapi.yml
  format: yaml
  label: Codebahn Package API
  slug: codebahn-net-package-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebahn-net/openapi/codebahn-net-package-api-openapi.yml
- filename: codebahn-net-repository-api-openapi.yml
  format: yaml
  label: Codebahn Repository API
  slug: codebahn-net-repository-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebahn-net/openapi/codebahn-net-repository-api-openapi.yml
- filename: codebahn-net-settings-api-openapi.yml
  format: yaml
  label: Codebahn Settings API
  slug: codebahn-net-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebahn-net/openapi/codebahn-net-settings-api-openapi.yml
- filename: codebahn-net-user-api-openapi.yml
  format: yaml
  label: Codebahn User API
  slug: codebahn-net-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebahn-net/openapi/codebahn-net-user-api-openapi.yml
authorization_urls: []
description: ''
docs: https://forgejo.org/docs/v15.0/user/api-usage/#authentication
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Codebahn Scopes
name_suffix: OAuth Scopes
note: The contract declares no oauth2 securityDefinition. Docs document an OAuth flow for the CLI and MCP server and Forgejo personal access tokens with scopes; only the scopes the Codebahn docs name are listed here.
overview: 'Codebahn publishes 3 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Codebahn API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Codebahn
provider_slug: codebahn-net
schemes: []
scope_count: 3
scope_names:
- read:package
- write:package
- read:repository
scopes:
- description: Pull container images / read packages; recommended per-consumer pull credential.
  flows: []
  scope: read:package
- description: Push container images / publish packages.
  flows: []
  scope: write:package
- description: Clone repositories from an external CI system.
  flows: []
  scope: read:repository
slug: codebahn-net-scopes
source_filename: codebahn-net-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://codebahn.net/docs/container-registry.md\ndocs: https://forgejo.org/docs/v15.0/user/api-usage/#authentication\nnote: The contract declares no oauth2 securityDefinition. Docs document an OAuth flow for the CLI and MCP server and Forgejo personal access tokens with scopes; only the scopes the Codebahn docs name are listed here.\nscopes:\n- name: read:package\n  description: Pull container images / read packages; recommended per-consumer pull credential.\n  source: https://codebahn.net/docs/container-registry.md\n- name: write:package\n  description: Push container images / publish packages.\n  source: https://codebahn.net/docs/container-registry.md\n- name: read:repository\n  description: Clone repositories from an external CI system.\n  source: https://codebahn.net/docs/run-your-own-ci.md\n"
source_yaml_url: https://artifacts.apis.io/codebahn-net/scopes/codebahn-net-scopes.yml
summary_line: 3 scopes
tags:
- Company
- Git Hosting
- Version Control
- Continuous Integration
- Forgejo
- Developer Tools
- EU-hosted
- Data Sovereignty
- MCP
token_bound: false
token_urls: []
---
