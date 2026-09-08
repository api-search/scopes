---
api_specs:
- filename: calico-bgpconfiguration-api-openapi.yml
  format: yaml
  label: Calico BGPConfiguration API
  slug: calico-bgpconfiguration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calico/refs/heads/main/openapi/calico-bgpconfiguration-api-openapi.yml
- filename: calico-bgppeer-api-openapi.yml
  format: yaml
  label: Calico BGPPeer API
  slug: calico-bgppeer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calico/refs/heads/main/openapi/calico-bgppeer-api-openapi.yml
- filename: calico-globalnetworkpolicy-api-openapi.yml
  format: yaml
  label: Calico GlobalNetworkPolicy API
  slug: calico-globalnetworkpolicy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calico/refs/heads/main/openapi/calico-globalnetworkpolicy-api-openapi.yml
- filename: calico-hostendpoint-api-openapi.yml
  format: yaml
  label: Calico HostEndpoint API
  slug: calico-hostendpoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calico/refs/heads/main/openapi/calico-hostendpoint-api-openapi.yml
- filename: calico-ippool-api-openapi.yml
  format: yaml
  label: Calico IPPool API
  slug: calico-ippool-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calico/refs/heads/main/openapi/calico-ippool-api-openapi.yml
- filename: calico-networkpolicy-api-openapi.yml
  format: yaml
  label: Calico NetworkPolicy API
  slug: calico-networkpolicy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calico/refs/heads/main/openapi/calico-networkpolicy-api-openapi.yml
- filename: calico-profile-api-openapi.yml
  format: yaml
  label: Calico Profile API
  slug: calico-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calico/refs/heads/main/openapi/calico-profile-api-openapi.yml
authorization_urls: []
description: OAuth scope surface reachable from this record. The Calico API itself (projectcalico.org/v3) does NOT use OAuth — it authenticates with Kubernetes bearer tokens or client certificates and authorizes with Kubernetes RBAC, so it has no scope vocabulary at all (see authentication/calico-authentication.yml). The only OAuth authorization server on a host in this record is Tigera's, which fronts the remote MCP server in mcp/calico-mcp.yml.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Calico Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Calico uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Calico
provider_slug: calico
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: calico-scopes
source_filename: calico-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: https://www.tigera.io/.well-known/oauth-authorization-server/\ndescription: >-\n  OAuth scope surface reachable from this record. The Calico API itself (projectcalico.org/v3) does\n  NOT use OAuth — it authenticates with Kubernetes bearer tokens or client certificates and\n  authorizes with Kubernetes RBAC, so it has no scope vocabulary at all (see\n  authentication/calico-authentication.yml). The only OAuth authorization server on a host in this\n  record is Tigera's, which fronts the remote MCP server in mcp/calico-mcp.yml.\nauthorization_server: https://www.tigera.io\nmetadata_document: https://www.tigera.io/.well-known/oauth-authorization-server/\nprotected_resource: https://www.tigera.io/wp-json/mcp/mcp-oauth-server\nflows:\n- type: authorization_code\n  pkce_required_methods: [S256]\n  token_endpoint_auth_methods: [none]\n  dynamic_registration: client_id_metadata_document\nscopes:\n- name: mcp\n  description: >-\n    The\
  \ single scope advertised in scopes_supported. Grants access to the Tigera MCP server. The\n    provider publishes no scopes reference page, so no finer-grained description is available and\n    none has been invented.\n  source: scopes_supported in the RFC 8414 metadata document\nscope_count: 1\ndocs: null\nnotes:\n- >-\n  Calico API authorization is Kubernetes RBAC, expressed as ClusterRole/Role rules over the\n  projectcalico.org API group (verbs get/list/watch/create/update/patch/delete on resources such as\n  networkpolicies, globalnetworkpolicies, ippools, bgppeers, hostendpoints, tiers). That is a real\n  permission model, but it is not an OAuth scope model and is deliberately not transcribed here as\n  one.\n- >-\n  This file is derived from a discovery document that was actually fetched. derive-oauth-scopes.py\n  found zero oauth2 securitySchemes in openapi/ and correctly wrote nothing.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/calico/refs/heads/main/scopes/calico-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- CNI
- Containers
- eBPF
- Kubernetes
- Network Policy
- Network Security
- Networking
- Open-Source
- Service Mesh
token_urls: []
---
