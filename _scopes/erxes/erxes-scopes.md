---
authorization_urls: []
description: ''
docs:
- https://github.com/erxes/erxes-skills/blob/main/agent-plugin/erxes-next/erxes-graphql-api.md
- https://github.com/erxes/erxes-skills/blob/main/agent-plugin/erxes-next/operation-api.md
- https://github.com/erxes/erxes-cli#authenticate
flows:
- deviceCode
kind: oauth-scopes
layout: scope
method: searched
name: Erxes Scopes
name_suffix: OAuth Scopes
note: '0-working/derive-oauth-scopes.py could not run a baseline — erxes publishes no OpenAPI, so there is no securitySchemes block to aggregate. These scopes are SEARCHED from the provider''s own published agent-plugin reference, where each core GraphQL operation is filed under the exact scope string that authorizes it, and from the erxes CLI README, which names the versioned "public operation" identifiers an OAuth client must enable. OAuth clients are created per tenant in erxes Settings > OAuth Clients. Nothing here is inferred: every scope string below appears verbatim in a provider-published document.'
overview: 'Erxes publishes 34 OAuth 2.0 scopes via the deviceCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Erxes API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Erxes
provider_slug: erxes
schemes:
- flows:
  - flow: deviceCode
    grant_type: urn:ietf:params:oauth:grant-type:device_code
    registration: erxes Settings > OAuth Clients
  name: OAuth2 Device Authorization Grant
  source: authentication/erxes-authentication.yml
scope_count: 34
scope_names:
- contacts:read
- contacts:create
- contacts:update
- contacts:remove
- contacts:merge
- products:read
- products:create
- products:update
- products:remove
- products:merge
- products:manage
- tags:read
- tags:create
- tags:update
- tags:remove
- tags:tag
- documents:read
- documents:create
- documents:update
- documents:remove
- brands:read
- brands:create
- brands:update
- brands:remove
- organization:read
- organization:manage
- teamMembers:read
- teamMembers:create
- teamMembers:update
- teamMembers:remove
- automations:read
- automations:create
- automations:update
- automations:delete
scopes:
- description: List and view customers (customers, customerDetail).
  flows: []
  scope: contacts:read
- description: Create a customer (customersAdd).
  flows: []
  scope: contacts:create
- description: Edit customer information (customersEdit).
  flows: []
  scope: contacts:update
- description: Delete customers (customersRemove).
  flows: []
  scope: contacts:remove
- description: Merge duplicate customer records (customersMerge).
  flows: []
  scope: contacts:merge
- description: List products (products).
  flows: []
  scope: products:read
- description: Create products and product categories (productsAdd, productCategoriesAdd).
  flows: []
  scope: products:create
- description: Edit products (productsEdit).
  flows: []
  scope: products:update
- description: Delete products (productsRemove).
  flows: []
  scope: products:remove
- description: Merge duplicate products (productsMerge).
  flows: []
  scope: products:merge
- description: Manage product supporting records such as units of measure (uomsAdd).
  flows: []
  scope: products:manage
- description: List tags (tags).
  flows: []
  scope: tags:read
- description: Create a tag (tagsAdd).
  flows: []
  scope: tags:create
- description: Edit a tag (tagsEdit).
  flows: []
  scope: tags:update
- description: Delete a tag (tagsRemove).
  flows: []
  scope: tags:remove
- description: Attach or detach a tag on another object (tagsTag).
  flows: []
  scope: tags:tag
- description: List documents (documents).
  flows: []
  scope: documents:read
- description: Create documents (documentsSave). erxes documents this paired with documents:update.
  flows: []
  scope: documents:create
- description: Edit documents (documentsSave). erxes documents this paired with documents:create.
  flows: []
  scope: documents:update
- description: Delete documents (documentsRemove).
  flows: []
  scope: documents:remove
- description: List brands (brands).
  flows: []
  scope: brands:read
- description: Create a brand (brandsAdd).
  flows: []
  scope: brands:create
- description: Edit a brand (brandsEdit).
  flows: []
  scope: brands:update
- description: Delete a brand (brandsRemove).
  flows: []
  scope: brands:remove
- description: Read the organization structure — departments, branches, units (structures).
  flows: []
  scope: organization:read
- description: Create organization structure records (departmentsAdd, branchesAdd).
  flows: []
  scope: organization:manage
- description: List team members (users).
  flows: []
  scope: teamMembers:read
- description: Invite a new team member (usersInvite).
  flows: []
  scope: teamMembers:create
- description: Edit a team member (usersEdit).
  flows: []
  scope: teamMembers:update
- description: Deactivate a team member (usersSetActiveStatus).
  flows: []
  scope: teamMembers:remove
- description: List automations (automations).
  flows: []
  scope: automations:read
- description: Create an automation (automationsAdd).
  flows: []
  scope: automations:create
- description: Edit an automation (automationsEdit).
  flows: []
  scope: automations:update
- description: Delete an automation (automationsRemove).
  flows: []
  scope: automations:delete
slug: erxes-scopes
source_filename: erxes-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://github.com/erxes/erxes-skills/blob/main/agent-plugin/erxes-next/erxes-graphql-api.md\ndocs:\n  - https://github.com/erxes/erxes-skills/blob/main/agent-plugin/erxes-next/erxes-graphql-api.md\n  - https://github.com/erxes/erxes-skills/blob/main/agent-plugin/erxes-next/operation-api.md\n  - https://github.com/erxes/erxes-cli#authenticate\nnote: >-\n  0-working/derive-oauth-scopes.py could not run a baseline — erxes publishes no\n  OpenAPI, so there is no securitySchemes block to aggregate. These scopes are\n  SEARCHED from the provider's own published agent-plugin reference, where each\n  core GraphQL operation is filed under the exact scope string that authorizes\n  it, and from the erxes CLI README, which names the versioned \"public\n  operation\" identifiers an OAuth client must enable. OAuth clients are created\n  per tenant in erxes Settings > OAuth Clients. Nothing here is inferred: every\n  scope string below\
  \ appears verbatim in a provider-published document.\nschemes:\n  - name: OAuth2 Device Authorization Grant\n    flows:\n      - flow: deviceCode\n        grant_type: 'urn:ietf:params:oauth:grant-type:device_code'\n        registration: erxes Settings > OAuth Clients\n    source: authentication/erxes-authentication.yml\nscopes:\n  - {scope: 'contacts:read', description: 'List and view customers (customers, customerDetail).', resource: contacts}\n  - {scope: 'contacts:create', description: 'Create a customer (customersAdd).', resource: contacts}\n  - {scope: 'contacts:update', description: 'Edit customer information (customersEdit).', resource: contacts}\n  - {scope: 'contacts:remove', description: 'Delete customers (customersRemove).', resource: contacts}\n  - {scope: 'contacts:merge', description: 'Merge duplicate customer records (customersMerge).', resource: contacts}\n  - {scope: 'products:read', description: 'List products (products).', resource: products}\n  - {scope: 'products:create',\
  \ description: 'Create products and product categories (productsAdd, productCategoriesAdd).', resource: products}\n  - {scope: 'products:update', description: 'Edit products (productsEdit).', resource: products}\n  - {scope: 'products:remove', description: 'Delete products (productsRemove).', resource: products}\n  - {scope: 'products:merge', description: 'Merge duplicate products (productsMerge).', resource: products}\n  - {scope: 'products:manage', description: 'Manage product supporting records such as units of measure (uomsAdd).', resource: products}\n  - {scope: 'tags:read', description: 'List tags (tags).', resource: tags}\n  - {scope: 'tags:create', description: 'Create a tag (tagsAdd).', resource: tags}\n  - {scope: 'tags:update', description: 'Edit a tag (tagsEdit).', resource: tags}\n  - {scope: 'tags:remove', description: 'Delete a tag (tagsRemove).', resource: tags}\n  - {scope: 'tags:tag', description: 'Attach or detach a tag on another object (tagsTag).', resource: tags}\n\
  \  - {scope: 'documents:read', description: 'List documents (documents).', resource: documents}\n  - {scope: 'documents:create', description: 'Create documents (documentsSave). erxes documents this paired with documents:update.', resource: documents}\n  - {scope: 'documents:update', description: 'Edit documents (documentsSave). erxes documents this paired with documents:create.', resource: documents}\n  - {scope: 'documents:remove', description: 'Delete documents (documentsRemove).', resource: documents}\n  - {scope: 'brands:read', description: 'List brands (brands).', resource: brands}\n  - {scope: 'brands:create', description: 'Create a brand (brandsAdd).', resource: brands}\n  - {scope: 'brands:update', description: 'Edit a brand (brandsEdit).', resource: brands}\n  - {scope: 'brands:remove', description: 'Delete a brand (brandsRemove).', resource: brands}\n  - {scope: 'organization:read', description: 'Read the organization structure — departments, branches, units (structures).', resource:\
  \ organization}\n  - {scope: 'organization:manage', description: 'Create organization structure records (departmentsAdd, branchesAdd).', resource: organization}\n  - {scope: 'teamMembers:read', description: 'List team members (users).', resource: teamMembers}\n  - {scope: 'teamMembers:create', description: 'Invite a new team member (usersInvite).', resource: teamMembers}\n  - {scope: 'teamMembers:update', description: 'Edit a team member (usersEdit).', resource: teamMembers}\n  - {scope: 'teamMembers:remove', description: 'Deactivate a team member (usersSetActiveStatus).', resource: teamMembers}\n  - {scope: 'automations:read', description: 'List automations (automations).', resource: automations}\n  - {scope: 'automations:create', description: 'Create an automation (automationsAdd).', resource: automations}\n  - {scope: 'automations:update', description: 'Edit an automation (automationsEdit).', resource: automations}\n  - {scope: 'automations:delete', description: 'Delete an automation\
  \ (automationsRemove).', resource: automations}\nscope_count: 34\npublic_operations:\n  note: >-\n    Separate from the scope strings above, the erxes CLI documents versioned\n    \"public operation\" identifiers that must be enabled individually on an\n    OAuth client before that client may call them. Only the three the CLI needs\n    are published; the naming shape is <plugin>.<module>.<resource>.<verb>.<version>.\n  source: https://github.com/erxes/erxes-cli#authenticate\n  operations:\n    - core.contacts.customers.list.v1\n    - core.contacts.customers.detail.v1\n    - core.contacts.customers.create.v1\nbackend_permissions:\n  note: >-\n    The operation plugin additionally publishes backend permission NAMES (not\n    OAuth scopes). erxes states these are backend reference only and that an\n    agent should proceed as owner and surface an access issue only when the API\n    actually rejects a call. Recorded for completeness, not as a scope surface.\n  source: https://github.com/erxes/erxes-skills/blob/main/agent-plugin/erxes-next/operation-api.md\n\
  \  permissions:\n    tasks: [taskRead, taskCreate, taskUpdate, taskRemove, taskAssign]\n    triage: [triageRead, triageCreate, triageUpdate, triageConvert]\n    projects: [projectRead, projectCreate, projectUpdate, projectRemove]\n    milestones: [milestoneRead, milestoneCreate, milestoneUpdate, milestoneRemove]\n    cycles: [cycleRead, cycleCreate, cycleUpdate, cycleRemove, cycleEnd]\n    teams: [teamRead, teamCreate, teamUpdate, teamRemove, teamMemberManage]\n    notes: [noteRead, noteCreate, noteUpdate, noteRemove]\n    statuses: [statusRead, statusCreate, statusUpdate, statusRemove]\ngaps:\n  - >-\n    erxes publishes no consolidated scopes reference page on erxes.io or\n    docs.erxes.io. The only place the scope vocabulary is written down is the\n    agent-plugin reference in the erxes-skills repository.\n  - >-\n    The block plugin ships no permission matrix at all; erxes says so itself\n    under \"Needs Verification\" in block-api.md.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/erxes/refs/heads/main/scopes/erxes-scopes.yml
summary_line: 34 scopes · deviceCode
tags:
- GraphQL
- CRM
- Customer Experience
- Open Source
- Marketing Automation
- Sales Pipeline
- Help Desk
- Ticketing
- Team Inbox
- Self-Hosted
- Apollo Federation
- Project Management
- Knowledge Base
- Webhooks
- Agent Skills
token_urls: []
---
