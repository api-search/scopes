---
api_specs:
- filename: linode-account-api-openapi.yml
  format: yaml
  label: linode Account API
  slug: linode-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linode/refs/heads/main/openapi/linode-account-api-openapi.yml
- filename: linode-databases-api-openapi.yml
  format: yaml
  label: linode Databases API
  slug: linode-databases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linode/refs/heads/main/openapi/linode-databases-api-openapi.yml
- filename: linode-domains-api-openapi.yml
  format: yaml
  label: linode Domains API
  slug: linode-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linode/refs/heads/main/openapi/linode-domains-api-openapi.yml
- filename: linode-images-api-openapi.yml
  format: yaml
  label: linode Images API
  slug: linode-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linode/refs/heads/main/openapi/linode-images-api-openapi.yml
- filename: linode-linode-instances-api-openapi.yml
  format: yaml
  label: linode Linode Instances API
  slug: linode-linode-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linode/refs/heads/main/openapi/linode-linode-instances-api-openapi.yml
- filename: linode-linode-kubernetes-engine-lke-api-openapi.yml
  format: yaml
  label: linode Linode Kubernetes Engine (LKE) API
  slug: linode-linode-kubernetes-engine-lke-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linode/refs/heads/main/openapi/linode-linode-kubernetes-engine-lke-api-openapi.yml
- filename: linode-longview-api-openapi.yml
  format: yaml
  label: linode Longview API
  slug: linode-longview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linode/refs/heads/main/openapi/linode-longview-api-openapi.yml
- filename: linode-managed-api-openapi.yml
  format: yaml
  label: linode Managed API
  slug: linode-managed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linode/refs/heads/main/openapi/linode-managed-api-openapi.yml
- filename: linode-networking-api-openapi.yml
  format: yaml
  label: linode Networking API
  slug: linode-networking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linode/refs/heads/main/openapi/linode-networking-api-openapi.yml
- filename: linode-nodebalancers-api-openapi.yml
  format: yaml
  label: linode NodeBalancers API
  slug: linode-nodebalancers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linode/refs/heads/main/openapi/linode-nodebalancers-api-openapi.yml
- filename: linode-object-storage-api-openapi.yml
  format: yaml
  label: linode Object Storage API
  slug: linode-object-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linode/refs/heads/main/openapi/linode-object-storage-api-openapi.yml
- filename: linode-placement-groups-api-openapi.yml
  format: yaml
  label: linode Placement Groups API
  slug: linode-placement-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linode/refs/heads/main/openapi/linode-placement-groups-api-openapi.yml
- filename: linode-profile-api-openapi.yml
  format: yaml
  label: linode Profile API
  slug: linode-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linode/refs/heads/main/openapi/linode-profile-api-openapi.yml
- filename: linode-regions-api-openapi.yml
  format: yaml
  label: linode Regions API
  slug: linode-regions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linode/refs/heads/main/openapi/linode-regions-api-openapi.yml
- filename: linode-stackscripts-api-openapi.yml
  format: yaml
  label: linode StackScripts API
  slug: linode-stackscripts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linode/refs/heads/main/openapi/linode-stackscripts-api-openapi.yml
- filename: linode-support-api-openapi.yml
  format: yaml
  label: linode Support API
  slug: linode-support-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linode/refs/heads/main/openapi/linode-support-api-openapi.yml
- filename: linode-tags-api-openapi.yml
  format: yaml
  label: linode Tags API
  slug: linode-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linode/refs/heads/main/openapi/linode-tags-api-openapi.yml
- filename: linode-volumes-api-openapi.yml
  format: yaml
  label: linode Volumes API
  slug: linode-volumes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linode/refs/heads/main/openapi/linode-volumes-api-openapi.yml
- filename: linode-vpcs-api-openapi.yml
  format: yaml
  label: linode VPCs API
  slug: linode-vpcs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linode/refs/heads/main/openapi/linode-vpcs-api-openapi.yml
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
