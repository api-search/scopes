---
api_specs:
- filename: xiaoman-openapi.yml
  format: yaml
  label: Xiaoman OKKI CRM Open API
  slug: xiaoman-okki-crm-open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xiaoman/refs/heads/main/openapi/xiaoman-openapi.yml
- filename: xiaoman-okki-go-openapi.yml
  format: yaml
  label: OKKI Go API
  slug: okki-go-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xiaoman/refs/heads/main/openapi/xiaoman-okki-go-openapi.yml
authorization_urls: []
description: Module scopes for the Xiaoman OKKI CRM Open API OAuth2 token endpoint (POST /v1/oauth2/access_token). The scope parameter is a space-separated list; a token can only call APIs of modules whose scope it carries (otherwise "no permission <module> scopes"). Each module's scope is also shown on the first page of that module's docs section.
docs: https://open.xiaoman.cn/api-3473041
flows:
- password
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Xiaoman Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Xiaoman (OKKI) publishes 12 OAuth 2.0 scopes via the password and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Xiaoman (OKKI) API on a user''s behalf.


  Tokens are issued from https://api-sandbox.xiaoman.cn/v1/oauth2/access_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Xiaoman (OKKI)
provider_slug: xiaoman
schemes:
- flows:
  - flow: password
    tokenUrl: https://api-sandbox.xiaoman.cn/v1/oauth2/access_token
  - flow: clientCredentials
    tokenUrl: https://api-sandbox.xiaoman.cn/v1/oauth2/access_token
  name: XiaomanOAuth2
scope_count: 12
scope_names:
- company
- lead
- opportunity
- product
- invoices
- purchaseOrder
- costInvoice
- paymentInvoice
- warehouse
- capitalAccount
- user
- webhook
scopes:
- description: Customers / companies module (客户)
  flows: []
  scope: company
- description: Leads module (线索)
  flows: []
  scope: lead
- description: Opportunities module (商机)
  flows: []
  scope: opportunity
- description: Products module (产品)
  flows: []
  scope: product
- description: Sales orders, quotations, and cash-collection invoices (订单、报价单、回款单)
  flows: []
  scope: invoices
- description: Purchase orders module (采购订单)
  flows: []
  scope: purchaseOrder
- description: Cost invoices module (费用单)
  flows: []
  scope: costInvoice
- description: Payment invoices module (付款单)
  flows: []
  scope: paymentInvoice
- description: Inventory / warehouse module (库存)
  flows: []
  scope: warehouse
- description: Capital accounts module (资金账户)
  flows: []
  scope: capitalAccount
- description: Users and departments (用户列表)
  flows: []
  scope: user
- description: Message push / webhook subscription module (消息推送)
  flows: []
  scope: webhook
slug: xiaoman-scopes
source_filename: xiaoman-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://open.xiaoman.cn/api-3473041\ndocs: https://open.xiaoman.cn/api-3473041\ndescription: >-\n  Module scopes for the Xiaoman OKKI CRM Open API OAuth2 token endpoint\n  (POST /v1/oauth2/access_token). The scope parameter is a space-separated\n  list; a token can only call APIs of modules whose scope it carries\n  (otherwise \"no permission <module> scopes\"). Each module's scope is also\n  shown on the first page of that module's docs section.\nschemes:\n  - name: XiaomanOAuth2\n    flows:\n      - flow: password\n        tokenUrl: https://api-sandbox.xiaoman.cn/v1/oauth2/access_token\n      - flow: clientCredentials\n        tokenUrl: https://api-sandbox.xiaoman.cn/v1/oauth2/access_token\nscopes:\n  - scope: company\n    description: Customers / companies module (客户)\n  - scope: lead\n    description: Leads module (线索)\n  - scope: opportunity\n    description: Opportunities module (商机)\n  - scope: product\n    description:\
  \ Products module (产品)\n  - scope: invoices\n    description: Sales orders, quotations, and cash-collection invoices (订单、报价单、回款单)\n  - scope: purchaseOrder\n    description: Purchase orders module (采购订单)\n  - scope: costInvoice\n    description: Cost invoices module (费用单)\n  - scope: paymentInvoice\n    description: Payment invoices module (付款单)\n  - scope: warehouse\n    description: Inventory / warehouse module (库存)\n  - scope: capitalAccount\n    description: Capital accounts module (资金账户)\n  - scope: user\n    description: Users and departments (用户列表)\n  - scope: webhook\n    description: Message push / webhook subscription module (消息推送)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xiaoman/refs/heads/main/scopes/xiaoman-scopes.yml
summary_line: 12 scopes · password/clientCredentials
tags:
- Company
- CRM
- Foreign Trade
- B2B
- Sales
- Prospecting
- Email Marketing
- AI Agents
- China
- Alibaba
token_urls:
- https://api-sandbox.xiaoman.cn/v1/oauth2/access_token
---
