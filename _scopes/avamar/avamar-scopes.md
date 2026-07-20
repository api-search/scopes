---
authorization_urls: []
description: ''
docs: https://www.dell.com/support/manuals/en-us/avamar-server/avamar_administration_guide_19.10/avamar-rest-api
flows:
- password
- authorizationCode
- clientCredentials
- implicit
kind: oauth-scopes
layout: scope
method: searched
name: Avamar Scopes
name_suffix: OAuth Scopes
note: Scopes are issued by the customer's own Avamar server, not by a Dell-hosted authorization server. Dell's documentation publishes a coarse read/write model rather than a per-resource scope registry; fine-grained authorization is carried by the Avamar role assigned to the authenticating user (the token response returns `role`, `domain` and `authorized_domain`).
overview: 'Avamar publishes 5 OAuth 2.0 scopes via the password, authorizationCode, clientCredentials, and implicit flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Avamar API on a user''s behalf.


  Tokens are issued from https://<AvamarServer>/api/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Avamar
provider_slug: avamar
schemes:
- flows:
  - clientRegistrationUrl: https://<AvamarServer>/api/v1/oauth2/clients
    flow: password
    tokenUrl: https://<AvamarServer>/api/oauth/token
  name: oauth2_password
  source: authentication/avamar-authentication.yml
- flows:
  - flow: authorizationCode
  - flow: clientCredentials
  - flow: implicit
  name: openid_connect_sso
  source: authentication/avamar-authentication.yml
scope_count: 5
scope_names:
- read
- write
- all
- openid
- profile
scopes:
- description: Read access to Avamar REST API resources.
  flows:
  - password
  - authorizationCode
  scope: read
- description: Write access to Avamar REST API resources, including creating clients, datasets and backups.
  flows:
  - password
  - authorizationCode
  scope: write
- description: Wildcard value accepted in the `autoApproveScopes` field of an OAuth 2.0 client registration, auto-approving every scope granted to that client.
  flows:
  - password
  scope: all
- description: Standard OIDC scope requesting an ID token. Used by the Keycloak SSO integration.
  flows:
  - authorizationCode
  - implicit
  scope: openid
- description: Standard OIDC scope requesting the authenticated user's profile claims.
  flows:
  - authorizationCode
  - implicit
  scope: profile
slug: avamar-scopes
source_filename: avamar-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://www.dell.com/support/manuals/en-us/avamar-server/avamar_administration_guide_19.10/avamar-rest-api\ndocs: https://www.dell.com/support/manuals/en-us/avamar-server/avamar_administration_guide_19.10/avamar-rest-api\nnote: >-\n  Scopes are issued by the customer's own Avamar server, not by a Dell-hosted authorization server.\n  Dell's documentation publishes a coarse read/write model rather than a per-resource scope registry;\n  fine-grained authorization is carried by the Avamar role assigned to the authenticating user (the\n  token response returns `role`, `domain` and `authorized_domain`).\nschemes:\n- name: oauth2_password\n  source: authentication/avamar-authentication.yml\n  flows:\n  - flow: password\n    tokenUrl: https://<AvamarServer>/api/oauth/token\n    clientRegistrationUrl: https://<AvamarServer>/api/v1/oauth2/clients\n- name: openid_connect_sso\n  source: authentication/avamar-authentication.yml\n  flows:\n\
  \  - flow: authorizationCode\n  - flow: clientCredentials\n  - flow: implicit\nscopes:\n- scope: read\n  description: Read access to Avamar REST API resources.\n  flows:\n  - password\n  - authorizationCode\n  sources:\n  - https://www.dell.com/support/manuals/en-us/avamar-server/avamar_administration_guide_19.10/avamar-rest-api\n- scope: write\n  description: Write access to Avamar REST API resources, including creating clients, datasets and backups.\n  flows:\n  - password\n  - authorizationCode\n  sources:\n  - https://www.dell.com/support/manuals/en-us/avamar-server/avamar_administration_guide_19.10/avamar-rest-api\n- scope: all\n  description: >-\n    Wildcard value accepted in the `autoApproveScopes` field of an OAuth 2.0 client registration,\n    auto-approving every scope granted to that client.\n  flows:\n  - password\n  sources:\n  - https://www.dell.com/support/manuals/en-us/avamar-server/avamar_administration_guide_19.10/avamar-rest-api\n- scope: openid\n  description: Standard\
  \ OIDC scope requesting an ID token. Used by the Keycloak SSO integration.\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - https://www.dell.com/support/manuals/en-us/avamar-server/avamar_administration_guide_19.10/avamar-rest-api\n- scope: profile\n  description: Standard OIDC scope requesting the authenticated user's profile claims.\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - https://www.dell.com/support/manuals/en-us/avamar-server/avamar_administration_guide_19.10/avamar-rest-api\nauthorization_model:\n  mechanism: role-and-domain\n  description: >-\n    Beyond the read/write scope, effective permissions derive from the Avamar role bound to the token\n    subject and the Avamar domain the token is authorized for. The access-token response carries\n    `role` (for example ROOT), `domain` and `authorized_domain`.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avamar/refs/heads/main/scopes/avamar-scopes.yml
summary_line: 5 scopes · password/authorizationCode/clientCredentials/implicit
tags:
- Company
- Backup
- Data Protection
- Deduplication
- Disaster Recovery
- Storage
- Enterprise Software
- Infrastructure
- Dell Technologies
- On-Premise
token_urls:
- https://<AvamarServer>/api/oauth/token
---
