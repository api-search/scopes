---
authorization_urls:
- https://equipmentshare-erp.us.auth0.com/authorize
description: ''
docs: https://github.com/EquipmentShare/t3os-examples/tree/main/apps/oauth-hello-world
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Equipmentshare Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'EquipmentShare publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the EquipmentShare API on a user''s behalf.


  Tokens are issued from https://equipmentshare-erp.us.auth0.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: EquipmentShare
provider_slug: equipmentshare
schemes:
- flows:
  - audience: https://api.equipmentshare.com/es-erp-api/delegated
    authorizationUrl: https://equipmentshare-erp.us.auth0.com/authorize
    flow: authorizationCode
    pkce: true
    tokenUrl: https://equipmentshare-erp.us.auth0.com/oauth/token
  name: T3OS OAuth2
  source: https://github.com/EquipmentShare/t3os-examples
scope_count: 2
scope_names:
- all_resources_reader
- contact_reader
scopes:
- description: Broadest read-only scope — read access across all T3OS resources the user can see.
  flows:
  - authorizationCode
  scope: all_resources_reader
- description: Read access to contacts only (example of the narrow, per-resource read scope pattern).
  flows:
  - authorizationCode
  scope: contact_reader
slug: equipmentshare-scopes
source_filename: equipmentshare-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://github.com/EquipmentShare/t3os-examples\ndocs: https://github.com/EquipmentShare/t3os-examples/tree/main/apps/oauth-hello-world\n# T3OS user-delegated OAuth uses granular per-resource read scopes following the pattern\n# `<resource>_reader`. The consent UI shows the user every scope an app requests; integrations\n# are advised to request the narrowest scope that satisfies their queries. Standard OIDC scopes\n# are served by the underlying Auth0 tenant (verified from its openid-configuration).\nschemes:\n- name: T3OS OAuth2\n  source: https://github.com/EquipmentShare/t3os-examples\n  flows:\n  - flow: authorizationCode\n    pkce: true\n    authorizationUrl: https://equipmentshare-erp.us.auth0.com/authorize\n    tokenUrl: https://equipmentshare-erp.us.auth0.com/oauth/token\n    audience: https://api.equipmentshare.com/es-erp-api/delegated\nscopes:\n- scope: all_resources_reader\n  description: Broadest read-only scope\
  \ — read access across all T3OS resources the user can see.\n  flows: [authorizationCode]\n  sources: [https://github.com/EquipmentShare/t3os-examples/tree/main/apps/oauth-hello-world]\n- scope: contact_reader\n  description: Read access to contacts only (example of the narrow, per-resource read scope pattern).\n  flows: [authorizationCode]\n  sources: [https://github.com/EquipmentShare/t3os-examples/tree/main/apps/oauth-hello-world]\nscope_pattern: \"<resource>_reader\"\noidc_scopes:\n  source: https://equipmentshare-erp.us.auth0.com/.well-known/openid-configuration\n  scopes: [openid, profile, email, offline_access, name, given_name, family_name, nickname, phone, address, picture]\nnotes: >-\n  Only two scope names are published verbatim in the reference apps (all_resources_reader,\n  contact_reader); the documented convention is per-resource `_reader` scopes. The full scope\n  registry lives behind the T3OS dev portal (app.t3os.ai) and app registration.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/equipmentshare/refs/heads/main/scopes/equipmentshare-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company
- Construction Technology
- Fleet Management
- Telematics
- Equipment Rental
- GraphQL
- Developer Platform
- OAuth
token_urls:
- https://equipmentshare-erp.us.auth0.com/oauth/token
---
