---
authorization_urls:
- https://login.linode.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Linode Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'linode publishes 28 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the linode API on a user''s behalf.


  Tokens are issued from https://login.linode.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: linode
provider_slug: linode
schemes:
- description: OAuth 2.0 authentication for third-party applications.
  flows:
  - authorizationUrl: https://login.linode.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://login.linode.com/oauth/token
  name: oauth
  source: openapi/linode-api-v4-openapi.yml
scope_count: 28
scope_names:
- account:read_only
- account:read_write
- domains:read_only
- domains:read_write
- events:read_only
- events:read_write
- firewall:read_only
- firewall:read_write
- images:read_only
- images:read_write
- ips:read_only
- ips:read_write
- linodes:read_only
- linodes:read_write
- lke:read_only
- lke:read_write
- longview:read_only
- longview:read_write
- nodebalancers:read_only
- nodebalancers:read_write
- object_storage:read_only
- object_storage:read_write
- stackscripts:read_only
- stackscripts:read_write
- volumes:read_only
- volumes:read_write
- vpc:read_only
- vpc:read_write
scopes:
- description: Read access to account information
  flows:
  - authorizationCode
  scope: account:read_only
- description: Read and write access to account information
  flows:
  - authorizationCode
  scope: account:read_write
- description: Read access to domains
  flows:
  - authorizationCode
  scope: domains:read_only
- description: Read and write access to domains
  flows:
  - authorizationCode
  scope: domains:read_write
- description: Read access to events
  flows:
  - authorizationCode
  scope: events:read_only
- description: Read and write access to events
  flows:
  - authorizationCode
  scope: events:read_write
- description: Read access to firewalls
  flows:
  - authorizationCode
  scope: firewall:read_only
- description: Read and write access to firewalls
  flows:
  - authorizationCode
  scope: firewall:read_write
- description: Read access to images
  flows:
  - authorizationCode
  scope: images:read_only
- description: Read and write access to images
  flows:
  - authorizationCode
  scope: images:read_write
- description: Read access to IP addresses
  flows:
  - authorizationCode
  scope: ips:read_only
- description: Read and write access to IP addresses
  flows:
  - authorizationCode
  scope: ips:read_write
- description: Read access to Linodes
  flows:
  - authorizationCode
  scope: linodes:read_only
- description: Read and write access to Linodes
  flows:
  - authorizationCode
  scope: linodes:read_write
- description: Read access to LKE
  flows:
  - authorizationCode
  scope: lke:read_only
- description: Read and write access to LKE
  flows:
  - authorizationCode
  scope: lke:read_write
- description: Read access to Longview
  flows:
  - authorizationCode
  scope: longview:read_only
- description: Read and write access to Longview
  flows:
  - authorizationCode
  scope: longview:read_write
- description: Read access to NodeBalancers
  flows:
  - authorizationCode
  scope: nodebalancers:read_only
- description: Read and write access to NodeBalancers
  flows:
  - authorizationCode
  scope: nodebalancers:read_write
- description: Read access to Object Storage
  flows:
  - authorizationCode
  scope: object_storage:read_only
- description: Read and write access to Object Storage
  flows:
  - authorizationCode
  scope: object_storage:read_write
- description: Read access to StackScripts
  flows:
  - authorizationCode
  scope: stackscripts:read_only
- description: Read and write access to StackScripts
  flows:
  - authorizationCode
  scope: stackscripts:read_write
- description: Read access to Volumes
  flows:
  - authorizationCode
  scope: volumes:read_only
- description: Read and write access to Volumes
  flows:
  - authorizationCode
  scope: volumes:read_write
- description: Read access to VPCs
  flows:
  - authorizationCode
  scope: vpc:read_only
- description: Read and write access to VPCs
  flows:
  - authorizationCode
  scope: vpc:read_write
slug: linode-scopes
source_filename: linode-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/linode-api-v4-openapi.yml\nschemes:\n- name: oauth\n  source: openapi/linode-api-v4-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.linode.com/oauth/authorize\n    tokenUrl: https://login.linode.com/oauth/token\n  description: OAuth 2.0 authentication for third-party applications.\nscopes:\n- scope: account:read_only\n  description: Read access to account information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/linode-api-v4-openapi.yml\n- scope: account:read_write\n  description: Read and write access to account information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/linode-api-v4-openapi.yml\n- scope: domains:read_only\n  description: Read access to domains\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/linode-api-v4-openapi.yml\n- scope: domains:read_write\n  description: Read and write access to domains\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/linode-api-v4-openapi.yml\n- scope: events:read_only\n  description: Read access to events\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/linode-api-v4-openapi.yml\n- scope: events:read_write\n  description: Read and write access to events\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/linode-api-v4-openapi.yml\n- scope: firewall:read_only\n  description: Read access to firewalls\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/linode-api-v4-openapi.yml\n- scope: firewall:read_write\n  description: Read and write access to firewalls\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/linode-api-v4-openapi.yml\n- scope: images:read_only\n  description: Read access to images\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/linode-api-v4-openapi.yml\n- scope: images:read_write\n  description: Read and write access to images\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/linode-api-v4-openapi.yml\n- scope: ips:read_only\n\
  \  description: Read access to IP addresses\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/linode-api-v4-openapi.yml\n- scope: ips:read_write\n  description: Read and write access to IP addresses\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/linode-api-v4-openapi.yml\n- scope: linodes:read_only\n  description: Read access to Linodes\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/linode-api-v4-openapi.yml\n- scope: linodes:read_write\n  description: Read and write access to Linodes\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/linode-api-v4-openapi.yml\n- scope: lke:read_only\n  description: Read access to LKE\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/linode-api-v4-openapi.yml\n- scope: lke:read_write\n  description: Read and write access to LKE\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/linode-api-v4-openapi.yml\n- scope: longview:read_only\n  description: Read access to Longview\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/linode-api-v4-openapi.yml\n- scope: longview:read_write\n  description: Read and write access to Longview\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/linode-api-v4-openapi.yml\n- scope: nodebalancers:read_only\n  description: Read access to NodeBalancers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/linode-api-v4-openapi.yml\n- scope: nodebalancers:read_write\n  description: Read and write access to NodeBalancers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/linode-api-v4-openapi.yml\n- scope: object_storage:read_only\n  description: Read access to Object Storage\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/linode-api-v4-openapi.yml\n- scope: object_storage:read_write\n  description: Read and write access to Object Storage\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/linode-api-v4-openapi.yml\n- scope: stackscripts:read_only\n  description: Read access to StackScripts\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/linode-api-v4-openapi.yml\n- scope: stackscripts:read_write\n  description: Read and write access to StackScripts\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/linode-api-v4-openapi.yml\n- scope: volumes:read_only\n  description: Read access to Volumes\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/linode-api-v4-openapi.yml\n- scope: volumes:read_write\n  description: Read and write access to Volumes\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/linode-api-v4-openapi.yml\n- scope: vpc:read_only\n  description: Read access to VPCs\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/linode-api-v4-openapi.yml\n- scope: vpc:read_write\n  description: Read and write access to VPCs\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/linode-api-v4-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linode/refs/heads/main/scopes/linode-scopes.yml
summary_line: 28 scopes · authorizationCode
tags: []
token_urls:
- https://login.linode.com/oauth/token
---
