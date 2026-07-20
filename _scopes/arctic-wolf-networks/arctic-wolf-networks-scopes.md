---
authorization_urls: []
description: ''
docs: https://docs.arcticwolf.com/en/developer-and-oem/aurora-multi-tenant-api/aurora-multi-tenant-api
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Arctic Wolf Networks Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Arctic Wolf Networks publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Arctic Wolf Networks API on a user''s behalf.


  Tokens are issued from https://api-admin.cylance.com/public/v2/{region_code}/auth.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Arctic Wolf Networks
provider_slug: arctic-wolf-networks
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api-admin.cylance.com/public/v2/{region_code}/auth
  name: AuroraMultiTenantOAuth
scope_count: 1
scope_names:
- api
scopes:
- description: The single scope requested on the client-credentials token request (scope=api); grants access to the Aurora Multi-Tenant / Endpoint Defense API resource surface for the authorized partner application.
  flows:
  - clientCredentials
  scope: api
slug: arctic-wolf-networks-scopes
source_filename: arctic-wolf-networks-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.arcticwolf.com/en/developer-and-oem/aurora-multi-tenant-api/aurora-multi-tenant-api/getting-started\ndocs: https://docs.arcticwolf.com/en/developer-and-oem/aurora-multi-tenant-api/aurora-multi-tenant-api\nschemes:\n- name: AuroraMultiTenantOAuth\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-admin.cylance.com/public/v2/{region_code}/auth\nscopes:\n- scope: api\n  description: >-\n    The single scope requested on the client-credentials token request\n    (scope=api); grants access to the Aurora Multi-Tenant / Endpoint Defense\n    API resource surface for the authorized partner application.\n  flows: [clientCredentials]\n  sources: [docs.arcticwolf.com]\nnotes: >-\n  Arctic Wolf's Aurora API documents a coarse-grained single-scope (api) OAuth\n  client-credentials model rather than fine-grained per-resource scopes;\n  authorization is scoped by the partner application's provisioned tenants.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arctic-wolf-networks/refs/heads/main/scopes/arctic-wolf-networks-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Company
- Cybersecurity
- Security Operations
- Managed Detection and Response
- Endpoint Security
- Threat Detection
- Incident Response
token_urls:
- https://api-admin.cylance.com/public/v2/{region_code}/auth
---
