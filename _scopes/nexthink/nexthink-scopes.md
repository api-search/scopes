---
api_specs:
- filename: nexthink-nql-api-openapi.json
  format: json
  label: Nexthink NQL API
  slug: nexthink-nql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexthink/refs/heads/main/openapi/nexthink-nql-api-openapi.json
- filename: nexthink-remote-actions-api-openapi.json
  format: json
  label: Nexthink Remote Actions API
  slug: nexthink-remote-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexthink/refs/heads/main/openapi/nexthink-remote-actions-api-openapi.json
- filename: nexthink-workflows-openapi.json
  format: json
  label: Nexthink Workflows API
  slug: nexthink-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexthink/refs/heads/main/openapi/nexthink-workflows-openapi.json
- filename: nexthink-enrichment-api-openapi.json
  format: json
  label: Nexthink Enrichment API
  slug: nexthink-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexthink/refs/heads/main/openapi/nexthink-enrichment-api-openapi.json
- filename: nexthink-campaigns-api-openapi.json
  format: json
  label: Nexthink Campaigns API
  slug: nexthink-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexthink/refs/heads/main/openapi/nexthink-campaigns-api-openapi.json
- filename: nexthink-data-management-api-openapi.json
  format: json
  label: Nexthink Data Management API
  slug: nexthink-data-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexthink/refs/heads/main/openapi/nexthink-data-management-api-openapi.json
- filename: nexthink-spark-api-openapi.json
  format: json
  label: Nexthink Spark API
  slug: nexthink-spark-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexthink/refs/heads/main/openapi/nexthink-spark-api-openapi.json
authorization_urls: []
description: ''
docs: https://docs.nexthink.com/api/getting-authentication-token
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Nexthink Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Nexthink publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Nexthink API on a user''s behalf.


  Tokens are issued from https://{instance}-login.{region}.nexthink.cloud/oauth2/default/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Nexthink
provider_slug: nexthink
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://{instance}-login.{region}.nexthink.cloud/oauth2/default/v1/token
  name: publicApiAuth
  source: openapi/nexthink-workflows-openapi.json
  type: oauth2
scope_count: 1
scope_names:
- service:integration
scopes:
- description: Grant used for the OAuth 2.0 client-credentials token request that authorizes an external integration to call the Nexthink public APIs. Passed as the `scope` form field on the token endpoint. Feature-level access (Remote Actions, Enrichment, Data Management, Workflows, Campaigns, NQL, Spark) is controlled by the permissions selected when the OAuth client credential is created in the Nexthink web interface, not by additional OAuth scopes.
  flows:
  - clientCredentials
  scope: service:integration
slug: nexthink-scopes
source_filename: nexthink-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/nexthink-workflows-openapi.json\ndocs: https://docs.nexthink.com/api/getting-authentication-token\nschemes:\n- name: publicApiAuth\n  type: oauth2\n  source: openapi/nexthink-workflows-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{instance}-login.{region}.nexthink.cloud/oauth2/default/v1/token\nscopes:\n- scope: 'service:integration'\n  description: >-\n    Grant used for the OAuth 2.0 client-credentials token request that authorizes\n    an external integration to call the Nexthink public APIs. Passed as the\n    `scope` form field on the token endpoint. Feature-level access (Remote\n    Actions, Enrichment, Data Management, Workflows, Campaigns, NQL, Spark) is\n    controlled by the permissions selected when the OAuth client credential is\n    created in the Nexthink web interface, not by additional OAuth scopes.\n  flows: [clientCredentials]\n  sources: [docs.nexthink.com/api/getting-authentication-token]\n\
  notes: >-\n  Nexthink issues a single documented OAuth scope (service:integration). Fine-grained\n  authorization is enforced through per-credential API permissions (checkboxes in\n  Administration > API credentials), so the scope surface is intentionally flat.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nexthink/refs/heads/main/scopes/nexthink-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Company
- Business Applications
- Digital Employee Experience
- Endpoint Analytics
- IT Operations
- Automation
- Observability
- DEX
token_urls:
- https://{instance}-login.{region}.nexthink.cloud/oauth2/default/v1/token
---
