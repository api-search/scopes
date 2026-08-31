---
api_specs:
- filename: cybelangel-adm-inventory-api-openapi.yml
  format: yaml
  label: CybelAngel ADM Inventory API
  slug: cybelangel-adm-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cybelangel/refs/heads/main/openapi/cybelangel-adm-inventory-api-openapi.yml
- filename: cybelangel-alerts-api-openapi.yml
  format: yaml
  label: CybelAngel Alerts API
  slug: cybelangel-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cybelangel/refs/heads/main/openapi/cybelangel-alerts-api-openapi.yml
- filename: cybelangel-asset-api-openapi.yml
  format: yaml
  label: CybelAngel Asset API
  slug: cybelangel-asset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cybelangel/refs/heads/main/openapi/cybelangel-asset-api-openapi.yml
- filename: cybelangel-audit-logs-api-openapi.yml
  format: yaml
  label: CybelAngel audit logs API
  slug: cybelangel-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cybelangel/refs/heads/main/openapi/cybelangel-audit-logs-api-openapi.yml
- filename: cybelangel-credential-watchlist-api-openapi.yml
  format: yaml
  label: CybelAngel Credential watchlist API
  slug: cybelangel-credential-watchlist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cybelangel/refs/heads/main/openapi/cybelangel-credential-watchlist-api-openapi.yml
- filename: cybelangel-domain-watchlist-api-openapi.yml
  format: yaml
  label: CybelAngel Domain watchlist API
  slug: cybelangel-domain-watchlist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cybelangel/refs/heads/main/openapi/cybelangel-domain-watchlist-api-openapi.yml
- filename: cybelangel-incident-reports-api-openapi.yml
  format: yaml
  label: CybelAngel Incident reports API
  slug: cybelangel-incident-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cybelangel/refs/heads/main/openapi/cybelangel-incident-reports-api-openapi.yml
- filename: cybelangel-keywords-api-openapi.yml
  format: yaml
  label: CybelAngel Keywords API
  slug: cybelangel-keywords-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cybelangel/refs/heads/main/openapi/cybelangel-keywords-api-openapi.yml
- filename: cybelangel-reports-api-openapi.yml
  format: yaml
  label: CybelAngel Reports API
  slug: cybelangel-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cybelangel/refs/heads/main/openapi/cybelangel-reports-api-openapi.yml
- filename: cybelangel-stats-api-openapi.yml
  format: yaml
  label: CybelAngel Stats API
  slug: cybelangel-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cybelangel/refs/heads/main/openapi/cybelangel-stats-api-openapi.yml
- filename: cybelangel-stix-api-openapi.yml
  format: yaml
  label: CybelAngel Stix API
  slug: cybelangel-stix-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cybelangel/refs/heads/main/openapi/cybelangel-stix-api-openapi.yml
- filename: cybelangel-threat-intelligence-api-openapi.yml
  format: yaml
  label: CybelAngel Threat Intelligence API
  slug: cybelangel-threat-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cybelangel/refs/heads/main/openapi/cybelangel-threat-intelligence-api-openapi.yml
- filename: cybelangel-workspaces-api-openapi.yml
  format: yaml
  label: CybelAngel Workspaces API
  slug: cybelangel-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cybelangel/refs/heads/main/openapi/cybelangel-workspaces-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Cybelangel Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'CybelAngel publishes 10 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the CybelAngel API on a user''s behalf.


  Tokens are issued from https://auth.cybelangel.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CybelAngel
provider_slug: cybelangel
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.cybelangel.com/oauth/token
  name: bearer_token
  source: openapi/cybelangel-platform-reports-openapi.yml
scope_count: 10
scope_names:
- assets.download
- credentials.export
- credentials.move
- credentials.read
- reports.move
- reports.read
- reports_global_comments.read
- reports_global_comments.write
- usergroups.admin
- usergroups.read
scopes:
- description: Downloading an asset
  flows:
  - clientCredentials
  scope: assets.download
- description: Export list of credentials
  flows:
  - clientCredentials
  scope: credentials.export
- description: Resolve or reopen a credential
  flows:
  - clientCredentials
  scope: credentials.move
- description: Read list of leaked monitored credentials
  flows:
  - clientCredentials
  scope: credentials.read
- description: Resolve or reopen an incident report
  flows:
  - clientCredentials
  scope: reports.move
- description: Read incident reports
  flows:
  - clientCredentials
  scope: reports.read
- description: Read comments of a incident report
  flows:
  - clientCredentials
  scope: reports_global_comments.read
- description: Write comments on a incident report (Endpoint not accessible, yet)
  flows:
  - clientCredentials
  scope: reports_global_comments.write
- description: Read and manage usergroups
  flows:
  - clientCredentials
  scope: usergroups.admin
- description: Read subscribed usergroups
  flows:
  - clientCredentials
  scope: usergroups.read
slug: cybelangel-scopes
source_filename: cybelangel-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: derived\nsource: openapi/cybelangel-platform-reports-openapi.yml\nschemes:\n- name: bearer_token\n  source: openapi/cybelangel-platform-reports-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.cybelangel.com/oauth/token\nscopes:\n- scope: assets.download\n  description: Downloading an asset\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/cybelangel-platform-reports-openapi.yml\n- scope: credentials.export\n  description: Export list of credentials\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/cybelangel-platform-reports-openapi.yml\n- scope: credentials.move\n  description: Resolve or reopen a credential\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/cybelangel-platform-reports-openapi.yml\n- scope: credentials.read\n  description: Read list of leaked monitored credentials\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/cybelangel-platform-reports-openapi.yml\n- scope:\
  \ reports.move\n  description: Resolve or reopen an incident report\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/cybelangel-platform-reports-openapi.yml\n- scope: reports.read\n  description: Read incident reports\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/cybelangel-platform-reports-openapi.yml\n- scope: reports_global_comments.read\n  description: Read comments of a incident report\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/cybelangel-platform-reports-openapi.yml\n- scope: reports_global_comments.write\n  description: Write comments on a incident report (Endpoint not accessible, yet)\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/cybelangel-platform-reports-openapi.yml\n- scope: usergroups.admin\n  description: Read and manage usergroups\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/cybelangel-platform-reports-openapi.yml\n- scope: usergroups.read\n  description: Read subscribed usergroups\n  flows:\n  - clientCredentials\n\
  \  sources:\n  - openapi/cybelangel-platform-reports-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cybelangel/refs/heads/main/scopes/cybelangel-scopes.yml
summary_line: 10 scopes · clientCredentials
tags:
- Company
- Cybersecurity
- Threat Intelligence
- external-attack-surface-management
- data-breach-prevention
- credential-intelligence
- brand-protection
- dark-web-monitoring
- digital-risk-protection
- STIX
- security-alerts
- asset-inventory
- audit-logs
token_urls:
- https://auth.cybelangel.com/oauth/token
---
