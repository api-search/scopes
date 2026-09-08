---
authorization_urls:
- https://cspm.<tenant>.accuknox.com/api/v1/o/authorize/
description: ''
docs: https://help.accuknox.com/integrations/oauth/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Accuknox Scopes
name_suffix: OAuth Scopes
note: AccuKnox documents a real OAuth 2.0 authorization-code surface but publishes NO scope vocabulary. Its OAuth page states that access is governed by role-based authentication on the AccuKnox user profile, not by scopes on the token, and no scopes appear in any authorization request example. scope_count is therefore an honest zero, and NO `OAuthScopes` pointer is wired into apis.yml — a pointer of that name against a document containing no scopes would assert a surface AccuKnox does not publish.
overview: 'AccuKnox uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://cspm.<tenant>.accuknox.com/api/v1/o/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AccuKnox
provider_slug: accuknox
schemes:
- flows:
  - authorizationUrl: https://cspm.<tenant>.accuknox.com/api/v1/o/authorize/
    flow: authorizationCode
    tokenUrl: https://cspm.<tenant>.accuknox.com/api/v1/o/token/
  name: oauth2
  source: https://help.accuknox.com/integrations/oauth/
scope_count: 0
scope_names: []
scopes: []
slug: accuknox-scopes
source_filename: accuknox-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: https://help.accuknox.com/integrations/oauth/\ndocs: https://help.accuknox.com/integrations/oauth/\nnote: >-\n  AccuKnox documents a real OAuth 2.0 authorization-code surface but publishes NO scope\n  vocabulary. Its OAuth page states that access is governed by role-based authentication on\n  the AccuKnox user profile, not by scopes on the token, and no scopes appear in any\n  authorization request example. scope_count is therefore an honest zero, and NO\n  `OAuthScopes` pointer is wired into apis.yml — a pointer of that name against a document\n  containing no scopes would assert a surface AccuKnox does not publish.\nscope_count: 0\nschemes:\n- name: oauth2\n  source: https://help.accuknox.com/integrations/oauth/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://cspm.<tenant>.accuknox.com/api/v1/o/authorize/\n    tokenUrl: https://cspm.<tenant>.accuknox.com/api/v1/o/token/\nscopes: []\nauthorization_model:\n\
  \  style: role-based\n  evidence: >-\n    \"role based authentication\" on the AccuKnox user profile, per\n    https://help.accuknox.com/integrations/oauth/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accuknox/refs/heads/main/scopes/accuknox-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Security
- Cloud Security
- Cloud Native Application Protection Platform
- Kubernetes Security
- Runtime Security
- Zero Trust
- DevSecOps
- Compliance
- AI Security
- Vulnerability Management
- Container Security
token_urls:
- https://cspm.<tenant>.accuknox.com/api/v1/o/token/
---
