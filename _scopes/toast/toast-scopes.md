---
api_specs:
- filename: toast-orders-openapi.yaml
  format: yaml
  label: Toast Orders API
  slug: toast-orders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-orders-openapi.yaml
- filename: toast-menus-openapi.yaml
  format: yaml
  label: Toast Menus API
  slug: toast-menus
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-menus-openapi.yaml
- filename: toast-labor-openapi.yaml
  format: yaml
  label: Toast Labor API
  slug: toast-labor
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-labor-openapi.yaml
- filename: toast-restaurants-openapi.yaml
  format: yaml
  label: Toast Restaurants API
  slug: toast-restaurants
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-restaurants-openapi.yaml
- filename: toast-stock-openapi.yaml
  format: yaml
  label: Toast Stock API
  slug: toast-stock
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-stock-openapi.yaml
- filename: toast-partners-openapi.yaml
  format: yaml
  label: Toast Partners API
  slug: toast-partners
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-partners-openapi.yaml
- filename: toast-authentication-openapi.yaml
  format: yaml
  label: Toast Authentication API
  slug: toast-authentication
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-authentication-openapi.yaml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Toast Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Toast publishes 22 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Toast API on a user''s behalf.


  Tokens are issued from https://toast-api-server/authentication/v1/authentication/login.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Toast
provider_slug: toast
schemes:
- description: "Access to Toast APIs, specific endpoints, \nand specific API endpoint operations is \ncontrolled by the scopes that are associated \nwith your API account. \nA full reference for Toast API scopes and \ntheir capabilities can be found in the\n[_Toast Developer Guide_](https://doc.toasttab.com/doc/devguide/apiScopes.html)."
  flows:
  - flow: clientCredentials
    tokenUrl: https://toast-api-server/authentication/v1/authentication/login
  name: oauth2
  source: openapi/toast-labor-openapi.yaml
- description: "Access to Toast APIs, specific endpoints, \nand specific API endpoint operations is \ncontrolled by the scopes that are associated \nwith your API account. \n\nA full reference for Toast API scopes and \ntheir capabilities can be found in the\n[_Toast Developer Guide_](https://doc.toasttab.com/doc/devguide/apiScopes.html)."
  flows:
  - flow: clientCredentials
    tokenUrl: https://toast-api-server/authentication/v1/authentication/login
  name: oauth2
  source: openapi/toast-menus-openapi.yaml
- description: "Access to Toast APIs, specific endpoints, \nand specific API endpoint operations is \ncontrolled by the scopes that are associated \nwith your API account. \n\nA full reference for Toast API scopes and \ntheir capabilities can be found in the\n[_Toast Developer Guide_](https://doc.toasttab.com/doc/devguide/apiScopes.html)."
  flows:
  - flow: clientCredentials
    tokenUrl: https://toast-api-server/authentication/v1/authentication/login
  name: oauth2
  source: openapi/toast-orders-openapi.yaml
- description: "Access to Toast APIs, specific endpoints, \nand specific API endpoint operations is \ncontrolled by the scopes that are associated \nwith your API account. \nA full reference for Toast API scopes and \ntheir capabilities can be found in the\n[_Toast Developer Guide_](https://doc.toasttab.com/doc/devguide/apiScopes.html)."
  flows:
  - flow: clientCredentials
    tokenUrl: https://toast-api-server/authentication/v1/authentication/login
  name: oauth2
  source: openapi/toast-partners-openapi.yaml
- description: "Access to Toast APIs, specific endpoints, \nand specific API endpoint operations is \ncontrolled by the scopes that are associated \nwith your API account. \nA full reference for Toast API scopes and \ntheir capabilities can be found in the\n[_Toast Developer Guide_](https://doc.toasttab.com/doc/devguide/apiScopes.html)."
  flows:
  - flow: clientCredentials
    tokenUrl: https://toast-api-server/authentication/v1/authentication/login
  name: oauth2
  source: openapi/toast-restaurants-openapi.yaml
- description: "Access to Toast APIs, specific endpoints, \nand specific API endpoint operations is \ncontrolled by the scopes that are associated \nwith your API account. \n\nA full reference for Toast API scopes and \ntheir capabilities can be found in the\n[_Toast Developer Guide_](https://doc.toasttab.com/doc/devguide/apiScopes.html)."
  flows:
  - flow: clientCredentials
    tokenUrl: https://toast-api-server/authentication/v1/authentication/login
  name: oauth2
  source: openapi/toast-stock-openapi.yaml
scope_count: 22
scope_names:
- delivery_info.address:read
- employees.tax-identifier-masked:read
- employees.tax-identifier-unmasked:read
- guest.pi:read
- labor.employees:read
- labor.employees:write
- labor.jobs:write
- labor.shifts:write
- labor:read
- menus:read
- orders.channel:read
- orders.channel:void
- orders.delivery_info:write
- orders.discounts:write
- orders.items:write
- orders.orders:write
- orders.payments:write
- orders:read
- orders:void
- restaurants:read
- stock:read
- stock:write
scopes:
- description: Allows reading guest delivery address information from the orders API. Optionally used in conjunction with the `orders:read` scope to return the `deliveredDate`, `dispatchedDate`, `deliveryEmployee`, and `deliveryState` fields as part of the `deliveryInfo` field on the Order object.
  flows:
  - clientCredentials
  scope: delivery_info.address:read
- description: Allows reading masked tax identifier (SSN) information for employees via expand parameter.
  flows:
  - clientCredentials
  scope: employees.tax-identifier-masked:read
- description: Allows reading full unmasked tax identifier (SSN) information for employees via expand parameter.
  flows:
  - clientCredentials
  scope: employees.tax-identifier-unmasked:read
- description: Allows reading guest and curbside pickup information from the orders API. Optionally used in conjunction with the `orders:read` scope to return the `email` and `phone` fields as part of the `checks[].customer` object.
  flows:
  - clientCredentials
  scope: guest.pi:read
- description: Allows reading employee information from the labor API.
  flows:
  - clientCredentials
  scope: labor.employees:read
- description: Allows updating employee information in the labor API.
  flows:
  - clientCredentials
  scope: labor.employees:write
- description: Allows updating job information in the labor API.
  flows:
  - clientCredentials
  scope: labor.jobs:write
- description: Allows updating shift information in the labor API.
  flows:
  - clientCredentials
  scope: labor.shifts:write
- description: Allows reading all data except employees from the labor API.
  flows:
  - clientCredentials
  scope: labor:read
- description: Allows reading from menus API V2.
  flows:
  - clientCredentials
  scope: menus:read
- description: Allows API clients that submit orders to the Toast platform to read from the orders API. To read orders, the API client must have both the orders:read scope and the orders.channel:read scope. API clients that have the orders.channel:read scope can only read the orders that they submitted. They cannot read orders from any other source.
  flows:
  - clientCredentials
  scope: orders.channel:read
- description: ''
  flows: []
  scope: orders.channel:void
- description: Allows updating delivery information from the orders API.
  flows:
  - clientCredentials
  scope: orders.delivery_info:write
- description: Allows adding discounts to orders using the orders API.
  flows:
  - clientCredentials
  scope: orders.discounts:write
- description: Allows adding items to orders using the orders API.
  flows:
  - clientCredentials
  scope: orders.items:write
- description: Allows posting orders orders using the orders API.
  flows:
  - clientCredentials
  scope: orders.orders:write
- description: Allows adding payments and tips to existing orders using the orders API.
  flows:
  - clientCredentials
  scope: orders.payments:write
- description: Allows reading from the orders API with the exception of guest information. If your API client creates orders, then to read orders, it must have both the orders:read scope and the orders.channel:read scope.
  flows:
  - clientCredentials
  scope: orders:read
- description: ''
  flows: []
  scope: orders:void
- description: Allows reading from the restaurants API.
  flows:
  - clientCredentials
  scope: restaurants:read
- description: Allows reading from the stock API.
  flows:
  - clientCredentials
  scope: stock:read
- description: Allows updating stock status for menu items (and modifier option item references) using the stock API.
  flows:
  - clientCredentials
  scope: stock:write
slug: toast-scopes
source_filename: toast-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/toast-labor-openapi.yaml, openapi/toast-menus-openapi.yaml, openapi/toast-orders-openapi.yaml,\n  openapi/toast-partners-openapi.yaml, openapi/toast-restaurants-openapi.yaml, openapi/toast-stock-openapi.yaml\nschemes:\n- name: oauth2\n  source: openapi/toast-labor-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://toast-api-server/authentication/v1/authentication/login\n  description: \"Access to Toast APIs, specific endpoints, \\nand specific API endpoint operations\\\n    \\ is \\ncontrolled by the scopes that are associated \\nwith your API account. \\nA full reference\\\n    \\ for Toast API scopes and \\ntheir capabilities can be found in the\\n[_Toast Developer Guide_](https://doc.toasttab.com/doc/devguide/apiScopes.html).\"\n- name: oauth2\n  source: openapi/toast-menus-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://toast-api-server/authentication/v1/authentication/login\n\
  \  description: \"Access to Toast APIs, specific endpoints, \\nand specific API endpoint operations\\\n    \\ is \\ncontrolled by the scopes that are associated \\nwith your API account. \\n\\nA full\\\n    \\ reference for Toast API scopes and \\ntheir capabilities can be found in the\\n[_Toast Developer\\\n    \\ Guide_](https://doc.toasttab.com/doc/devguide/apiScopes.html).\"\n- name: oauth2\n  source: openapi/toast-orders-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://toast-api-server/authentication/v1/authentication/login\n  description: \"Access to Toast APIs, specific endpoints, \\nand specific API endpoint operations\\\n    \\ is \\ncontrolled by the scopes that are associated \\nwith your API account. \\n\\nA full\\\n    \\ reference for Toast API scopes and \\ntheir capabilities can be found in the\\n[_Toast Developer\\\n    \\ Guide_](https://doc.toasttab.com/doc/devguide/apiScopes.html).\"\n- name: oauth2\n  source: openapi/toast-partners-openapi.yaml\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: https://toast-api-server/authentication/v1/authentication/login\n  description: \"Access to Toast APIs, specific endpoints, \\nand specific API endpoint operations\\\n    \\ is \\ncontrolled by the scopes that are associated \\nwith your API account. \\nA full reference\\\n    \\ for Toast API scopes and \\ntheir capabilities can be found in the\\n[_Toast Developer Guide_](https://doc.toasttab.com/doc/devguide/apiScopes.html).\"\n- name: oauth2\n  source: openapi/toast-restaurants-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://toast-api-server/authentication/v1/authentication/login\n  description: \"Access to Toast APIs, specific endpoints, \\nand specific API endpoint operations\\\n    \\ is \\ncontrolled by the scopes that are associated \\nwith your API account. \\nA full reference\\\n    \\ for Toast API scopes and \\ntheir capabilities can be found in the\\n[_Toast Developer Guide_](https://doc.toasttab.com/doc/devguide/apiScopes.html).\"\
  \n- name: oauth2\n  source: openapi/toast-stock-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://toast-api-server/authentication/v1/authentication/login\n  description: \"Access to Toast APIs, specific endpoints, \\nand specific API endpoint operations\\\n    \\ is \\ncontrolled by the scopes that are associated \\nwith your API account. \\n\\nA full\\\n    \\ reference for Toast API scopes and \\ntheir capabilities can be found in the\\n[_Toast Developer\\\n    \\ Guide_](https://doc.toasttab.com/doc/devguide/apiScopes.html).\"\nscopes:\n- scope: delivery_info.address:read\n  description: |-\n    Allows reading guest delivery address information from the orders API.\n    Optionally used in conjunction with the `orders:read` scope to return\n    the `deliveredDate`, `dispatchedDate`, `deliveryEmployee`, and `deliveryState`\n    fields as part of the `deliveryInfo` field on the Order object.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/toast-orders-openapi.yaml\n\
  - scope: employees.tax-identifier-masked:read\n  description: |-\n    Allows reading masked tax identifier (SSN) information for employees via\n    expand parameter.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/toast-labor-openapi.yaml\n- scope: employees.tax-identifier-unmasked:read\n  description: |-\n    Allows reading full unmasked tax identifier (SSN) information for employees\n    via expand parameter.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/toast-labor-openapi.yaml\n- scope: guest.pi:read\n  description: |-\n    Allows reading guest and curbside pickup information from the orders API.\n    Optionally used in conjunction with the `orders:read` scope to return the\n    `email` and `phone` fields as part of the `checks[].customer` object.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/toast-orders-openapi.yaml\n- scope: labor.employees:read\n  description: Allows reading employee information from the labor API.\n  flows:\n  - clientCredentials\n\
  \  sources:\n  - openapi/toast-labor-openapi.yaml\n- scope: labor.employees:write\n  description: Allows updating employee information in the labor API.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/toast-labor-openapi.yaml\n- scope: labor.jobs:write\n  description: Allows updating job information in the labor API.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/toast-labor-openapi.yaml\n- scope: labor.shifts:write\n  description: Allows updating shift information in the labor API.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/toast-labor-openapi.yaml\n- scope: labor:read\n  description: Allows reading all data except employees from the labor API.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/toast-labor-openapi.yaml\n- scope: menus:read\n  description: Allows reading from menus API V2.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/toast-menus-openapi.yaml\n- scope: orders.channel:read\n  description: |-\n    Allows API clients\
  \ that submit orders to the Toast platform to read from the orders API.\n\n    To read orders, the API client must have both the orders:read scope and the orders.channel:read scope.\n\n    API clients that have the orders.channel:read scope can only read the orders that they submitted. They cannot\n    read orders from any other source.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/toast-orders-openapi.yaml\n- scope: orders.channel:void\n  sources:\n  - openapi/toast-orders-openapi.yaml\n- scope: orders.delivery_info:write\n  description: Allows updating delivery information from the orders API.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/toast-orders-openapi.yaml\n- scope: orders.discounts:write\n  description: Allows adding discounts to orders using the orders API.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/toast-orders-openapi.yaml\n- scope: orders.items:write\n  description: Allows adding items to orders using the orders API.\n  flows:\n  -\
  \ clientCredentials\n  sources:\n  - openapi/toast-orders-openapi.yaml\n- scope: orders.orders:write\n  description: Allows posting orders orders using the orders API.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/toast-orders-openapi.yaml\n- scope: orders.payments:write\n  description: Allows adding payments and tips to existing orders using the orders API.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/toast-orders-openapi.yaml\n- scope: orders:read\n  description: \"Allows reading from the orders API with the exception of guest information.\\n\\\n    \\nIf your API client creates orders, then to read orders, it must have both the orders:read\\\n    \\ scope and the \\norders.channel:read scope.\"\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/toast-orders-openapi.yaml\n- scope: orders:void\n  sources:\n  - openapi/toast-orders-openapi.yaml\n- scope: restaurants:read\n  description: Allows reading from the restaurants API.\n  flows:\n  - clientCredentials\n\
  \  sources:\n  - openapi/toast-restaurants-openapi.yaml\n- scope: stock:read\n  description: Allows reading from the stock API.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/toast-stock-openapi.yaml\n- scope: stock:write\n  description: Allows updating stock status for menu items (and modifier option item references)\n    using the stock API.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/toast-stock-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/scopes/toast-scopes.yml
summary_line: 22 scopes · clientCredentials
tags:
- Food Service
- Point of Sale
- Restaurants
- Hospitality
token_urls:
- https://toast-api-server/authentication/v1/authentication/login
---
