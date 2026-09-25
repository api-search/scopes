---
authorization_urls: []
description: ''
docs: https://buf.build/docs/bsr/apis/mcp/
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Buf Scopes
name_suffix: OAuth Scopes
note: 'Derived from the provider''s own RFC 8414 and RFC 9728 discovery documents, both fetched anonymously and saved verbatim under well-known/. There is no broader scope catalogue: the BSR''s non-MCP surface uses unscoped user API tokens, so this file describes the whole of Buf''s OAuth scope surface rather than a subset of it.'
overview: 'Buf uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Buf
provider_slug: buf
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: buf-scopes
source_filename: buf-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: https://buf.build/.well-known/oauth-authorization-server\ndocs: https://buf.build/docs/bsr/apis/mcp/\nauthorization_server: https://buf.build\nprotected_resources:\n  - resource: https://buf.build/mcp\n    metadata: https://buf.build/.well-known/oauth-protected-resource/mcp\n    scopes_supported: [mcp]\n    bearer_methods_supported: [header]\nflows:\n  authorization_code:\n    authorization_endpoint: https://buf.build/oauth2/authorize\n    token_endpoint: https://buf.build/oauth2/token\n    pkce: S256\n    dynamic_client_registration: https://buf.build/oauth2/register\nscopes:\n  - name: mcp\n    description: >-\n      The only scope the BSR authorization server advertises. Granting it lets an MCP\n      client call the BSR Registry API as the approving user. It is NOT a read-only or\n      least-privilege scope: Buf's docs state the resulting token \"has the same access as\n      the user who approved it ... including writes.\"\
  \n    read_only: false\n    source: https://buf.build/.well-known/oauth-authorization-server\nscope_count: 1\nnote: >-\n  Derived from the provider's own RFC 8414 and RFC 9728 discovery documents, both fetched\n  anonymously and saved verbatim under well-known/. There is no broader scope catalogue:\n  the BSR's non-MCP surface uses unscoped user API tokens, so this file describes the\n  whole of Buf's OAuth scope surface rather than a subset of it.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buf/refs/heads/main/scopes/buf-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Code Generation
- gRPC
- Kafka
- Open Source
- Protocol Buffers
- Schema Registry
- SDK
- Streaming
token_urls: []
---
