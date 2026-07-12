---
authorization_urls:
- https://consent.criteo.com/authorize
description: ''
docs: https://developers.criteo.com/retail-media/docs/create-your-app
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Criteo Scopes
name_suffix: OAuth Scopes
note: Criteo expresses API permissions as application "domains" chosen when creating an API app in the developer portal, each set to a No access / Read / Manage authorization level, rather than as OAuth scope strings passed in the token request (see https://developers.criteo.com/retail-media/docs/create-your-app and https://developers.criteo.com/marketing-solutions/docs/create-your-app).
overview: 'Criteo publishes 13 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Criteo API on a user''s behalf.


  Tokens are issued from https://api.criteo.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Criteo
provider_slug: criteo
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.criteo.com/oauth2/token
  - authorizationUrl: https://consent.criteo.com/authorize
    flow: authorizationCode
    tokenUrl: https://api.criteo.com/oauth2/token
  name: OAuth2ClientCredentials
  source: openapi/criteo-openapi.yml
scope_count: 13
scope_names:
- Accounts
- Analytics
- Audiences
- Balances
- Billing
- Campaigns
- Catalog
- Analytics (Marketing Solutions)
- Audiences (Marketing Solutions)
- Campaigns (Marketing Solutions)
- Catalog (Marketing Solutions)
- Creatives (Marketing Solutions)
- Product recommendations configuration (Marketing Solutions)
scopes:
- description: 'Retail Media domain: manages permissions to endpoints responsible for describing accounts'' entities, with their properties and relationships, like parent/child accounts. Authorization levels: No access / Read / Manage (Manage requires prior activation by a Criteo contact).'
  flows: []
  scope: Accounts
- description: 'Retail Media domain: manages permissions to generate reporting data for campaigns & line-items, considering desired list of dimensions & metrics. Authorization levels: No access / Read.'
  flows: []
  scope: Analytics
- description: 'Retail Media domain: manages permissions to check/manage audiences available to campaigns. Authorization levels: No access / Read / Manage.'
  flows: []
  scope: Audiences
- description: 'Retail Media domain: manages permissions to endpoints responsible for configuring and retrieving balance entities, which define spending limits applied across campaigns. Authorization levels: No access / Read / Manage (Manage requires prior activation by a Criteo contact).'
  flows: []
  scope: Balances
- description: 'Retail Media domain: manages permissions to generate billing data for campaigns & line items for a retailer partner. Authorization levels: No access / Read (Read requires prior activation by a Criteo contact).'
  flows: []
  scope: Billing
- description: 'Retail Media domain: manages permissions to endpoints responsible for campaigns management, including line-items, balances and creatives. Authorization levels: No access / Read / Manage.'
  flows: []
  scope: Campaigns
- description: 'Retail Media domain: manages permissions to check/manage products catalogs. Authorization levels: No access / Read / Manage.'
  flows: []
  scope: Catalog
- description: 'Marketing Solutions (Commerce Growth) domain: generate custom reports; slice and dice your data across marketing goals and channels, including App, Web, and Store campaigns. Authorization levels: No access / Read.'
  flows: []
  scope: Analytics (Marketing Solutions)
- description: 'Marketing Solutions (Commerce Growth) domain: create, update, or delete your audiences using your own CRM segments, Criteo''s or your lists from a third party. Authorization levels: No access / Read / Manage.'
  flows: []
  scope: Audiences (Marketing Solutions)
- description: 'Marketing Solutions (Commerce Growth) domain: create and edit campaigns, ad sets, as well as update settings like CPCs. Authorization levels: No access / Read / Manage.'
  flows: []
  scope: Campaigns (Marketing Solutions)
- description: 'Marketing Solutions (Commerce Growth) domain: add and edit your product details. Authorization levels: No access / Read / Manage.'
  flows: []
  scope: Catalog (Marketing Solutions)
- description: 'Marketing Solutions (Commerce Growth) domain: create your own or use third-party creative that is displayed by an external creative provider at display time; access, add, or edit creative from the API. Authorization levels: No access / Read / Manage.'
  flows: []
  scope: Creatives (Marketing Solutions)
- description: 'Marketing Solutions (Commerce Growth) domain: product recommendations configuration; access must be requested. Authorization levels: No access / Read / Manage.'
  flows: []
  scope: Product recommendations configuration (Marketing Solutions)
slug: criteo-scopes
source_filename: criteo-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\nsource: openapi/criteo-openapi.yml\ndocs: https://developers.criteo.com/retail-media/docs/create-your-app\nnote: Criteo expresses API permissions as application \"domains\" chosen when creating\n  an API app in the developer portal, each set to a No access / Read / Manage authorization\n  level, rather than as OAuth scope strings passed in the token request (see\n  https://developers.criteo.com/retail-media/docs/create-your-app and\n  https://developers.criteo.com/marketing-solutions/docs/create-your-app).\nschemes:\n- name: OAuth2ClientCredentials\n  source: openapi/criteo-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.criteo.com/oauth2/token\n  - flow: authorizationCode\n    authorizationUrl: https://consent.criteo.com/authorize\n    tokenUrl: https://api.criteo.com/oauth2/token\nscopes:\n- scope: Accounts\n  description: 'Retail Media domain: manages permissions to endpoints responsible\n    for describing\
  \ accounts'' entities, with their properties and relationships,\n    like parent/child accounts. Authorization levels: No access / Read / Manage\n    (Manage requires prior activation by a Criteo contact).'\n  sources:\n  - https://developers.criteo.com/retail-media/docs/create-your-app\n- scope: Analytics\n  description: 'Retail Media domain: manages permissions to generate reporting data\n    for campaigns & line-items, considering desired list of dimensions & metrics.\n    Authorization levels: No access / Read.'\n  sources:\n  - https://developers.criteo.com/retail-media/docs/create-your-app\n- scope: Audiences\n  description: 'Retail Media domain: manages permissions to check/manage audiences\n    available to campaigns. Authorization levels: No access / Read / Manage.'\n  sources:\n  - https://developers.criteo.com/retail-media/docs/create-your-app\n- scope: Balances\n  description: 'Retail Media domain: manages permissions to endpoints responsible\n    for configuring and retrieving\
  \ balance entities, which define spending limits\n    applied across campaigns. Authorization levels: No access / Read / Manage\n    (Manage requires prior activation by a Criteo contact).'\n  sources:\n  - https://developers.criteo.com/retail-media/docs/create-your-app\n- scope: Billing\n  description: 'Retail Media domain: manages permissions to generate billing data\n    for campaigns & line items for a retailer partner. Authorization levels: No\n    access / Read (Read requires prior activation by a Criteo contact).'\n  sources:\n  - https://developers.criteo.com/retail-media/docs/create-your-app\n- scope: Campaigns\n  description: 'Retail Media domain: manages permissions to endpoints responsible\n    for campaigns management, including line-items, balances and creatives.\n    Authorization levels: No access / Read / Manage.'\n  sources:\n  - https://developers.criteo.com/retail-media/docs/create-your-app\n- scope: Catalog\n  description: 'Retail Media domain: manages permissions\
  \ to check/manage products\n    catalogs. Authorization levels: No access / Read / Manage.'\n  sources:\n  - https://developers.criteo.com/retail-media/docs/create-your-app\n- scope: Analytics (Marketing Solutions)\n  description: 'Marketing Solutions (Commerce Growth) domain: generate custom\n    reports; slice and dice your data across marketing goals and channels,\n    including App, Web, and Store campaigns. Authorization levels: No access /\n    Read.'\n  sources:\n  - https://developers.criteo.com/marketing-solutions/docs/create-your-app\n- scope: Audiences (Marketing Solutions)\n  description: 'Marketing Solutions (Commerce Growth) domain: create, update, or\n    delete your audiences using your own CRM segments, Criteo''s or your lists\n    from a third party. Authorization levels: No access / Read / Manage.'\n  sources:\n  - https://developers.criteo.com/marketing-solutions/docs/create-your-app\n- scope: Campaigns (Marketing Solutions)\n  description: 'Marketing Solutions (Commerce\
  \ Growth) domain: create and edit\n    campaigns, ad sets, as well as update settings like CPCs. Authorization\n    levels: No access / Read / Manage.'\n  sources:\n  - https://developers.criteo.com/marketing-solutions/docs/create-your-app\n- scope: Catalog (Marketing Solutions)\n  description: 'Marketing Solutions (Commerce Growth) domain: add and edit your\n    product details. Authorization levels: No access / Read / Manage.'\n  sources:\n  - https://developers.criteo.com/marketing-solutions/docs/create-your-app\n- scope: Creatives (Marketing Solutions)\n  description: 'Marketing Solutions (Commerce Growth) domain: create your own or\n    use third-party creative that is displayed by an external creative provider\n    at display time; access, add, or edit creative from the API. Authorization\n    levels: No access / Read / Manage.'\n  sources:\n  - https://developers.criteo.com/marketing-solutions/docs/create-your-app\n- scope: Product recommendations configuration (Marketing Solutions)\n\
  \  description: 'Marketing Solutions (Commerce Growth) domain: product\n    recommendations configuration; access must be requested. Authorization\n    levels: No access / Read / Manage.'\n  sources:\n  - https://developers.criteo.com/marketing-solutions/docs/create-your-app\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/scopes/criteo-scopes.yml
summary_line: 13 scopes · clientCredentials/authorizationCode
tags:
- Advertising
- Audiences
- Campaigns
- Catalog
- Commerce
- Display Advertising
- Marketing
- Media
- OAuth 2.0
- Reporting
- Retail
- Retail Media
token_urls:
- https://api.criteo.com/oauth2/token
---
