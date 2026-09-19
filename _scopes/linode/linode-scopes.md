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
  label: linode Instances API
  slug: linode-linode-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linode/refs/heads/main/openapi/linode-linode-instances-api-openapi.yml
- filename: linode-linode-kubernetes-engine-lke-api-openapi.yml
  format: yaml
  label: linode Kubernetes Engine (LKE) API
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
docs: https://techdocs.akamai.com/linode-api/reference/get-started#oauth-reference
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Linode Scopes
name_suffix: OAuth Scopes
note: 'Union of the scopes Akamai documents in the OAuth reference table and the scopes the first-party OpenAPI declares on its oauth securityScheme. They do not agree in either direction, which is the finding: the documented table carries databases:read_only and databases:read_write, which the contract does not declare, and the contract declares vpc:read_only, which the table does not list. An application requesting scopes from either source alone gets an incomplete or invalid set.'
overview: 'Linode publishes 30 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Linode API on a user''s behalf.


  Tokens are issued from https://login.linode.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Linode
provider_slug: linode
schemes:
- description: OAuth 2.0 authentication for third-party applications.
  flows:
  - authorizationUrl: https://login.linode.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://login.linode.com/oauth/token
  name: oauth
  source: openapi/linode-account-api-openapi.yml
- description: OAuth 2.0 authentication for third-party applications.
  flows:
  - authorizationUrl: https://login.linode.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://login.linode.com/oauth/token
  name: oauth
  source: openapi/linode-databases-api-openapi.yml
- description: OAuth 2.0 authentication for third-party applications.
  flows:
  - authorizationUrl: https://login.linode.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://login.linode.com/oauth/token
  name: oauth
  source: openapi/linode-domains-api-openapi.yml
- description: OAuth 2.0 authentication for third-party applications.
  flows:
  - authorizationUrl: https://login.linode.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://login.linode.com/oauth/token
  name: oauth
  source: openapi/linode-images-api-openapi.yml
- description: OAuth 2.0 authentication for third-party applications.
  flows:
  - authorizationUrl: https://login.linode.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://login.linode.com/oauth/token
  name: oauth
  source: openapi/linode-linode-instances-api-openapi.yml
- description: OAuth 2.0 authentication for third-party applications.
  flows:
  - authorizationUrl: https://login.linode.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://login.linode.com/oauth/token
  name: oauth
  source: openapi/linode-linode-kubernetes-engine-lke-api-openapi.yml
- description: OAuth 2.0 authentication for third-party applications.
  flows:
  - authorizationUrl: https://login.linode.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://login.linode.com/oauth/token
  name: oauth
  source: openapi/linode-longview-api-openapi.yml
- description: OAuth 2.0 authentication for third-party applications.
  flows:
  - authorizationUrl: https://login.linode.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://login.linode.com/oauth/token
  name: oauth
  source: openapi/linode-managed-api-openapi.yml
- description: OAuth 2.0 authentication for third-party applications.
  flows:
  - authorizationUrl: https://login.linode.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://login.linode.com/oauth/token
  name: oauth
  source: openapi/linode-networking-api-openapi.yml
- description: OAuth 2.0 authentication for third-party applications.
  flows:
  - authorizationUrl: https://login.linode.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://login.linode.com/oauth/token
  name: oauth
  source: openapi/linode-nodebalancers-api-openapi.yml
- description: OAuth 2.0 authentication for third-party applications.
  flows:
  - authorizationUrl: https://login.linode.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://login.linode.com/oauth/token
  name: oauth
  source: openapi/linode-object-storage-api-openapi.yml
- description: OAuth 2.0 authentication for third-party applications.
  flows:
  - authorizationUrl: https://login.linode.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://login.linode.com/oauth/token
  name: oauth
  source: openapi/linode-placement-groups-api-openapi.yml
- description: OAuth 2.0 authentication for third-party applications.
  flows:
  - authorizationUrl: https://login.linode.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://login.linode.com/oauth/token
  name: oauth
  source: openapi/linode-profile-api-openapi.yml
- description: OAuth 2.0 authentication for third-party applications.
  flows:
  - authorizationUrl: https://login.linode.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://login.linode.com/oauth/token
  name: oauth
  source: openapi/linode-regions-api-openapi.yml
- description: OAuth 2.0 authentication for third-party applications.
  flows:
  - authorizationUrl: https://login.linode.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://login.linode.com/oauth/token
  name: oauth
  source: openapi/linode-stackscripts-api-openapi.yml
- description: OAuth 2.0 authentication for third-party applications.
  flows:
  - authorizationUrl: https://login.linode.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://login.linode.com/oauth/token
  name: oauth
  source: openapi/linode-support-api-openapi.yml
- description: OAuth 2.0 authentication for third-party applications.
  flows:
  - authorizationUrl: https://login.linode.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://login.linode.com/oauth/token
  name: oauth
  source: openapi/linode-tags-api-openapi.yml
- description: OAuth 2.0 authentication for third-party applications.
  flows:
  - authorizationUrl: https://login.linode.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://login.linode.com/oauth/token
  name: oauth
  source: openapi/linode-volumes-api-openapi.yml
- description: OAuth 2.0 authentication for third-party applications.
  flows:
  - authorizationUrl: https://login.linode.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://login.linode.com/oauth/token
  name: oauth
  source: openapi/linode-vpcs-api-openapi.yml
scope_count: 30
scope_names:
- account:read_only
- account:read_write
- databases:read_only
- databases:read_write
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
- description: Allows access to GET information about your account.
  flows:
  - authorizationCode
  scope: account:read_only
- description: Allows access to all operations related to your account.
  flows:
  - authorizationCode
  scope: account:read_write
- description: Allows access to GET managed databases on your account.
  flows:
  - authorizationCode
  scope: databases:read_only
- description: Allows access to all operations related to your Managed Database.
  flows:
  - authorizationCode
  scope: databases:read_write
- description: Allows access to GET DNS Manager domains on your account.
  flows:
  - authorizationCode
  scope: domains:read_only
- description: Allows access to all DNS Manager domain operations.
  flows:
  - authorizationCode
  scope: domains:read_write
- description: Allows access to GET your events.
  flows:
  - authorizationCode
  scope: events:read_only
- description: Allows access to all operations related to your events.
  flows:
  - authorizationCode
  scope: events:read_write
- description: Allows access to GET information about your Cloud Firewalls.
  flows:
  - authorizationCode
  scope: firewall:read_only
- description: Allows access to all Cloud Firewall operations.
  flows:
  - authorizationCode
  scope: firewall:read_write
- description: Allows access to GET your Image Servicesimages.
  flows:
  - authorizationCode
  scope: images:read_only
- description: Allows access to all operations related to your Image Servicesimages.
  flows:
  - authorizationCode
  scope: images:read_write
- description: Allows access to GET your IPs.
  flows:
  - authorizationCode
  scope: ips:read_only
- description: Allows access to all operations related to your IPs.
  flows:
  - authorizationCode
  scope: ips:read_write
- description: Allows access to GET Linodes on your account.
  flows:
  - authorizationCode
  scope: linodes:read_only
- description: Allow access to all operations related to your Linodes.
  flows:
  - authorizationCode
  scope: linodes:read_write
- description: Allows access to GET LKE clusters on your account.
  flows:
  - authorizationCode
  scope: lke:read_only
- description: Allows access to all operations related to LKE clusters on your account.
  flows:
  - authorizationCode
  scope: lke:read_write
- description: Allows access to GET your Longview clients.
  flows:
  - authorizationCode
  scope: longview:read_only
- description: Allows access to all operations related to your Longview clients.
  flows:
  - authorizationCode
  scope: longview:read_write
- description: Allows access to GET NodeBalancers on your account.
  flows:
  - authorizationCode
  scope: nodebalancers:read_only
- description: Allows access to all NodeBalancer operations.
  flows:
  - authorizationCode
  scope: nodebalancers:read_write
- description: Allows access to GET information related to your Object Storage.
  flows:
  - authorizationCode
  scope: object_storage:read_only
- description: Allows access to all Object Storage operations.
  flows:
  - authorizationCode
  scope: object_storage:read_write
- description: Allows access to GET your StackScripts.
  flows:
  - authorizationCode
  scope: stackscripts:read_only
- description: Allows access to all operations related to your StackScripts.
  flows:
  - authorizationCode
  scope: stackscripts:read_write
- description: Allows access to GET your volumes.
  flows:
  - authorizationCode
  scope: volumes:read_only
- description: Allows access to all operations related to your volumes.
  flows:
  - authorizationCode
  scope: volumes:read_write
- description: Read access to VPCs
  flows:
  - authorizationCode
  scope: vpc:read_only
- description: Allows access to all operations related to VPC and subnet creation, updating, and deletion
  flows:
  - authorizationCode
  scope: vpc:read_write
slug: linode-scopes
source_filename: linode-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: searched\nsource: https://techdocs.akamai.com/linode-api/reference/get-started#oauth-reference\ndocs: https://techdocs.akamai.com/linode-api/reference/get-started#oauth-reference\nderived_from: openapi/_original/linode-api-v4-official-openapi.json (components.securitySchemes.oauth)\nprovider: Linode (Akamai Cloud)\nproviderId: linode\nnote: 'Union of the scopes Akamai documents in the OAuth reference table and the scopes the first-party OpenAPI\n  declares on its oauth securityScheme. They do not agree in either direction, which is the finding: the documented\n  table carries databases:read_only and databases:read_write, which the contract does not declare, and the contract\n  declares vpc:read_only, which the table does not list. An application requesting scopes from either source alone\n  gets an incomplete or invalid set.'\nschemes:\n- name: oauth\n  source: openapi/linode-account-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n \
  \   authorizationUrl: https://login.linode.com/oauth/authorize\n    tokenUrl: https://login.linode.com/oauth/token\n  description: OAuth 2.0 authentication for third-party applications.\n- name: oauth\n  source: openapi/linode-databases-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.linode.com/oauth/authorize\n    tokenUrl: https://login.linode.com/oauth/token\n  description: OAuth 2.0 authentication for third-party applications.\n- name: oauth\n  source: openapi/linode-domains-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.linode.com/oauth/authorize\n    tokenUrl: https://login.linode.com/oauth/token\n  description: OAuth 2.0 authentication for third-party applications.\n- name: oauth\n  source: openapi/linode-images-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.linode.com/oauth/authorize\n    tokenUrl: https://login.linode.com/oauth/token\n  description:\
  \ OAuth 2.0 authentication for third-party applications.\n- name: oauth\n  source: openapi/linode-linode-instances-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.linode.com/oauth/authorize\n    tokenUrl: https://login.linode.com/oauth/token\n  description: OAuth 2.0 authentication for third-party applications.\n- name: oauth\n  source: openapi/linode-linode-kubernetes-engine-lke-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.linode.com/oauth/authorize\n    tokenUrl: https://login.linode.com/oauth/token\n  description: OAuth 2.0 authentication for third-party applications.\n- name: oauth\n  source: openapi/linode-longview-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.linode.com/oauth/authorize\n    tokenUrl: https://login.linode.com/oauth/token\n  description: OAuth 2.0 authentication for third-party applications.\n- name: oauth\n  source: openapi/linode-managed-api-openapi.yml\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.linode.com/oauth/authorize\n    tokenUrl: https://login.linode.com/oauth/token\n  description: OAuth 2.0 authentication for third-party applications.\n- name: oauth\n  source: openapi/linode-networking-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.linode.com/oauth/authorize\n    tokenUrl: https://login.linode.com/oauth/token\n  description: OAuth 2.0 authentication for third-party applications.\n- name: oauth\n  source: openapi/linode-nodebalancers-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.linode.com/oauth/authorize\n    tokenUrl: https://login.linode.com/oauth/token\n  description: OAuth 2.0 authentication for third-party applications.\n- name: oauth\n  source: openapi/linode-object-storage-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.linode.com/oauth/authorize\n    tokenUrl:\
  \ https://login.linode.com/oauth/token\n  description: OAuth 2.0 authentication for third-party applications.\n- name: oauth\n  source: openapi/linode-placement-groups-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.linode.com/oauth/authorize\n    tokenUrl: https://login.linode.com/oauth/token\n  description: OAuth 2.0 authentication for third-party applications.\n- name: oauth\n  source: openapi/linode-profile-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.linode.com/oauth/authorize\n    tokenUrl: https://login.linode.com/oauth/token\n  description: OAuth 2.0 authentication for third-party applications.\n- name: oauth\n  source: openapi/linode-regions-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.linode.com/oauth/authorize\n    tokenUrl: https://login.linode.com/oauth/token\n  description: OAuth 2.0 authentication for third-party applications.\n- name:\
  \ oauth\n  source: openapi/linode-stackscripts-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.linode.com/oauth/authorize\n    tokenUrl: https://login.linode.com/oauth/token\n  description: OAuth 2.0 authentication for third-party applications.\n- name: oauth\n  source: openapi/linode-support-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.linode.com/oauth/authorize\n    tokenUrl: https://login.linode.com/oauth/token\n  description: OAuth 2.0 authentication for third-party applications.\n- name: oauth\n  source: openapi/linode-tags-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.linode.com/oauth/authorize\n    tokenUrl: https://login.linode.com/oauth/token\n  description: OAuth 2.0 authentication for third-party applications.\n- name: oauth\n  source: openapi/linode-volumes-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.linode.com/oauth/authorize\n\
  \    tokenUrl: https://login.linode.com/oauth/token\n  description: OAuth 2.0 authentication for third-party applications.\n- name: oauth\n  source: openapi/linode-vpcs-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.linode.com/oauth/authorize\n    tokenUrl: https://login.linode.com/oauth/token\n  description: OAuth 2.0 authentication for third-party applications.\nauthorization_url: https://login.linode.com/oauth/authorize\ntoken_url: https://login.linode.com/oauth/token\ntoken_ttl: access_token expires in two hours; the private (confidential) client flow issues a refresh_token, the\n  public client flow does not\nscope_count: 30\ndocumented_count: 29\ncontract_count: 28\ndiscrepancies:\n  documented_not_in_contract:\n  - databases:read_only\n  - databases:read_write\n  in_contract_not_documented:\n  - vpc:read_only\nscopes:\n- scope: account:read_only\n  description: Allows access to GET information about your account.\n  flows:\n  - authorizationCode\n\
  \  in_contract: true\n  in_docs: true\n  sources:\n  - https://techdocs.akamai.com/linode-api/reference/get-started#oauth-reference\n  - openapi/_original/linode-api-v4-official-openapi.json\n- scope: account:read_write\n  description: Allows access to all operations related to your account.\n  flows:\n  - authorizationCode\n  in_contract: true\n  in_docs: true\n  sources:\n  - https://techdocs.akamai.com/linode-api/reference/get-started#oauth-reference\n  - openapi/_original/linode-api-v4-official-openapi.json\n- scope: databases:read_only\n  description: Allows access to GET managed databases on your account.\n  flows:\n  - authorizationCode\n  in_contract: false\n  in_docs: true\n  sources:\n  - https://techdocs.akamai.com/linode-api/reference/get-started#oauth-reference\n  note: Documented by Akamai but not declared in the OpenAPI securityScheme.\n- scope: databases:read_write\n  description: Allows access to all operations related to your Managed Database.\n  flows:\n  - authorizationCode\n\
  \  in_contract: false\n  in_docs: true\n  sources:\n  - https://techdocs.akamai.com/linode-api/reference/get-started#oauth-reference\n  note: Documented by Akamai but not declared in the OpenAPI securityScheme.\n- scope: domains:read_only\n  description: Allows access to GET DNS Manager domains on your account.\n  flows:\n  - authorizationCode\n  in_contract: true\n  in_docs: true\n  sources:\n  - https://techdocs.akamai.com/linode-api/reference/get-started#oauth-reference\n  - openapi/_original/linode-api-v4-official-openapi.json\n- scope: domains:read_write\n  description: Allows access to all DNS Manager domain operations.\n  flows:\n  - authorizationCode\n  in_contract: true\n  in_docs: true\n  sources:\n  - https://techdocs.akamai.com/linode-api/reference/get-started#oauth-reference\n  - openapi/_original/linode-api-v4-official-openapi.json\n- scope: events:read_only\n  description: Allows access to GET your events.\n  flows:\n  - authorizationCode\n  in_contract: true\n  in_docs:\
  \ true\n  sources:\n  - https://techdocs.akamai.com/linode-api/reference/get-started#oauth-reference\n  - openapi/_original/linode-api-v4-official-openapi.json\n- scope: events:read_write\n  description: Allows access to all operations related to your events.\n  flows:\n  - authorizationCode\n  in_contract: true\n  in_docs: true\n  sources:\n  - https://techdocs.akamai.com/linode-api/reference/get-started#oauth-reference\n  - openapi/_original/linode-api-v4-official-openapi.json\n- scope: firewall:read_only\n  description: Allows access to GET information about your Cloud Firewalls.\n  flows:\n  - authorizationCode\n  in_contract: true\n  in_docs: true\n  sources:\n  - https://techdocs.akamai.com/linode-api/reference/get-started#oauth-reference\n  - openapi/_original/linode-api-v4-official-openapi.json\n- scope: firewall:read_write\n  description: Allows access to all Cloud Firewall operations.\n  flows:\n  - authorizationCode\n  in_contract: true\n  in_docs: true\n  sources:\n  - https://techdocs.akamai.com/linode-api/reference/get-started#oauth-reference\n\
  \  - openapi/_original/linode-api-v4-official-openapi.json\n- scope: images:read_only\n  description: Allows access to GET your Image Servicesimages.\n  flows:\n  - authorizationCode\n  in_contract: true\n  in_docs: true\n  sources:\n  - https://techdocs.akamai.com/linode-api/reference/get-started#oauth-reference\n  - openapi/_original/linode-api-v4-official-openapi.json\n- scope: images:read_write\n  description: Allows access to all operations related to your Image Servicesimages.\n  flows:\n  - authorizationCode\n  in_contract: true\n  in_docs: true\n  sources:\n  - https://techdocs.akamai.com/linode-api/reference/get-started#oauth-reference\n  - openapi/_original/linode-api-v4-official-openapi.json\n- scope: ips:read_only\n  description: Allows access to GET your IPs.\n  flows:\n  - authorizationCode\n  in_contract: true\n  in_docs: true\n  sources:\n  - https://techdocs.akamai.com/linode-api/reference/get-started#oauth-reference\n  - openapi/_original/linode-api-v4-official-openapi.json\n\
  - scope: ips:read_write\n  description: Allows access to all operations related to your IPs.\n  flows:\n  - authorizationCode\n  in_contract: true\n  in_docs: true\n  sources:\n  - https://techdocs.akamai.com/linode-api/reference/get-started#oauth-reference\n  - openapi/_original/linode-api-v4-official-openapi.json\n- scope: linodes:read_only\n  description: Allows access to GET Linodes on your account.\n  flows:\n  - authorizationCode\n  in_contract: true\n  in_docs: true\n  sources:\n  - https://techdocs.akamai.com/linode-api/reference/get-started#oauth-reference\n  - openapi/_original/linode-api-v4-official-openapi.json\n- scope: linodes:read_write\n  description: Allow access to all operations related to your Linodes.\n  flows:\n  - authorizationCode\n  in_contract: true\n  in_docs: true\n  sources:\n  - https://techdocs.akamai.com/linode-api/reference/get-started#oauth-reference\n  - openapi/_original/linode-api-v4-official-openapi.json\n- scope: lke:read_only\n  description: Allows\
  \ access to GET LKE clusters on your account.\n  flows:\n  - authorizationCode\n  in_contract: true\n  in_docs: true\n  sources:\n  - https://techdocs.akamai.com/linode-api/reference/get-started#oauth-reference\n  - openapi/_original/linode-api-v4-official-openapi.json\n- scope: lke:read_write\n  description: Allows access to all operations related to LKE clusters on your account.\n  flows:\n  - authorizationCode\n  in_contract: true\n  in_docs: true\n  sources:\n  - https://techdocs.akamai.com/linode-api/reference/get-started#oauth-reference\n  - openapi/_original/linode-api-v4-official-openapi.json\n- scope: longview:read_only\n  description: Allows access to GET your Longview clients.\n  flows:\n  - authorizationCode\n  in_contract: true\n  in_docs: true\n  sources:\n  - https://techdocs.akamai.com/linode-api/reference/get-started#oauth-reference\n  - openapi/_original/linode-api-v4-official-openapi.json\n- scope: longview:read_write\n  description: Allows access to all operations related\
  \ to your Longview clients.\n  flows:\n  - authorizationCode\n  in_contract: true\n  in_docs: true\n  sources:\n  - https://techdocs.akamai.com/linode-api/reference/get-started#oauth-reference\n  - openapi/_original/linode-api-v4-official-openapi.json\n- scope: nodebalancers:read_only\n  description: Allows access to GET NodeBalancers on your account.\n  flows:\n  - authorizationCode\n  in_contract: true\n  in_docs: true\n  sources:\n  - https://techdocs.akamai.com/linode-api/reference/get-started#oauth-reference\n  - openapi/_original/linode-api-v4-official-openapi.json\n- scope: nodebalancers:read_write\n  description: Allows access to all NodeBalancer operations.\n  flows:\n  - authorizationCode\n  in_contract: true\n  in_docs: true\n  sources:\n  - https://techdocs.akamai.com/linode-api/reference/get-started#oauth-reference\n  - openapi/_original/linode-api-v4-official-openapi.json\n- scope: object_storage:read_only\n  description: Allows access to GET information related to your Object\
  \ Storage.\n  flows:\n  - authorizationCode\n  in_contract: true\n  in_docs: true\n  sources:\n  - https://techdocs.akamai.com/linode-api/reference/get-started#oauth-reference\n  - openapi/_original/linode-api-v4-official-openapi.json\n- scope: object_storage:read_write\n  description: Allows access to all Object Storage operations.\n  flows:\n  - authorizationCode\n  in_contract: true\n  in_docs: true\n  sources:\n  - https://techdocs.akamai.com/linode-api/reference/get-started#oauth-reference\n  - openapi/_original/linode-api-v4-official-openapi.json\n- scope: stackscripts:read_only\n  description: Allows access to GET your StackScripts.\n  flows:\n  - authorizationCode\n  in_contract: true\n  in_docs: true\n  sources:\n  - https://techdocs.akamai.com/linode-api/reference/get-started#oauth-reference\n  - openapi/_original/linode-api-v4-official-openapi.json\n- scope: stackscripts:read_write\n  description: Allows access to all operations related to your StackScripts.\n  flows:\n  - authorizationCode\n\
  \  in_contract: true\n  in_docs: true\n  sources:\n  - https://techdocs.akamai.com/linode-api/reference/get-started#oauth-reference\n  - openapi/_original/linode-api-v4-official-openapi.json\n- scope: volumes:read_only\n  description: Allows access to GET your volumes.\n  flows:\n  - authorizationCode\n  in_contract: true\n  in_docs: true\n  sources:\n  - https://techdocs.akamai.com/linode-api/reference/get-started#oauth-reference\n  - openapi/_original/linode-api-v4-official-openapi.json\n- scope: volumes:read_write\n  description: Allows access to all operations related to your volumes.\n  flows:\n  - authorizationCode\n  in_contract: true\n  in_docs: true\n  sources:\n  - https://techdocs.akamai.com/linode-api/reference/get-started#oauth-reference\n  - openapi/_original/linode-api-v4-official-openapi.json\n- scope: vpc:read_only\n  description: Read access to VPCs\n  flows:\n  - authorizationCode\n  in_contract: true\n  in_docs: false\n  sources:\n  - openapi/_original/linode-api-v4-official-openapi.json\n\
  \  note: Declared in the OpenAPI securityScheme but absent from the documented scope table.\n- scope: vpc:read_write\n  description: Allows access to all operations related to VPC and subnet creation, updating, and deletion\n  flows:\n  - authorizationCode\n  in_contract: true\n  in_docs: true\n  sources:\n  - https://techdocs.akamai.com/linode-api/reference/get-started#oauth-reference\n  - openapi/_original/linode-api-v4-official-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linode/refs/heads/main/scopes/linode-scopes.yml
summary_line: 30 scopes · authorizationCode
tags:
- Cloud Computing
- Infrastructure-as-a-Service
- Virtual Machines
- Kubernetes
- Object Storage
- Block Storage
- DNS
- Managed Database
- Networking
- GPU
- Load Balancer
- Developer Tools
token_urls:
- https://login.linode.com/oauth/token
---
