---
api_specs:
- filename: complyadvantage-mesh-api-openapi.json
  format: json
  label: ComplyAdvantage Mesh Platform API
  slug: complyadvantage-mesh-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/complyadvantage/refs/heads/main/openapi/complyadvantage-mesh-api-openapi.json
- filename: complyadvantage-case-management-api-openapi.yml
  format: yaml
  label: ComplyAdvantage Case Management API
  slug: complyadvantage-case-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/complyadvantage/refs/heads/main/openapi/complyadvantage-case-management-api-openapi.yml
- filename: complyadvantage-monitored-searches-api-openapi.yml
  format: yaml
  label: ComplyAdvantage Monitored Searches API
  slug: complyadvantage-monitored-searches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/complyadvantage/refs/heads/main/openapi/complyadvantage-monitored-searches-api-openapi.yml
- filename: complyadvantage-searches-api-openapi.yml
  format: yaml
  label: ComplyAdvantage Searches API
  slug: complyadvantage-searches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/complyadvantage/refs/heads/main/openapi/complyadvantage-searches-api-openapi.yml
- filename: complyadvantage-users-api-openapi.yml
  format: yaml
  label: ComplyAdvantage Users API
  slug: complyadvantage-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/complyadvantage/refs/heads/main/openapi/complyadvantage-users-api-openapi.yml
authorization_urls: []
description: Mesh authenticates with an OAuth2 client-credentials token but does NOT use OAuth scopes. Authorization is carried by named account permissions attached to the role behind the API credential, and by coarser account-level entitlements that gate whole product areas. The Mesh API reference states the required permission on each endpoint in prose ("You need the 'View customers' permission to use this endpoint"), which makes the model fully documented but entirely invisible to a machine reading the OpenAPI - components.securitySchemes declares only an opaque http bearer scheme with no scope list, and no operation carries a per-operation security requirement. A caller cannot compute least privilege from the contract; it has to be read out of the docs, which is what this artifact does. Permissions are enumerable at runtime via GET /v3/iam/permissions.
docs: https://docs.mesh.complyadvantage.com/reference/identity_v2_iam_permissions_listpermissions
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Complyadvantage Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'ComplyAdvantage uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ComplyAdvantage
provider_slug: complyadvantage
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: complyadvantage-scopes
source_filename: complyadvantage-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: https://docs.mesh.complyadvantage.com/llms.txt\ndocs: https://docs.mesh.complyadvantage.com/reference/identity_v2_iam_permissions_listpermissions\nprovider: ComplyAdvantage\nproviderId: complyadvantage\nmodel: account-permissions\noauth_scopes_published: false\ndescription: >-\n  Mesh authenticates with an OAuth2 client-credentials token but does NOT use OAuth scopes.\n  Authorization is carried by named account permissions attached to the role behind the API\n  credential, and by coarser account-level entitlements that gate whole product areas. The\n  Mesh API reference states the required permission on each endpoint in prose (\"You need the\n  'View customers' permission to use this endpoint\"), which makes the model fully documented\n  but entirely invisible to a machine reading the OpenAPI - components.securitySchemes\n  declares only an opaque http bearer scheme with no scope list, and no operation carries a\n  per-operation\
  \ security requirement. A caller cannot compute least privilege from the\n  contract; it has to be read out of the docs, which is what this artifact does.\n  Permissions are enumerable at runtime via GET /v3/iam/permissions.\nauthorization_layers:\n- layer: account entitlement\n  description: >-\n    Product access sold at the account level. Gates whole capability families regardless of\n    the credential's permissions; a 403 here cannot be fixed by an administrator, only by a\n    contract change.\n  values:\n  - Access to base customer screening functionality\n  - Access to base customer monitoring functionality\n  - Access to base transaction monitoring functionality\n  - Access to base payment screening functionality\n  - Access to custom lists for customer screening\n  - Account has access to monitor on demand functionality\n  - Account has access to FinCEN CTR reports\n  - Account has access to FinCEN SAR reports\n- layer: role permission\n  description: >-\n    Granted on a role\
  \ in Settings > Access Management and inherited by the API credential.\n    This is the layer an administrator controls.\nenumeration:\n  operation: GET /v3/iam/permissions\n  deprecated_operation: GET /v2/iam/permissions\n  note: >-\n    The live permission list is retrievable from the API itself. The list below is what the\n    published reference names on at least one endpoint - it is the documented subset, not\n    necessarily the complete registry.\npermissions:\n- name: View customers\n  grants: Read customers, acquisition sources, notes, products, monitoring configuration, risk scores, screening certificates.\n  operations_documented: 12\n- name: Update customers\n  grants: Create customer notes, override risk score level, transition customer status.\n  operations_documented: 5\n- name: Create and screen customers\n  grants: The create-and-screen onboarding workflow, sync and async.\n  operations_documented: 4\n  requires_entitlement: Access to base customer screening functionality\n\
  - name: Manage customer custom fields\n  grants: Create and update customer custom-field definitions.\n  operations_documented: 2\n- name: Create and update labels\n  grants: Read and set customer labels.\n  operations_documented: 2\n- name: View customer monitoring status\n  grants: Read a customer's monitoring configuration.\n  operations_documented: 1\n- name: Monitor and unmonitor customers\n  grants: Set a customer's monitoring configuration.\n  operations_documented: 1\n  requires_entitlement: Access to base customer monitoring functionality\n- name: Create and update customer screening configurations\n  grants: Create and update entity-screening configurations.\n  operations_documented: 2\n- name: View cases (customer onboarding)\n  grants: Read cases raised by onboarding screening.\n- name: View cases (customer monitoring)\n  grants: Read cases raised by ongoing monitoring.\n- name: View cases (payment screening)\n  grants: Read cases raised by payment screening.\n- name: View\
  \ cases (transaction monitoring)\n  grants: Read cases raised by transaction monitoring.\n  operations_documented: 7\n  note: >-\n    Case read access is partitioned by the product that raised the case, so a\n    least-privilege agent reading only onboarding cases needs exactly one of the four.\n- name: Update cases\n  grants: Assign cases, transition case stage, leave notes - individually and in bulk (up to 100).\n  operations_documented: 5\n- name: Update case workflows\n  grants: Update case workflow definitions.\n  operations_documented: 1\n- name: View alerts\n  grants: Read alerts and alert notes.\n  operations_documented: 4\n- name: Update alerts\n  grants: Transition alert state.\n  operations_documented: 2\n- name: Update risks\n  grants: Change the status of a risk on an alert.\n  operations_documented: 1\n- name: Create and delete mutes\n  grants: Create and delete alert mutes (v2 and v3).\n  operations_documented: 4\n- name: View transactions\n  grants: Read transactions, versions,\
  \ and transaction custom fields.\n  operations_documented: 4\n  note: Appears in the reference in two casings, \"View transactions\" and \"View Transactions\".\n- name: View lookup lists\n  grants: Read lookup lists, versions and mappings.\n  operations_documented: 8\n- name: Create and update lookup lists\n  grants: Create, update and delete lookup lists, drafts and mappings.\n  operations_documented: 8\n- name: Create and update webhooks\n  grants: Create, update and test webhook notification configurations.\n  operations_documented: 3\n- name: View webhooks\n  grants: Read webhook notification configurations and their logs.\n  operations_documented: 1\n- name: Create and update email notification configurations\n  grants: Create, update, delete and test email notification configurations.\n  operations_documented: 4\n- name: View email notification configurations\n  grants: Read email notification configurations.\n  operations_documented: 1\n- name: View and download insights\n  grants:\
  \ Data exports.\n  operations_documented: 4\n- name: View users\n  grants: Read users on the account.\n  operations_documented: 3\n- name: Create and update users\n  grants: Create and update users.\n  operations_documented: 2\n- name: View roles in account\n  grants: Read roles.\n  operations_documented: 3\n- name: 'Create, update, and delete roles in account'\n  grants: Manage roles.\n  operations_documented: 3\n- name: Assign roles in account\n  grants: Assign roles to users.\n  operations_documented: 2\n- name: View all accounts\n  grants: Cross-account read for multi-account clients.\n  operations_documented: 2\n- name: Manage settings such as pre-fill data for FinCEN CTR reports\n  grants: Upsert and bulk-delete CTR transaction locations.\n  operations_documented: 2\n  requires_entitlement: Account has access to FinCEN CTR reports\n- name: Manage settings such as pre-fill data for FinCEN SAR reports\n  grants: Upsert and bulk-delete SAR financial institutions.\n  operations_documented:\
  \ 2\n  requires_entitlement: Account has access to FinCEN SAR reports\nlegacy_api:\n  model: none\n  note: >-\n    The legacy REST API (api.complyadvantage.com) has no scope or permission model in its\n    published reference - a single account API key carries whatever the account can do.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/complyadvantage/refs/heads/main/scopes/complyadvantage-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Anti-Money Laundering
- AML
- Fraud Detection
- Sanctions Screening
- Compliance
- PEP Screening
- Adverse Media
- KYC
- Watchlist
- Transaction Monitoring
- Financial Crime
- RegTech
token_urls: []
---
