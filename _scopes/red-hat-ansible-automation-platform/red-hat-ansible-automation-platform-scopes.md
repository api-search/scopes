---
api_specs:
- filename: red-hat-ansible-automation-platform-automation-controller-openapi.json
  format: json
  label: Red Hat Ansible Automation Controller API
  slug: controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-ansible-automation-platform/refs/heads/main/openapi/red-hat-ansible-automation-platform-automation-controller-openapi.json
- filename: red-hat-ansible-automation-platform-automation-hub-openapi.json
  format: json
  label: Red Hat Ansible Private Automation Hub API
  slug: private-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-ansible-automation-platform/refs/heads/main/openapi/red-hat-ansible-automation-platform-automation-hub-openapi.json
- filename: red-hat-ansible-automation-platform-event-driven-ansible-openapi.json
  format: json
  label: Red Hat Event-Driven Ansible Controller API
  slug: eda-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-ansible-automation-platform/refs/heads/main/openapi/red-hat-ansible-automation-platform-event-driven-ansible-openapi.json
- filename: red-hat-ansible-automation-platform-platform-gateway-openapi.json
  format: json
  label: Red Hat Ansible Automation Platform Gateway API
  slug: platform-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-ansible-automation-platform/refs/heads/main/openapi/red-hat-ansible-automation-platform-platform-gateway-openapi.json
- filename: red-hat-ansible-automation-platform-ansible-lightspeed-openapi.json
  format: json
  label: Red Hat Ansible Lightspeed with IBM watsonx Code Assistant API
  slug: ansible-lightspeed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-ansible-automation-platform/refs/heads/main/openapi/red-hat-ansible-automation-platform-ansible-lightspeed-openapi.json
- filename: red-hat-ansible-automation-platform-automation-hub-openapi.json
  format: json
  label: Red Hat Automation Hub API (Hybrid Cloud Console)
  slug: hosted-automation-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-ansible-automation-platform/refs/heads/main/openapi/red-hat-ansible-automation-platform-automation-hub-openapi.json
authorization_urls:
- /o/authorize/
description: ''
docs: ''
flows:
- authorizationCode
- password
kind: oauth-scopes
layout: scope
method: derived
name: Red Hat Ansible Automation Platform Scopes
name_suffix: OAuth Scopes
note: 'AAP''s OAuth scope surface is deliberately coarse: the Platform Gateway issues only `read` and `write`. Authorization is enforced by AAP RBAC AFTER the token is accepted (role definitions, role user/team assignments in the Gateway API), not by scope. An agent cannot request a least-privilege token for a single resource type — it gets read or write across everything the user can reach. Ansible Lightspeed adds a third scope, `delete`.'
overview: 'Red Hat Ansible Automation Platform publishes 3 OAuth 2.0 scopes via the authorizationCode and password flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Red Hat Ansible Automation Platform API on a user''s behalf.


  Tokens are issued from /o/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Red Hat Ansible Automation Platform
provider_slug: red-hat-ansible-automation-platform
schemes:
- flows:
  - authorizationUrl: /o/authorize/
    flow: authorizationCode
    tokenUrl: /o/token/
  name: oauth2
  source: openapi/red-hat-ansible-automation-platform-ansible-lightspeed-openapi.json
- flows:
  - authorizationUrl: /o/authorize/
    flow: authorizationCode
    tokenUrl: /o/token/
  - flow: password
    tokenUrl: /o/token/
  name: OAuth2_Authentication
  source: openapi/red-hat-ansible-automation-platform-platform-gateway-openapi.json
scope_count: 3
scope_names:
- delete
- read
- write
scopes:
- description: 'Ansible Lightspeed only: "Delete resources".'
  flows:
  - authorizationCode
  scope: delete
- description: 'Platform Gateway: "Read access to resources". Ansible Lightspeed: "Read basic user information".'
  flows:
  - authorizationCode
  - password
  scope: read
- description: 'Platform Gateway: "Write access to resources (includes read)". Ansible Lightspeed: "Request Ansible content suggestions".'
  flows:
  - authorizationCode
  - password
  scope: write
slug: red-hat-ansible-automation-platform-scopes
source_filename: red-hat-ansible-automation-platform-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: derived\nsource: openapi/red-hat-ansible-automation-platform-ansible-lightspeed-openapi.json, openapi/red-hat-ansible-automation-platform-platform-gateway-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/red-hat-ansible-automation-platform-ansible-lightspeed-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /o/authorize/\n    tokenUrl: /o/token/\n- name: OAuth2_Authentication\n  source: openapi/red-hat-ansible-automation-platform-platform-gateway-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /o/authorize/\n    tokenUrl: /o/token/\n  - flow: password\n    tokenUrl: /o/token/\nscopes:\n- scope: delete\n  description: 'Ansible Lightspeed only: \"Delete resources\".'\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/red-hat-ansible-automation-platform-ansible-lightspeed-openapi.json\n- scope: read\n  description: 'Platform Gateway: \"Read access to resources\". Ansible Lightspeed:\
  \ \"Read basic user information\".'\n  flows:\n  - authorizationCode\n  - password\n  sources:\n  - openapi/red-hat-ansible-automation-platform-ansible-lightspeed-openapi.json\n  - openapi/red-hat-ansible-automation-platform-platform-gateway-openapi.json\n- scope: write\n  description: 'Platform Gateway: \"Write access to resources (includes read)\". Ansible Lightspeed: \"Request\n    Ansible content suggestions\".'\n  flows:\n  - authorizationCode\n  - password\n  sources:\n  - openapi/red-hat-ansible-automation-platform-ansible-lightspeed-openapi.json\n  - openapi/red-hat-ansible-automation-platform-platform-gateway-openapi.json\nnote: 'AAP''s OAuth scope surface is deliberately coarse: the Platform Gateway issues only `read` and\n  `write`. Authorization is enforced by AAP RBAC AFTER the token is accepted (role definitions, role user/team\n  assignments in the Gateway API), not by scope. An agent cannot request a least-privilege token for a\n  single resource type — it gets read or\
  \ write across everything the user can reach. Ansible Lightspeed\n  adds a third scope, `delete`.'\nwarning: The Gateway declares BOTH authorizationCode and password (resource-owner) grants. The password\n  grant is removed in OAuth 2.1; recorded as a fact about the contract.\ntoken_endpoints:\n  authorization: https://{aap-gateway-host}/o/authorize/\n  token: https://{aap-gateway-host}/o/token/\nrelated:\n  authentication: authentication/red-hat-ansible-automation-platform-authentication.yml\n  rbac_operations:\n  - role_definitions_list\n  - role_user_assignments_list\n  - role_team_assignments_list\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/red-hat-ansible-automation-platform/refs/heads/main/scopes/red-hat-ansible-automation-platform-scopes.yml
summary_line: 3 scopes · authorizationCode/password
tags:
- Automation
- Configuration Management
- DevOps
- Enterprise
- Red Hat
- Ansible
- IT Operations
- Event-Driven Architecture
- Infrastructure as Code
- MCP
token_urls:
- /o/token/
---
