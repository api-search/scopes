---
api_specs:
- filename: venafi-certificate-manager-saas-openapi.yml
  format: yaml
  label: Certificate Manager - SaaS API (Venafi Control Plane)
  slug: certificate-manager-saas
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venafi/refs/heads/main/openapi/venafi-certificate-manager-saas-openapi.yml
- filename: venafi-trust-protection-foundation-websdk-openapi.yml
  format: yaml
  label: Trust Protection Foundation WebSDK (Venafi Trust Protection Platform)
  slug: trust-protection-foundation-websdk
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venafi/refs/heads/main/openapi/venafi-trust-protection-foundation-websdk-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.venafi.com/Docs/currentSDK/TopNav/Content/SDK/AuthSDK/r-SDKa-OAuthScopePrivilegeMapping.php
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Venafi Scopes
name_suffix: OAuth Scopes
note: 'Two different authorization models. (1) The self-hosted Trust Protection Foundation WebSDK is a full OAuth 2.0 authorization server (POST /vedauth/authorize/oauth, /device, /jwt, /certificate, /integrated, /token, and DELETE /vedauth/revoke/token) and every operation in the published contract annotates its required scope in the operation description. Scopes take the form <scope>:<privilege> where privilege is one of manage, delete, discover, revoke, approve, read; a bare scope name grants read. The provider docs describe a client declaring, e.g., "scope: certificate:discover,delete,manage,revoke". (2) The SaaS Control Plane does NOT use OAuth scopes in its OpenAPI securitySchemes — it authenticates with the tppl-api-key header or a service-account bearer token, and the scope a service account may hold is enumerated at runtime from GET /v1/serviceaccounts/scopes. Counts below are the number of operations in the WebSDK contract that declare each scope.'
overview: 'Venafi uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Venafi
provider_slug: venafi
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: venafi-scopes
source_filename: venafi-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: openapi/venafi-trust-protection-foundation-websdk-openapi.yml (per-operation \"_Required\n  scope:_\" annotations) + openapi/venafi-certificate-manager-saas-openapi.yml\ndocs: https://docs.venafi.com/Docs/currentSDK/TopNav/Content/SDK/AuthSDK/r-SDKa-OAuthScopePrivilegeMapping.php\nnote: 'Two different authorization models. (1) The self-hosted Trust Protection Foundation WebSDK\n  is a full OAuth 2.0 authorization server (POST /vedauth/authorize/oauth, /device, /jwt,\n  /certificate, /integrated, /token, and DELETE /vedauth/revoke/token) and every operation in the\n  published contract annotates its required scope in the operation description. Scopes take the\n  form <scope>:<privilege> where privilege is one of manage, delete, discover, revoke, approve,\n  read; a bare scope name grants read. The provider docs describe a client declaring, e.g.,\n  \"scope: certificate:discover,delete,manage,revoke\". (2) The SaaS Control Plane\
  \ does NOT use\n  OAuth scopes in its OpenAPI securitySchemes — it authenticates with the tppl-api-key header or\n  a service-account bearer token, and the scope a service account may hold is enumerated at\n  runtime from GET /v1/serviceaccounts/scopes. Counts below are the number of operations in the\n  WebSDK contract that declare each scope.'\noauth:\n  authorization_server: self-hosted Trust Protection Foundation (/vedauth)\n  flows:\n  - authorization_code (POST /vedauth/authorize/oauth)\n  - device_code (POST /vedauth/authorize/device)\n  - jwt_bearer (POST /vedauth/authorize/jwt)\n  - client_certificate (POST /vedauth/authorize/certificate)\n  - integrated_windows_auth (POST /vedauth/authorize/integrated)\n  - refresh_token (POST /vedauth/authorize/token)\n  revocation: DELETE /vedauth/revoke/token\n  introspection: GET /vedauth/authorize/verify\nscopes:\n- name: any\n  description: Implicitly granted alongside any other valid scope; covers read-only system,\n    config-lookup,\
  \ metadata, log and workflow-ticket endpoints.\n  operations: 82\n- name: configuration\n  description: Read policy-tree configuration objects.\n  operations: 40\n- name: configuration:manage\n  description: Create, update and move configuration objects and policy folders.\n  operations: 35\n- name: configuration:delete\n  description: Delete configuration objects.\n  operations: 8\n- name: admin\n  description: Platform administration — engines, upgrades, system settings.\n  operations: 33\n- name: admin:recyclebin\n  description: Read and restore items from the recycle bin.\n  operations: 10\n- name: admin:algorithms\n  description: Manage the algorithm selector.\n  operations: 1\n- name: admin:rotate\n  description: Key/secret rotation administration.\n  operations: 1\n- name: certificate\n  description: Read certificate objects and their details.\n  operations: 17\n- name: certificate:manage\n  description: Request, renew, retry, import and provision certificates.\n  operations: 15\n\
  - name: certificate:delete\n  description: Delete certificate objects.\n  operations: 2\n- name: certificate:discover\n  description: Run and manage certificate discovery jobs.\n  operations: 2\n- name: certificate:revoke\n  description: Revoke issued certificates.\n  operations: 1\n- name: codesign\n  description: Read Code Sign Manager projects, applications, environments and templates.\n  operations: 16\n- name: codesign:manage\n  description: Create and update code-signing projects, environments and applications.\n  operations: 20\n- name: codesign:admin\n  description: Code Signing Administrator operations, including HSM configuration.\n  operations: 9\n- name: codesign:delete\n  description: Delete code-signing objects.\n  operations: 5\n- name: codesign:approve\n  description: Approve code-signing requests.\n  operations: 2\n- name: codesignclient\n  description: Client-side signing scope (API/Sign, API/SignJWT, GPG public key retrieval).\n  operations: 10\n- name: security\n  description:\
  \ Read identity, credential and permission security objects.\n  operations: 13\n- name: security:manage\n  description: Manage credentials, identities and permissions.\n  operations: 15\n- name: security:delete\n  description: Delete credentials and security objects.\n  operations: 4\n- name: restricted\n  description: Read access to restricted objects (SecretStore and similar).\n  operations: 10\n- name: restricted:manage\n  description: Manage restricted objects.\n  operations: 7\n- name: restricted:delete\n  description: Delete restricted objects.\n  operations: 2\n- name: statistics\n  description: Read platform statistics.\n  operations: 5\n- name: statistics:manage\n  description: Manage statistics collection.\n  operations: 3\n- name: statistics:delete\n  description: Delete statistics.\n  operations: 1\n- name: agent\n  description: Client/agent registration and management.\n  operations: 3\n- name: agent:delete\n  description: Delete agent registrations.\n  operations: 1\n- name:\
  \ ssh\n  description: SSH key and SSH certificate management.\n  operations: 1\n- name: ':manage'\n  description: 'Published verbatim in the contract as \"_Required scope: :manage_\" with an empty\n    scope prefix. The provider''s own scope map documents this as the \"any\" scope carrying the\n    Manage privilege (POST Log, POST Metadata/Set). Recorded as published — a consumer reading\n    only the OpenAPI cannot resolve it.'\n  operations: 11\n- name: ':approve'\n  description: 'Published verbatim as \"_Required scope: :approve_\"; the scope map documents it as\n    the \"any\" scope carrying the Approve privilege (Flow/Tickets/Approve, Flow/Tickets/Reject,\n    Workflow/Ticket/UpdateStatus).'\n  operations: 4\nsaas_service_account_scopes:\n  discovery: GET /v1/serviceaccounts/scopes\n  note: The SaaS contract enumerates scopes at runtime rather than listing them statically; the\n    published schema examples name \"distributed-issuance\" and \"certificate-issuance\" with an\n    authenticationType\
  \ (e.g. rsaKey) per scope.\n  observed_in_spec:\n  - distributed-issuance\n  - certificate-issuance\nsummary:\n  scope_count: 33\n  source_operations_annotated: 388\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/venafi/refs/heads/main/scopes/venafi-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Security
- Certificates
- PKI
- Machine Identity
- Identity
- Cryptography
- Key Management
- Certificate Lifecycle Management
- DevOps
- Kubernetes
- Code Signing
token_urls: []
---
