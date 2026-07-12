---
authorization_urls: []
description: ''
docs: https://docs.redhat.com/en/documentation/red_hat_insights/1-latest/html/using_the_red_hat_insights_api/apis-authentication
flows:
- password
kind: oauth-scopes
layout: scope
method: searched
name: Rhel Scopes
name_suffix: OAuth Scopes
note: api.console is the only OAuth scope Red Hat documents for its APIs; console.redhat.com access control is RBAC-based, and the Subscription Management API instead uses an offline-token refresh flow (client_id rhsm-api) with no scopes per https://access.redhat.com/articles/3626371.
overview: 'Red Hat Enterprise Linux publishes 1 OAuth 2.0 scope via the password flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Red Hat Enterprise Linux API on a user''s behalf.


  Tokens are issued from https://sso.redhat.com/auth/realms/redhat-external/protocol/openid-connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Red Hat Enterprise Linux
provider_slug: rhel
schemes:
- flows:
  - flow: password
    tokenUrl: https://sso.redhat.com/auth/realms/redhat-external/protocol/openid-connect/token
  name: OAuth2
  source: openapi/rhel-subscription-management-openapi.yml
scope_count: 1
scope_names:
- api.console
scopes:
- description: Grants a service account access to Red Hat Hybrid Cloud Console APIs (Insights, Compliance, Vulnerability, Patch, Inventory, Remediations) via the client_credentials grant against the Red Hat SSO token endpoint; fine-grained permissions are managed through Hybrid Cloud Console User Access (RBAC) groups rather than additional OAuth scopes.
  flows: []
  scope: api.console
slug: rhel-scopes
source_filename: rhel-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\nsource: openapi/rhel-subscription-management-openapi.yml\ndocs: https://docs.redhat.com/en/documentation/red_hat_insights/1-latest/html/using_the_red_hat_insights_api/apis-authentication\nschemes:\n- name: OAuth2\n  source: openapi/rhel-subscription-management-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: https://sso.redhat.com/auth/realms/redhat-external/protocol/openid-connect/token\nscopes:\n- scope: api.console\n  description: Grants a service account access to Red Hat Hybrid Cloud Console APIs\n    (Insights, Compliance, Vulnerability, Patch, Inventory, Remediations) via the\n    client_credentials grant against the Red Hat SSO token endpoint; fine-grained\n    permissions are managed through Hybrid Cloud Console User Access (RBAC) groups\n    rather than additional OAuth scopes.\n  sources:\n  - https://docs.redhat.com/en/documentation/red_hat_insights/1-latest/html/using_the_red_hat_insights_api/apis-authentication\n\
  note: api.console is the only OAuth scope Red Hat documents for its APIs; console.redhat.com\n  access control is RBAC-based, and the Subscription Management API instead uses\n  an offline-token refresh flow (client_id rhsm-api) with no scopes per https://access.redhat.com/articles/3626371.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rhel/refs/heads/main/scopes/rhel-scopes.yml
summary_line: 1 scope · password
tags:
- Automation
- Compliance
- Enterprise
- Linux
- Operating System
- Red Hat
- RHEL
- Security
- Subscription Management
- Vulnerability Management
token_urls:
- https://sso.redhat.com/auth/realms/redhat-external/protocol/openid-connect/token
---
