---
api_specs:
- filename: fluence-openapi-original.yml
  format: yaml
  label: Fluence API
  slug: fluence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fluence/refs/heads/main/openapi/fluence-openapi-original.yml
authorization_urls: []
description: ''
docs: https://console.fluence.network/settings/api-keys
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Fluence Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Fluence publishes 34 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Fluence API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Fluence
provider_slug: fluence
schemes: []
scope_count: 34
scope_names:
- vms:read
- vms:write
- vm:create
- vm:remove
- vm:restart
- vm:update
- vm:list
- vm:request_access
- storage:read
- storage:write
- public_ip:read
- public_ip:write
- subnet:read
- subnet:write
- vpc:read
- vpc:write
- security_groups:read
- security_groups:write
- ssh_key:create
- ssh_key:remove
- ssh_key:activate
- ssh_key:deactivate
- ssh_key:list
- clusters:read
- prices:read
- token:deposit
- token:withdraw
- billing:top_up
- billing:get_history
- billing:get_spending_history
- billing:get_spending_aggregated
- api_key:create
- api_key:remove
- api_key:list
scopes:
- description: List and read virtual machines.
  flows: []
  scope: vms:read
- description: Create, update, restart, and terminate virtual machines.
  flows: []
  scope: vms:write
- description: Create a virtual machine.
  flows: []
  scope: vm:create
- description: Terminate a virtual machine.
  flows: []
  scope: vm:remove
- description: Restart a virtual machine.
  flows: []
  scope: vm:restart
- description: Update a virtual machine.
  flows: []
  scope: vm:update
- description: List virtual machines.
  flows: []
  scope: vm:list
- description: Request access to a virtual machine.
  flows: []
  scope: vm:request_access
- description: List and read storage volumes.
  flows: []
  scope: storage:read
- description: Create, update, and delete storage volumes.
  flows: []
  scope: storage:write
- description: List and read public IPs.
  flows: []
  scope: public_ip:read
- description: Allocate, update, and release public IPs.
  flows: []
  scope: public_ip:write
- description: List and read subnets.
  flows: []
  scope: subnet:read
- description: Create, update, and delete subnets.
  flows: []
  scope: subnet:write
- description: List and read VPCs.
  flows: []
  scope: vpc:read
- description: Create, update, and delete VPCs.
  flows: []
  scope: vpc:write
- description: List and read security groups.
  flows: []
  scope: security_groups:read
- description: Create, update, and delete security groups.
  flows: []
  scope: security_groups:write
- description: Create an SSH key.
  flows: []
  scope: ssh_key:create
- description: Delete an SSH key.
  flows: []
  scope: ssh_key:remove
- description: Activate an SSH key.
  flows: []
  scope: ssh_key:activate
- description: Deactivate an SSH key.
  flows: []
  scope: ssh_key:deactivate
- description: List SSH keys.
  flows: []
  scope: ssh_key:list
- description: Read available compute clusters.
  flows: []
  scope: clusters:read
- description: Read compute, storage, and public-IP prices.
  flows: []
  scope: prices:read
- description: Deposit tokens to the account balance.
  flows: []
  scope: token:deposit
- description: Withdraw tokens from the account balance.
  flows: []
  scope: token:withdraw
- description: Create a balance top-up.
  flows: []
  scope: billing:top_up
- description: Read top-up history.
  flows: []
  scope: billing:get_history
- description: Read spending (charge) history.
  flows: []
  scope: billing:get_spending_history
- description: Read aggregated spending.
  flows: []
  scope: billing:get_spending_aggregated
- description: Create API keys.
  flows: []
  scope: api_key:create
- description: Delete API keys.
  flows: []
  scope: api_key:remove
- description: List API keys.
  flows: []
  scope: api_key:list
slug: fluence-scopes
source_filename: fluence-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/fluence-openapi-original.yml\ndocs: https://console.fluence.network/settings/api-keys\n# Fluence is NOT OAuth2. API keys (X-API-KEY) carry a set of permission scopes\n# (components.schemas.PermissionScope). These are the API-key permission scopes, not\n# OAuth grant scopes. Admin-only scopes (admin:*) are internal and not grantable to\n# ordinary API keys; they are listed under admin_scopes for completeness.\nscheme:\n  type: apiKey\n  in: header\n  name: X-API-KEY\nscopes:\n  - scope: vms:read\n    description: List and read virtual machines.\n  - scope: vms:write\n    description: Create, update, restart, and terminate virtual machines.\n  - scope: vm:create\n    description: Create a virtual machine.\n  - scope: vm:remove\n    description: Terminate a virtual machine.\n  - scope: vm:restart\n    description: Restart a virtual machine.\n  - scope: vm:update\n    description: Update a virtual machine.\n  - scope: vm:list\n\
  \    description: List virtual machines.\n  - scope: vm:request_access\n    description: Request access to a virtual machine.\n  - scope: storage:read\n    description: List and read storage volumes.\n  - scope: storage:write\n    description: Create, update, and delete storage volumes.\n  - scope: public_ip:read\n    description: List and read public IPs.\n  - scope: public_ip:write\n    description: Allocate, update, and release public IPs.\n  - scope: subnet:read\n    description: List and read subnets.\n  - scope: subnet:write\n    description: Create, update, and delete subnets.\n  - scope: vpc:read\n    description: List and read VPCs.\n  - scope: vpc:write\n    description: Create, update, and delete VPCs.\n  - scope: security_groups:read\n    description: List and read security groups.\n  - scope: security_groups:write\n    description: Create, update, and delete security groups.\n  - scope: ssh_key:create\n    description: Create an SSH key.\n  - scope: ssh_key:remove\n    description:\
  \ Delete an SSH key.\n  - scope: ssh_key:activate\n    description: Activate an SSH key.\n  - scope: ssh_key:deactivate\n    description: Deactivate an SSH key.\n  - scope: ssh_key:list\n    description: List SSH keys.\n  - scope: clusters:read\n    description: Read available compute clusters.\n  - scope: prices:read\n    description: Read compute, storage, and public-IP prices.\n  - scope: token:deposit\n    description: Deposit tokens to the account balance.\n  - scope: token:withdraw\n    description: Withdraw tokens from the account balance.\n  - scope: billing:top_up\n    description: Create a balance top-up.\n  - scope: billing:get_history\n    description: Read top-up history.\n  - scope: billing:get_spending_history\n    description: Read spending (charge) history.\n  - scope: billing:get_spending_aggregated\n    description: Read aggregated spending.\n  - scope: api_key:create\n    description: Create API keys.\n  - scope: api_key:remove\n    description: Delete API keys.\n \
  \ - scope: api_key:list\n    description: List API keys.\nadmin_scopes:\n  note: >-\n    Internal administrative scopes present in the PermissionScope enum (not grantable to\n    ordinary API keys): admin:users:*, admin:vms:*, admin:invites:*, admin:peers:*,\n    admin:default_images:*, admin:promo_codes:*, admin:basic_configuration:*,\n    admin:payment_methods:*, admin:payments:read, admin:security_groups:*, admin:storages:*,\n    admin:subnets:*, admin:public_ips:*, admin:vpcs:*, admin:clusters:*, admin:prices:*,\n    and the marketplace-backend scopes akash:* and spheron:*.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fluence/refs/heads/main/scopes/fluence-scopes.yml
summary_line: 34 scopes
tags:
- Company
- Crypto Web3
- Cloud Compute
- DePIN
- GPU
- Infrastructure
- Virtual Machines
- AI Infrastructure
- Decentralized Cloud
token_urls: []
---
