---
authorization_urls:
- https://auth.jit.io/oauth/authorize
description: ''
docs: https://docs.jit.io/reference
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Jit Fka Cbrix Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Jit (fka Cbrix) uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://auth.jit.io/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Jit (fka Cbrix)
provider_slug: jit-fka-cbrix
schemes:
- authorization_server: https://auth.jit.io
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.jit.io/oauth/token
  - authorizationUrl: https://auth.jit.io/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://auth.jit.io/oauth/token
  name: OAuth2
scope_count: 0
scope_names: []
scopes: []
slug: jit-fka-cbrix-scopes
source_filename: jit-fka-cbrix-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.jit.io/reference\ndocs: https://docs.jit.io/reference\ndiscovery: https://auth.jit.io/.well-known/openid-configuration\nschemes:\n- name: OAuth2\n  authorization_server: https://auth.jit.io\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.jit.io/oauth/token\n  - flow: authorizationCode\n    authorizationUrl: https://auth.jit.io/oauth/authorize\n    tokenUrl: https://auth.jit.io/oauth/token\noidc_scopes:\n- scope: openid\n  description: OpenID Connect authentication.\n- scope: profile\n  description: Access to the authenticated user's profile claims.\n- scope: email\n  description: Access to the authenticated user's email address.\npermissions:\n  description: >-\n    Jit API operations are gated by fine-grained jit.* permissions carried by the\n    JWT (derived from the token's role). Each API reference operation documents the\n    permission it requires.\n  scopes:\n  - scope: jit.artifacts.read\n\
  \    description: Read and download artifacts (SBOM, Wiz issues, ZAP scanned URLs).\n  - scope: jit.generalMetrics.read\n    description: Read general metrics such as SCM billable-minutes statistics.\n  - scope: jit.findings.read\n    description: List and read security findings and generate CSV reports.\n  - scope: jit.findings.write\n    description: Act on findings, e.g. dispatch an Open Fix Pull Request event.\n  - scope: jit.preferences.read\n    description: Read tenant/user preferences and the Security-as-Code configuration file.\n  - scope: jit.preferences.write\n    description: Update the Security-as-Code configuration file.\n  - scope: jit.integrations.read\n    description: Read the integration file / third-party integration configuration.\n  - scope: jit.integrations.write\n    description: Update the integration file / third-party integration configuration.\n  - scope: jit.teams.read\n    description: List teams, members, and child teams.\n  - scope: jit.teams.write\n   \
  \ description: Create, update, delete, and import teams.\n  - scope: jit.trigger.write\n    description: Trigger synchronous executions (controls CLI / local environments).\n  - scope: jit.policies.read\n    description: Read policy rules, templates, and entity types.\n  - scope: jit.policies.write\n    description: Create, update, and delete policy rules (Premium).\n  - scope: jit.workflows.read\n    description: Fetch workflows, step options, and workflow runs (Premium).\n  - scope: jit.workflows.write\n    description: Create, update, and delete workflows (Premium).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jit-fka-cbrix/refs/heads/main/scopes/jit-fka-cbrix-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Cybersecurity
- Application Security
- DevSecOps
- ASPM
- Security
- Vulnerability Management
- API
token_urls:
- https://auth.jit.io/oauth/token
---
