---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Hologic Scopes
name_suffix: OAuth Scopes
note: 'These are the scopes_supported values advertised by the OpenID Connect discovery document Hologic serves at support.hologic.com. IMPORTANT PROVENANCE: this is the stock Salesforce Experience Cloud scope vocabulary, served under Hologic''s issuer for the customer support community. Hologic did not author these scope names and does not document them as an API permission model; no Hologic scope reference page exists. They are recorded because the document is real, fetchable and provider-served, and because it is the only OAuth scope surface the company exposes. Do not read this file as a Hologic API authorization scheme.'
overview: 'Hologic uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Hologic
provider_slug: hologic
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: hologic-scopes
source_filename: hologic-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: https://support.hologic.com/.well-known/openid-configuration\nnote: >-\n  These are the scopes_supported values advertised by the OpenID Connect discovery document\n  Hologic serves at support.hologic.com. IMPORTANT PROVENANCE: this is the stock Salesforce\n  Experience Cloud scope vocabulary, served under Hologic's issuer for the customer support\n  community. Hologic did not author these scope names and does not document them as an API\n  permission model; no Hologic scope reference page exists. They are recorded because the\n  document is real, fetchable and provider-served, and because it is the only OAuth scope\n  surface the company exposes. Do not read this file as a Hologic API authorization scheme.\nauthorization_server: https://support.hologic.com\nplatform: Salesforce Experience Cloud\ndocs: null\ndocs_note: No Hologic-published scope or permissions reference page exists.\nscope_count: 36\nscopes:\n  - name: openid\n\
  \    description: OpenID Connect — request an ID token for the authenticated support-community user.\n  - name: profile\n    description: Standard OIDC profile claims.\n  - name: email\n    description: Standard OIDC email claims.\n  - name: address\n    description: Standard OIDC address claim.\n  - name: phone\n    description: Standard OIDC phone claims.\n  - name: offline_access\n    description: Issue a refresh token.\n  - name: refresh_token\n    description: Salesforce alias for refresh-token issuance.\n  - name: id\n    description: Salesforce identity URL access.\n  - name: api\n    description: Salesforce platform REST/SOAP API access on behalf of the user.\n  - name: full\n    description: Full access to all data the user can reach.\n  - name: web\n    description: Access via a web-server flow session.\n  - name: lightning\n    description: Lightning Experience application access.\n  - name: visualforce\n    description: Visualforce page access.\n  - name: content\n    description:\
  \ Salesforce Files/Content access.\n  - name: chatter_api\n    description: Chatter REST API access.\n  - name: chatbot_api\n    description: Einstein Bots API access.\n  - name: custom_permissions\n    description: Return the custom permissions granted to the user.\n  - name: wave_api\n    description: CRM Analytics (Wave) API access.\n  - name: eclair_api\n    description: CRM Analytics geo/map (Eclair) API access.\n  - name: pardot_api\n    description: Account Engagement (Pardot) API access.\n  - name: interaction_api\n    description: Interaction/Next-Best-Action API access.\n  - name: user_registration_api\n    description: Self-registration API for community users.\n  - name: pwdless_login_api\n    description: Passwordless login API.\n  - name: forgot_password\n    description: Password-reset API.\n  - name: scrt_api\n    description: Service Cloud real-time (messaging) API access.\n  - name: sfap_api\n    description: Salesforce AI platform API access.\n  - name: einstein_gpt_api\n\
  \    description: Einstein generative-AI API access.\n  - name: mcp_api\n    description: >-\n      Salesforce-platform MCP API scope advertised by the Experience Cloud IdP. This is a\n      Salesforce capability, NOT a Hologic-operated MCP server — no Hologic MCP endpoint was\n      found by any probe in this pass.\n  - name: cdp_api\n    description: Data Cloud (CDP) API access.\n  - name: cdp_ingest_api\n    description: Data Cloud ingestion API access.\n  - name: cdp_query_api\n    description: Data Cloud query API access.\n  - name: cdp_profile_api\n    description: Data Cloud profile API access.\n  - name: cdp_segment_api\n    description: Data Cloud segmentation API access.\n  - name: cdp_identityresolution_api\n    description: Data Cloud identity-resolution API access.\n  - name: cdp_calculated_insight_api\n    description: Data Cloud calculated-insights API access.\n  - name: data_cloud_user_claims\n    description: Data Cloud user claims in the ID token.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hologic/refs/heads/main/scopes/hologic-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Fortune 1000
- Healthcare
- Medical Devices
- Medical Imaging
- Diagnostics
- Women's Health
- DICOM
- Life Sciences
token_urls: []
---
