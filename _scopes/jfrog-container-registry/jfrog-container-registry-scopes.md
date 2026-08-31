---
authorization_urls: []
description: Scope grammar for JFrog Platform scoped access tokens — the credential used for the REST surface behind JFrog Container Registry. Read from JFrog's own access-token documentation; no OpenAPI securityScheme block exists to derive from (JFrog publishes no downloadable spec).
docs: https://docs.jfrog.com/administration/reference/create-scoped-token
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Jfrog Container Registry Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'JFrog Container Registry uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: JFrog Container Registry
provider_slug: jfrog-container-registry
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: jfrog-container-registry-scopes
source_filename: jfrog-container-registry-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "specification: API Commons OAuth Scopes\nspecificationVersion: '0.1'\nprovider: JFrog Container Registry\nproviderId: jfrog-container-registry\ngenerated: '2026-08-29'\nmodified: '2026-08-29'\nmethod: searched\nsource: https://docs.jfrog.com/administration/docs/access-tokens\ndocs: https://docs.jfrog.com/administration/reference/create-scoped-token\ndescription: >-\n  Scope grammar for JFrog Platform scoped access tokens — the credential used for the REST\n  surface behind JFrog Container Registry. Read from JFrog's own access-token documentation;\n  no OpenAPI securityScheme block exists to derive from (JFrog publishes no downloadable spec).\nmodel: >-\n  Since Artifactory 7.21.1 every access token is a SCOPED token. REST API access is granted by\n  default; the scope string then adds the permissions the token carries. Scopes are passed as a\n  space- or comma-delimited `scope` form field on POST /access/api/v1/tokens.\nscopes:\n  - name: applied-permissions/user\n    description:\
  \ >-\n      The token carries exactly the permissions of the user it was created for. This is the\n      default for a self-created identity token.\n  - name: applied-permissions/admin\n    description: >-\n      Admin-level permissions across the platform. Only an Artifactory administrator can mint\n      this. Used by companion services (Xray, Mission Control) that require admin access.\n  - name: 'applied-permissions/groups:<group-name>[,<group-name>...]'\n    description: The token is granted the permissions of the named group(s).\n  - name: 'applied-permissions/roles:<project-key>:<role>[,<role>...]'\n    description: >-\n      Project-scoped role grant. Documented example —\n      scope=applied-permissions/roles:project-key:developer,qa\n  - name: 'system:info/storage:r'\n    description: >-\n      Resource-style read scope. Named explicitly by the Get Storage Summary Info operation,\n      which states it \"Requires authentication using Access Tokens, either as admin or using a\n\
  \      scoped token with the system:info/storage:r scope.\"\n    evidence: https://docs.jfrog.com/artifactory/reference/getstoragesummaryinfo\ntoken_kinds:\n  - name: Identity token\n    description: A user-scoped token any user can create for themselves.\n    docs: https://docs.jfrog.com/user-management/docs/identity-tokens\n  - name: Reference token\n    description: >-\n      A short opaque token that can be used in place of a password for basic authentication by\n      clients that only support basic auth.\n  - name: Admin scoped token\n  - name: Project admin token\n  - name: Group scoped token\nnotes:\n  - >-\n    A token's scope is visible in the Access Tokens UI as a Scope column from Artifactory 7.46.3.\n  - >-\n    This is not an RFC 6749 delegated-authorization scope list — JFrog's scopes are permission\n    assertions minted into the token, not consented OAuth scopes on an authorization endpoint.\n    The OAuth flow JFrog does expose is the MCP server's client authorization;\
  \ its scope set is\n    not published and could not be introspected anonymously.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jfrog-container-registry/refs/heads/main/scopes/jfrog-container-registry-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Container Images
- Containers
- Docker
- Helm
- JFrog
- Registry
token_urls: []
---
