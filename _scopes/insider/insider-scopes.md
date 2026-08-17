---
api_specs:
- filename: insider-unification-openapi.yml
  format: yaml
  label: Insider One Unification API
  slug: insider-one-unification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-unification-openapi.yml
- filename: insider-contact-openapi.yml
  format: yaml
  label: Insider One Contact API
  slug: insider-one-contact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-contact-openapi.yml
- filename: insider-mail-openapi.yml
  format: yaml
  label: Insider One Mail API
  slug: insider-one-mail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-mail-openapi.yml
- filename: insider-sms-openapi.yml
  format: yaml
  label: Insider One SMS API
  slug: insider-one-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-sms-openapi.yml
- filename: insider-whatsapp-openapi.yml
  format: yaml
  label: Insider One WhatsApp API
  slug: insider-one-whatsapp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-whatsapp-openapi.yml
- filename: insider-gateway-openapi.yml
  format: yaml
  label: Insider One Gateway API (OAuth 2.0)
  slug: insider-one-gateway-api-oauth-20
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-gateway-openapi.yml
- filename: insider-web-push-openapi.yml
  format: yaml
  label: Insider One Web Push API
  slug: insider-one-web-push-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-web-push-openapi.yml
- filename: insider-mobile-openapi.yml
  format: yaml
  label: Insider One Mobile App API
  slug: insider-one-mobile-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-mobile-openapi.yml
- filename: insider-mobile-settings-openapi.yml
  format: yaml
  label: Insider One Mobile Settings API
  slug: insider-one-mobile-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-mobile-settings-openapi.yml
- filename: insider-live-activity-openapi.yml
  format: yaml
  label: Insider One Live Activity API
  slug: insider-one-live-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-live-activity-openapi.yml
- filename: insider-verify-openapi.yml
  format: yaml
  label: Insider One Verify (OTP) API
  slug: insider-one-verify-otp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-verify-openapi.yml
- filename: insider-catalog-openapi.yml
  format: yaml
  label: Insider One Catalog API
  slug: insider-one-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-catalog-openapi.yml
- filename: insider-recommendation-openapi.yml
  format: yaml
  label: Insider One Recommendation API
  slug: insider-one-recommendation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-recommendation-openapi.yml
- filename: insider-eureka-search-openapi.yml
  format: yaml
  label: Insider One Eureka Search API
  slug: insider-one-eureka-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-eureka-search-openapi.yml
- filename: insider-eureka-events-openapi.yml
  format: yaml
  label: Insider One Eureka Event Collection API
  slug: insider-one-eureka-event-collection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-eureka-events-openapi.yml
- filename: insider-analytics-openapi.yml
  format: yaml
  label: Insider One Analytics API
  slug: insider-one-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-analytics-openapi.yml
- filename: insider-architect-analytics-openapi.yml
  format: yaml
  label: Insider One Architect Analytics API
  slug: insider-one-architect-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-architect-analytics-openapi.yml
- filename: insider-architect-transactional-openapi.yml
  format: yaml
  label: Insider One Architect Transactional Journey API
  slug: insider-one-architect-transactional-journey-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-architect-transactional-openapi.yml
authorization_urls:
- https://gw.useinsider.com/oauth2/authorize
description: ''
docs: https://academy.insiderone.com/docs/set-up-insider-one-mcp
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Insider Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Insider uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://gw.useinsider.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Insider
provider_slug: insider
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://gw.useinsider.com/oauth2/token
  - authorizationUrl: https://gw.useinsider.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://gw.useinsider.com/oauth2/token
  name: OAuth2
  pkce:
  - S256
  revocation_endpoint: https://gw.useinsider.com/oauth2/revoke
  source: openapi/insider-gateway-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: insider-scopes
source_filename: insider-scopes.yml
source_heading: OAuth Scopes
source_url: https://academy.insiderone.com/docs/set-up-insider-one-mcp
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://academy.insiderone.com/docs/set-up-insider-one-mcp\ndocs: https://academy.insiderone.com/docs/set-up-insider-one-mcp\nsources:\n- https://academy.insiderone.com/docs/set-up-insider-one-mcp\n- https://academy.insiderone.com/docs/insider-one-mcp-functions\n- https://gw.useinsider.com/.well-known/oauth-authorization-server\n- https://mcp.insiderone.com/.well-known/oauth-protected-resource\n- openapi/insider-gateway-openapi.yml\nauthorization_server: https://gw.useinsider.com\nprotected_resource: https://gw.useinsider.com\nscope_model: >-\n  Insider One issues OAuth 2.0 credentials from the InOne panel (Settings > InOne Settings >\n  Integration Settings > OAuth 2.0 Credentials) and the operator SELECTS SCOPES AT GENERATION TIME,\n  one per channel. Insider One states plainly that \"a tool is available only if the corresponding\n  scope is included in the credential\", so the scope set is the access-control boundary for\
  \ both the\n  gateway API and the MCP server.\npublished_scope_names: false\npublished_scope_names_note: >-\n  The RFC 9728 protected-resource document advertises scopes_supported: [\"*\"] — a wildcard, not a\n  list. Insider One does not publish the concrete scope strings anywhere public; they are only\n  visible in the credential-generation screen. The channel-level GRANULARITY below is documented in\n  the MCP setup and functions pages; the literal scope tokens are NOT, and are deliberately not\n  guessed here.\n\nschemes:\n- name: OAuth2\n  source: openapi/insider-gateway-openapi.yml\n  flows:\n  - {flow: clientCredentials, tokenUrl: 'https://gw.useinsider.com/oauth2/token'}\n  - {flow: authorizationCode, authorizationUrl: 'https://gw.useinsider.com/oauth2/authorize', tokenUrl: 'https://gw.useinsider.com/oauth2/token'}\n  pkce: [S256]\n  revocation_endpoint: https://gw.useinsider.com/oauth2/revoke\n\nscopes: []\n\nscope_dimensions:\n- {dimension: channel, values: [Email, SMS, WhatsApp,\
  \ Web Push, Mobile App, Architect], evidence: 'MCP setup page: \"Select the scopes you want to grant. For full MCP functionality, enable all available channels.\"'}\n- {dimension: access, values: [read, write], evidence: 'MCP functions page: 28 read-only tools and 7 write tools, with write tools defaulting to needs-approval.'}\n- {dimension: excluded, values: [OnSite], evidence: 'MCP functions page: \"On-site is currently unsupported.\"'}\n\nguidance:\n- Create a dedicated OAuth 2.0 credential for each client (Insider One explicitly recommends against\n  reusing credentials for MCP).\n- The Client Secret is displayed once.\n- Access tokens live up to 90 minutes; the refresh_token grant is supported.\n\ngaps:\n- No public scope reference page; scopes_supported is a wildcard.\n- No OpenID Connect discovery document, so no scopes_supported from that direction either.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/scopes/insider-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Customer Engagement
- Personalization
- Customer Data Platform
- Marketing
- Journey Orchestration
- Omnichannel
- CDP
- Artificial Intelligence
- Messaging
- WhatsApp
- Email
- SMS
- Push Notifications
- Recommendations
- Search
- Product Catalog
- Analytics
- MCP
- Agents
- Consent
- GDPR
token_urls:
- https://gw.useinsider.com/oauth2/token
---
