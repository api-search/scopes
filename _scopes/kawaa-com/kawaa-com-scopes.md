---
api_specs:
- filename: kawaa-com-account-api-openapi.yml
  format: yaml
  label: kawaa-com Account API
  slug: kawaa-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kawaa-com/openapi/kawaa-com-account-api-openapi.yml
- filename: kawaa-com-activity-api-openapi.yml
  format: yaml
  label: kawaa-com Activity API
  slug: kawaa-com-activity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kawaa-com/openapi/kawaa-com-activity-api-openapi.yml
- filename: kawaa-com-api-keys-api-openapi.yml
  format: yaml
  label: kawaa-com API keys API
  slug: kawaa-com-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kawaa-com/openapi/kawaa-com-api-keys-api-openapi.yml
- filename: kawaa-com-catalogue-api-openapi.yml
  format: yaml
  label: kawaa-com Catalogue API
  slug: kawaa-com-catalogue-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kawaa-com/openapi/kawaa-com-catalogue-api-openapi.yml
- filename: kawaa-com-deliverability-api-openapi.yml
  format: yaml
  label: kawaa-com Deliverability API
  slug: kawaa-com-deliverability-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kawaa-com/openapi/kawaa-com-deliverability-api-openapi.yml
- filename: kawaa-com-exports-api-openapi.yml
  format: yaml
  label: kawaa-com Exports API
  slug: kawaa-com-exports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kawaa-com/openapi/kawaa-com-exports-api-openapi.yml
- filename: kawaa-com-health-api-openapi.yml
  format: yaml
  label: kawaa-com Health API
  slug: kawaa-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kawaa-com/openapi/kawaa-com-health-api-openapi.yml
- filename: kawaa-com-jobs-api-openapi.yml
  format: yaml
  label: kawaa-com Jobs API
  slug: kawaa-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kawaa-com/openapi/kawaa-com-jobs-api-openapi.yml
- filename: kawaa-com-search-api-openapi.yml
  format: yaml
  label: kawaa-com Search API
  slug: kawaa-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kawaa-com/openapi/kawaa-com-search-api-openapi.yml
- filename: kawaa-com-verification-api-openapi.yml
  format: yaml
  label: kawaa-com Verification API
  slug: kawaa-com-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kawaa-com/openapi/kawaa-com-verification-api-openapi.yml
- filename: kawaa-com-webhooks-api-openapi.yml
  format: yaml
  label: kawaa-com Webhooks API
  slug: kawaa-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kawaa-com/openapi/kawaa-com-webhooks-api-openapi.yml
authorization_urls:
- https://api.kawaa.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Kawaa Com Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'kawaa-com publishes 21 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the kawaa-com API on a user''s behalf.


  Tokens are issued from https://api.kawaa.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: kawaa-com
provider_slug: kawaa-com
schemes:
- description: 'OAuth 2.1 sign-in, for an app or agent that acts for a person who approves it on a Kawaa consent screen, instead of being handed an API key. The access token is sent as `Authorization: Bearer <token>`, the same header as `BearerToken`, and is checked exactly like a scoped API key: scopes, rate limits and credits apply unchanged.


    - **Discovery.** Authorization server metadata (RFC 8414): `https://api.kawaa.com/.well-known/oauth-authorization-server`. Protected resource metadata (RFC 9728): `https://api.kawaa.com/.well-known/oauth-protected-resource` for this API and `https://api.kawaa.com/.well-known/oauth-protected-resource/mcp` for the MCP server.

    - **Client.** Use the https URL of a Client ID Metadata Document, on the default port, as `client_id` (public clients only), or register at `https://api.kawaa.com/oauth/register` (RFC 7591; no credential needed). Registration follows the RFC defaults when a field is omitted: `token_endpoint_auth_method` `client_secret_basic` (a secret is issued) and `grant_types` `authorization_code` alone. Send `none` for a public client, and include `refresh_token` in `grant_types` to be issued refresh tokens. A redirect URI is https, loopback http (any port), or an app''s own scheme: a reversed domain name (RFC 8252 §7.1, `com.example.app:/callback`) or one of `cursor`, `vscode`, `vscode-insiders`, `claude` and `windsurf`. Browser and operating-system handler schemes are refused (`invalid_redirect_uri`).

    - **PKCE.** Required on every authorization request, with `code_challenge_method=S256`; no other method is accepted. The only grants are `authorization_code` and `refresh_token`.

    - **Resource.** Send `resource=https://api.kawaa.com` for this API (RFC 8707). Without it the token is issued for the MCP server, `https://api.kawaa.com/mcp`; any other value is refused with `invalid_target`.

    - **Scopes.** With no `scope` parameter the request is for `verification:write verification:read account:read analytics:read`. Scopes Kawaa does not define, and scopes a connected app can never hold, are dropped rather than refused; if none remain the request is refused with `invalid_scope`. An authorization request refused before the person answers it (`invalid_request`, `unsupported_response_type`, `invalid_target`, `invalid_scope`) is shown to them on a Kawaa error page carrying that code, and is not sent to the redirect URI (RFC 9700 §4.11.2); only their answer is, the code or `access_denied`, with `state` and `iss`. The person approving can untick any scope, and the token response''s `scope` states what was granted. `account:write`, `account:delete`, `billing:write`, `team:write`, `security:write` and `white_label:write` are never granted, so the operations that need them do not list this scheme, and neither do those marked `x-kawaa-unscoped-only`. As for API keys, `<area>:write`
    also satisfies `<area>:read`.

    - **Tokens.** An access token is `evo_` followed by 40 alphanumeric characters and lasts one hour (`expires_in: 3600`); after that the API answers 401 `OAUTH_TOKEN_EXPIRED`. A refresh token is `evr_` followed by 48 alphanumeric characters and is never accepted as a bearer credential. Every refresh returns a new refresh token and retires the one presented. The one just used may be presented up to 5 more times within 60 seconds of its use (a lost response, or several refreshes sent at once) and gets a new one of its own each time; the first of those to be used retires the rest. Presenting it again after that, or presenting any older refresh token, is treated as theft and ends the connection: its refresh tokens and every live access token stop working. A refresh may ask for fewer scopes than the connection holds, never more. A connection that is not refreshed for 30 days ends. Revoke at `https://api.kawaa.com/oauth/revoke` (RFC 7009).'
  flows:
  - authorizationUrl: https://api.kawaa.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.kawaa.com/oauth/token
  name: OAuth2
  source: openapi/kawaa-com-openapi.json
scope_count: 21
scope_names:
- account:read
- analytics:read
- analytics:write
- billing:read
- compose:read
- compose:write
- deliverability:read
- deliverability:write
- exports:read
- exports:write
- integrations:read
- integrations:write
- lists:read
- lists:write
- security:read
- team:read
- verification:read
- verification:write
- webhooks:read
- webhooks:write
- white_label:read
scopes:
- description: Read the account profile, credit balance and notifications.
  flows:
  - authorizationCode
  scope: account:read
- description: Read usage, analytics and tracking figures.
  flows:
  - authorizationCode
  scope: analytics:read
- description: Create, change and permanently delete tracking pixels and links, and record usage-analytics events for this account. Deleting a pixel or link breaks the tracking already embedded in sent mail. Credit alert thresholds are fixed, so no scope changes them.
  flows:
  - authorizationCode
  scope: analytics:write
- description: Read the subscription, invoices, payment methods and billing address.
  flows:
  - authorizationCode
  scope: billing:read
- description: Read AI composition history.
  flows:
  - authorizationCode
  scope: compose:read
- description: Generate and improve email copy with AI. Spends credits.
  flows:
  - authorizationCode
  scope: compose:write
- description: Read deliverability checks, blacklist and DMARC monitors, and inbox-placement and warmup state. Email warmup and inbox placement tests are not available yet.
  flows:
  - authorizationCode
  scope: deliverability:read
- description: Run deliverability checks and manage blacklist and DMARC monitors. Email warmup and inbox placement tests are not available yet; warmup campaigns and SMTP credentials already set up can still be removed.
  flows:
  - authorizationCode
  scope: deliverability:write
- description: Read exports, export schedules and data-sharing settings. Downloading an export also needs the scope that reads the data in it. Data sharing is not available yet.
  flows:
  - authorizationCode
  scope: exports:read
- description: 'Create and delete exports, manage export schedules and delivery destinations, and change export settings. Exported files contain customer addresses, so each kind of data also needs the scope that reads it: verification:read, account:read or security:read. Scheduled exports deliver by email, webhook or Amazon S3; Google Cloud Storage and Azure Blob Storage delivery is not available yet.'
  flows:
  - authorizationCode
  scope: exports:write
- description: Read connected integrations and their status.
  flows:
  - authorizationCode
  scope: integrations:read
- description: Connect and disconnect integrations, and push verification into them. The HubSpot, Salesforce and Mailchimp connections are not available yet.
  flows:
  - authorizationCode
  scope: integrations:write
- description: Read auto-clean lists and their run history.
  flows:
  - authorizationCode
  scope: lists:read
- description: Create, change, pause and delete auto-clean lists, and start rechecks. Each rechecked address spends one credit. Creating, reactivating and starting rechecks require Professional or above and account execution availability.
  flows:
  - authorizationCode
  scope: lists:write
- description: Read security settings, sessions, login history and the audit log.
  flows:
  - authorizationCode
  scope: security:read
- description: Read the team, its members and its invitations.
  flows:
  - authorizationCode
  scope: team:read
- description: Read verification results and jobs this account has already paid for. Spends nothing.
  flows:
  - authorizationCode
  scope: verification:read
- description: 'Anything that spends verification credits: verifying an address, a batch or a file, finding a business email, and the domain and address-history lookups, which are charged too.'
  flows:
  - authorizationCode
  scope: verification:write
- description: Read webhook endpoints and their delivery logs.
  flows:
  - authorizationCode
  scope: webhooks:read
- description: Create, change and delete webhook endpoints, and rotate their signing secrets.
  flows:
  - authorizationCode
  scope: webhooks:write
- description: Read white-label configuration, sub-accounts and the custom API domain.
  flows:
  - authorizationCode
  scope: white_label:read
slug: kawaa-com-scopes
source_filename: kawaa-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/kawaa-com-openapi.json\nschemes:\n- name: OAuth2\n  source: openapi/kawaa-com-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.kawaa.com/oauth/authorize\n    tokenUrl: https://api.kawaa.com/oauth/token\n  description: |-\n    OAuth 2.1 sign-in, for an app or agent that acts for a person who approves it on a Kawaa consent screen, instead of being handed an API key. The access token is sent as `Authorization: Bearer <token>`, the same header as `BearerToken`, and is checked exactly like a scoped API key: scopes, rate limits and credits apply unchanged.\n\n    - **Discovery.** Authorization server metadata (RFC 8414): `https://api.kawaa.com/.well-known/oauth-authorization-server`. Protected resource metadata (RFC 9728): `https://api.kawaa.com/.well-known/oauth-protected-resource` for this API and `https://api.kawaa.com/.well-known/oauth-protected-resource/mcp` for the MCP server.\n\
  \    - **Client.** Use the https URL of a Client ID Metadata Document, on the default port, as `client_id` (public clients only), or register at `https://api.kawaa.com/oauth/register` (RFC 7591; no credential needed). Registration follows the RFC defaults when a field is omitted: `token_endpoint_auth_method` `client_secret_basic` (a secret is issued) and `grant_types` `authorization_code` alone. Send `none` for a public client, and include `refresh_token` in `grant_types` to be issued refresh tokens. A redirect URI is https, loopback http (any port), or an app's own scheme: a reversed domain name (RFC 8252 §7.1, `com.example.app:/callback`) or one of `cursor`, `vscode`, `vscode-insiders`, `claude` and `windsurf`. Browser and operating-system handler schemes are refused (`invalid_redirect_uri`).\n    - **PKCE.** Required on every authorization request, with `code_challenge_method=S256`; no other method is accepted. The only grants are `authorization_code` and `refresh_token`.\n    - **Resource.**\
  \ Send `resource=https://api.kawaa.com` for this API (RFC 8707). Without it the token is issued for the MCP server, `https://api.kawaa.com/mcp`; any other value is refused with `invalid_target`.\n    - **Scopes.** With no `scope` parameter the request is for `verification:write verification:read account:read analytics:read`. Scopes Kawaa does not define, and scopes a connected app can never hold, are dropped rather than refused; if none remain the request is refused with `invalid_scope`. An authorization request refused before the person answers it (`invalid_request`, `unsupported_response_type`, `invalid_target`, `invalid_scope`) is shown to them on a Kawaa error page carrying that code, and is not sent to the redirect URI (RFC 9700 §4.11.2); only their answer is, the code or `access_denied`, with `state` and `iss`. The person approving can untick any scope, and the token response's `scope` states what was granted. `account:write`, `account:delete`, `billing:write`, `team:write`, `security:write`\
  \ and `white_label:write` are never granted, so the operations that need them do not list this scheme, and neither do those marked `x-kawaa-unscoped-only`. As for API keys, `<area>:write` also satisfies `<area>:read`.\n    - **Tokens.** An access token is `evo_` followed by 40 alphanumeric characters and lasts one hour (`expires_in: 3600`); after that the API answers 401 `OAUTH_TOKEN_EXPIRED`. A refresh token is `evr_` followed by 48 alphanumeric characters and is never accepted as a bearer credential. Every refresh returns a new refresh token and retires the one presented. The one just used may be presented up to 5 more times within 60 seconds of its use (a lost response, or several refreshes sent at once) and gets a new one of its own each time; the first of those to be used retires the rest. Presenting it again after that, or presenting any older refresh token, is treated as theft and ends the connection: its refresh tokens and every live access token stop working. A refresh may ask\
  \ for fewer scopes than the connection holds, never more. A connection that is not refreshed for 30 days ends. Revoke at `https://api.kawaa.com/oauth/revoke` (RFC 7009).\nscopes:\n- scope: account:read\n  description: Read the account profile, credit balance and notifications.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/kawaa-com-openapi.json\n- scope: analytics:read\n  description: Read usage, analytics and tracking figures.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/kawaa-com-openapi.json\n- scope: analytics:write\n  description: Create, change and permanently delete tracking pixels and links, and record usage-analytics\n    events for this account. Deleting a pixel or link breaks the tracking already embedded in\n    sent mail. Credit alert thresholds are fixed, so no scope changes them.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/kawaa-com-openapi.json\n- scope: billing:read\n  description: Read the subscription, invoices, payment methods\
  \ and billing address.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/kawaa-com-openapi.json\n- scope: compose:read\n  description: Read AI composition history.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/kawaa-com-openapi.json\n- scope: compose:write\n  description: Generate and improve email copy with AI. Spends credits.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/kawaa-com-openapi.json\n- scope: deliverability:read\n  description: Read deliverability checks, blacklist and DMARC monitors, and inbox-placement\n    and warmup state. Email warmup and inbox placement tests are not available yet.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/kawaa-com-openapi.json\n- scope: deliverability:write\n  description: Run deliverability checks and manage blacklist and DMARC monitors. Email warmup\n    and inbox placement tests are not available yet; warmup campaigns and SMTP credentials already\n    set up can still be removed.\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/kawaa-com-openapi.json\n- scope: exports:read\n  description: Read exports, export schedules and data-sharing settings. Downloading an export\n    also needs the scope that reads the data in it. Data sharing is not available yet.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/kawaa-com-openapi.json\n- scope: exports:write\n  description: 'Create and delete exports, manage export schedules and delivery destinations,\n    and change export settings. Exported files contain customer addresses, so each kind of data\n    also needs the scope that reads it: verification:read, account:read or security:read. Scheduled\n    exports deliver by email, webhook or Amazon S3; Google Cloud Storage and Azure Blob Storage\n    delivery is not available yet.'\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/kawaa-com-openapi.json\n- scope: integrations:read\n  description: Read connected integrations and their status.\n  flows:\n  - authorizationCode\n  sources:\n\
  \  - openapi/kawaa-com-openapi.json\n- scope: integrations:write\n  description: Connect and disconnect integrations, and push verification into them. The HubSpot,\n    Salesforce and Mailchimp connections are not available yet.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/kawaa-com-openapi.json\n- scope: lists:read\n  description: Read auto-clean lists and their run history.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/kawaa-com-openapi.json\n- scope: lists:write\n  description: Create, change, pause and delete auto-clean lists, and start rechecks. Each rechecked\n    address spends one credit. Creating, reactivating and starting rechecks require Professional\n    or above and account execution availability.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/kawaa-com-openapi.json\n- scope: security:read\n  description: Read security settings, sessions, login history and the audit log.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/kawaa-com-openapi.json\n\
  - scope: team:read\n  description: Read the team, its members and its invitations.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/kawaa-com-openapi.json\n- scope: verification:read\n  description: Read verification results and jobs this account has already paid for. Spends\n    nothing.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/kawaa-com-openapi.json\n- scope: verification:write\n  description: 'Anything that spends verification credits: verifying an address, a batch or\n    a file, finding a business email, and the domain and address-history lookups, which are\n    charged too.'\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/kawaa-com-openapi.json\n- scope: webhooks:read\n  description: Read webhook endpoints and their delivery logs.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/kawaa-com-openapi.json\n- scope: webhooks:write\n  description: Create, change and delete webhook endpoints, and rotate their signing secrets.\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/kawaa-com-openapi.json\n- scope: white_label:read\n  description: Read white-label configuration, sub-accounts and the custom API domain.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/kawaa-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/kawaa-com/scopes/kawaa-com-scopes.yml
summary_line: 21 scopes · authorizationCode
tags:
- Company
- Email Verification
- Software-as-a-Service
- Marketing
token_bound: false
token_urls:
- https://api.kawaa.com/oauth/token
---
