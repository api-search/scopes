---
api_specs:
- filename: ifs-finance-api-openapi.yml
  format: yaml
  label: IFS Finance API
  slug: ifs-finance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ifs/refs/heads/main/openapi/ifs-finance-api-openapi.yml
- filename: ifs-inventory-api-openapi.yml
  format: yaml
  label: IFS Inventory API
  slug: ifs-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ifs/refs/heads/main/openapi/ifs-inventory-api-openapi.yml
- filename: ifs-procurement-api-openapi.yml
  format: yaml
  label: IFS Procurement API
  slug: ifs-procurement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ifs/refs/heads/main/openapi/ifs-procurement-api-openapi.yml
- filename: ifs-work-orders-api-openapi.yml
  format: yaml
  label: IFS Work Orders API
  slug: ifs-work-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ifs/refs/heads/main/openapi/ifs-work-orders-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.ifs.com/techdocs/26r1/030_administration/010_security/020_permission_sets/004_permission_set_overview/010_projections/
flows:
- clientCredentials
- authorizationCode
- authorizationCode+PKCE
- password
kind: oauth-scopes
layout: scope
method: searched
name: Ifs Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'IFS publishes 2 OAuth 2.0 scopes via the clientCredentials, authorizationCode, authorizationCode+PKCE, and password flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the IFS API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: IFS
provider_slug: ifs
schemes:
- flows:
  - clientCredentials
  - authorizationCode
  - authorizationCode+PKCE
  - password
  name: IFS IAM (OpenID Connect)
  token_endpoint: https://<SYSTEM_URL>/auth/realms/<NAMESPACE>/protocol/openid-connect/token
scope_count: 2
scope_names:
- openid
- microprofile-jwt
scopes:
- description: Standard OpenID Connect scope. Required on the token request for external integration clients.
  flows:
  - clientCredentials
  - authorizationCode
  - authorizationCode+PKCE
  - password
  scope: openid
- description: Requests the MicroProfile JWT claim set IFS Cloud uses for role-based access. Required alongside `openid` on the token request.
  flows:
  - clientCredentials
  - authorizationCode
  - authorizationCode+PKCE
  - password
  scope: microprofile-jwt
slug: ifs-scopes
source_filename: ifs-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: searched\nsource: https://docs.ifs.com/techdocs/26r1/030_administration/010_security/040_iam_settings/035_iam_clients/020_authenticate_external_integration/300_client_credential_flow/\ndocs: https://docs.ifs.com/techdocs/26r1/030_administration/010_security/020_permission_sets/004_permission_set_overview/010_projections/\nsupersedes:\n  previous_method: derived\n  previous_source: openapi/ifs-cloud-erp-openapi.yml\n  reason: >-\n    The previous derived file listed scopes `ifs.read` and `ifs.write` against\n    https://login.ifs.cloud/oauth2/authorize. That host does not resolve (DNS NXDOMAIN,\n    probed 2026-09-13) and IFS documents neither scope name. The values below are the ones\n    IFS publishes.\nsummary: >-\n  IFS Cloud does NOT express API authorization as OAuth scopes. The OIDC token request\n  carries a fixed protocol scope set; what an integration is actually allowed to do is\n  decided by IFS Cloud permission sets and projection\
  \ grants attached to the service user,\n  not by scope strings. Treat the scope list below as the complete published set — it is\n  short because the model is role-based, not scope-based.\nmodel: permission-sets\nschemes:\n- name: IFS IAM (OpenID Connect)\n  token_endpoint: https://<SYSTEM_URL>/auth/realms/<NAMESPACE>/protocol/openid-connect/token\n  flows:\n  - clientCredentials\n  - authorizationCode\n  - authorizationCode+PKCE\n  - password\nscopes:\n- scope: openid\n  description: Standard OpenID Connect scope. Required on the token request for external integration clients.\n  required: true\n  flows: [clientCredentials, authorizationCode, authorizationCode+PKCE, password]\n  source: https://docs.ifs.com/techdocs/26r1/030_administration/010_security/040_iam_settings/035_iam_clients/020_authenticate_external_integration/300_client_credential_flow/\n- scope: microprofile-jwt\n  description: >-\n    Requests the MicroProfile JWT claim set IFS Cloud uses for role-based access. Required\n\
  \    alongside `openid` on the token request.\n  required: true\n  flows: [clientCredentials, authorizationCode, authorizationCode+PKCE, password]\n  source: https://docs.ifs.com/techdocs/26r1/030_administration/010_security/040_iam_settings/035_iam_clients/020_authenticate_external_integration/300_client_credential_flow/\nscopes_returned_in_token:\n  observed: openid audience microprofile-jwt email profile\n  note: >-\n    The scope string IFS shows in its documented sample token response. `audience`, `email`\n    and `profile` are returned by the authorization server; only `openid microprofile-jwt`\n    is documented as required on the request.\nauthorization_beyond_scopes:\n- mechanism: Permission sets\n  description: Projection grants, per-page and per-navigator grants, and per-projection access levels granted to the user or service user.\n  docs: https://docs.ifs.com/techdocs/26r1/030_administration/010_security/020_permission_sets/011_creating_permission_sets/010_projections/\n-\
  \ mechanism: Access Control Lists (ACL)\n  description: ACLs applied at projection level; projections can also be excluded outright.\n  docs: https://docs.ifs.com/techdocs/26r1/030_administration/010_security/008_data_access_control/020_apply_acl_to_projection/\n- mechanism: StandardEntity activation\n  description: StandardEntity-class APIs require explicit activation by a system administrator before they can be used at all.\n  docs: https://docs.ifs.com/policy/APIUsageCloud.pdf\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ifs/refs/heads/main/scopes/ifs-scopes.yml
summary_line: 2 scopes · clientCredentials/authorizationCode/authorizationCode+PKCE/password
tags:
- ERP
- Field Service
- Asset Management
- Manufacturing
- Energy
- Cloud
- Sweden
token_urls: []
---
