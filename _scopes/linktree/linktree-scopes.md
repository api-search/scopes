---
authorization_urls:
- https://ciam.linktr.ee/oauth2/v1/apps/agentic/P32ACVpudk8MNftmpf1LR1pW5k8s/MS3C64tMj5Trl5KunDJVudGIMAeGB/authorize
description: ''
docs: https://mcp.linktr.ee/docs
flows:
- authorizationCode
- clientCredentials
- deviceCode
kind: oauth-scopes
layout: scope
method: searched
name: Linktree Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Linktree publishes 30 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Linktree API on a user''s behalf.


  Tokens are issued from https://ciam.linktr.ee/oauth2/v1/apps/agentic/P32ACVpudk8MNftmpf1LR1pW5k8s/MS3C64tMj5Trl5KunDJVudGIMAeGB/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Linktree
provider_slug: linktree
schemes:
- flows:
  - authorizationUrl: https://ciam.linktr.ee/oauth2/v1/apps/agentic/P32ACVpudk8MNftmpf1LR1pW5k8s/MS3C64tMj5Trl5KunDJVudGIMAeGB/authorize
    flow: authorizationCode
    pkce:
    - S256
    tokenUrl: https://ciam.linktr.ee/oauth2/v1/apps/agentic/P32ACVpudk8MNftmpf1LR1pW5k8s/MS3C64tMj5Trl5KunDJVudGIMAeGB/token
  - flow: clientCredentials
    tokenUrl: https://ciam.linktr.ee/oauth2/v1/apps/agentic/P32ACVpudk8MNftmpf1LR1pW5k8s/MS3C64tMj5Trl5KunDJVudGIMAeGB/token
  - deviceAuthorizationUrl: https://ciam.linktr.ee/oauth2/v1/apps/device
    flow: deviceCode
  issuer: https://mcp.linktr.ee
  name: LinktreeMCPOAuth2
  provider: Descope
  source: well-known/linktree-oauth-authorization-server.json
  type: oauth2
scope_count: 30
scope_names:
- mcp:list_accessible_profiles
- mcp:set_active_profile
- mcp:get_account
- mcp:update_account_profile
- mcp:get_suggested_bio
- mcp:get_account_analytics
- mcp:get_analytics_lifetime_totals
- mcp:get_top_links
- mcp:get_profile_views
- mcp:get_social_integrations
- mcp:get_appearance
- mcp:update_appearance
- mcp:get_knowledge_base
- mcp:get_workspaces_for_user
- mcp:get_workspace
- mcp:get_workspace_profiles
- mcp:get_workspace_profiles_analytics
- mcp:get_workspace_members
- mcp:get_links
- mcp:add_link
- mcp:create_collection
- mcp:add_links_to_collection
- mcp:update_link
- mcp:reorder_link
- mcp:delete_link
- mcp:get_link_analytics
- mcp:get_social_links
- mcp:upsert_social_link
- mcp:reorder_social_links
- mcp:delete_social_link
scopes:
- description: Retrieve every Linktree profile the authenticated user can access across direct accounts and workspaces.
  flows:
  - authorizationCode
  scope: mcp:list_accessible_profiles
- description: Set the active Linktree profile for the current conversation so later tools target it.
  flows:
  - authorizationCode
  scope: mcp:set_active_profile
- description: Retrieve a Linktree profile's details (display name, bio, avatar, username).
  flows:
  - authorizationCode
  scope: mcp:get_account
- description: Update a Linktree profile's display name and/or bio.
  flows:
  - authorizationCode
  scope: mcp:update_account_profile
- description: Retrieve a suggested bio for a Linktree profile based on its existing content.
  flows:
  - authorizationCode
  scope: mcp:get_suggested_bio
- description: Retrieve account-level analytics for a Linktree profile (views, clicks, CTR, and optional breakdowns).
  flows:
  - authorizationCode
  scope: mcp:get_account_analytics
- description: Retrieve lifetime analytics totals for a Linktree profile (views, clicks, CTR, earnings).
  flows:
  - authorizationCode
  scope: mcp:get_analytics_lifetime_totals
- description: Retrieve every link on a Linktree profile ranked by clicks, including links with zero clicks.
  flows:
  - authorizationCode
  scope: mcp:get_top_links
- description: Retrieve profile view counts for a Linktree profile over a recent time window.
  flows:
  - authorizationCode
  scope: mcp:get_profile_views
- description: Retrieve the active social integrations connected to a Linktree profile.
  flows:
  - authorizationCode
  scope: mcp:get_social_integrations
- description: Retrieve a Linktree profile's appearance settings (colors, fonts, button styles, background).
  flows:
  - authorizationCode
  scope: mcp:get_appearance
- description: Update a Linktree profile's appearance (colors, fonts, button styles, background).
  flows:
  - authorizationCode
  scope: mcp:update_appearance
- description: Retrieve a Linktree profile's knowledge base entries (business, product, policy, or FAQ information).
  flows:
  - authorizationCode
  scope: mcp:get_knowledge_base
- description: Retrieve every workspace the authenticated user is a member of.
  flows:
  - authorizationCode
  scope: mcp:get_workspaces_for_user
- description: Retrieve details for a workspace the authenticated user belongs to.
  flows:
  - authorizationCode
  scope: mcp:get_workspace
- description: Retrieve every Linktree profile belonging to a workspace.
  flows:
  - authorizationCode
  scope: mcp:get_workspace_profiles
- description: Retrieve lifetime analytics for every Linktree profile in a workspace.
  flows:
  - authorizationCode
  scope: mcp:get_workspace_profiles_analytics
- description: Retrieve the members of a workspace.
  flows:
  - authorizationCode
  scope: mcp:get_workspace_members
- description: Retrieve the ordered links on a Linktree profile, including link-app metadata.
  flows:
  - authorizationCode
  scope: mcp:get_links
- description: Add a new URL-backed link to a Linktree profile.
  flows:
  - authorizationCode
  scope: mcp:add_link
- description: Create a new empty collection on a Linktree profile.
  flows:
  - authorizationCode
  scope: mcp:create_collection
- description: Move existing top-level links into a collection on a Linktree profile.
  flows:
  - authorizationCode
  scope: mcp:add_links_to_collection
- description: Update an existing link or collection on a Linktree profile (title, URL, or active state).
  flows:
  - authorizationCode
  scope: mcp:update_link
- description: Reorder a top-level link, collection, or collection item on a Linktree profile.
  flows:
  - authorizationCode
  scope: mcp:reorder_link
- description: Delete a top-level link from a Linktree profile.
  flows:
  - authorizationCode
  scope: mcp:delete_link
- description: Retrieve analytics for a specific link on a Linktree profile (clicks, views, CTR, trend data).
  flows:
  - authorizationCode
  scope: mcp:get_link_analytics
- description: Retrieve a Linktree profile's social icon links and their display order.
  flows:
  - authorizationCode
  scope: mcp:get_social_links
- description: Create or update a social icon link on a Linktree profile for a supported platform.
  flows:
  - authorizationCode
  scope: mcp:upsert_social_link
- description: Move a social icon link to a new position on a Linktree profile.
  flows:
  - authorizationCode
  scope: mcp:reorder_social_links
- description: Delete a social icon link from a Linktree profile by platform type.
  flows:
  - authorizationCode
  scope: mcp:delete_social_link
slug: linktree-scopes
source_filename: linktree-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "# OAuth scopes for the Linktree MCP server. One scope per tool.\ngenerated: '2026-07-19'\nmethod: searched\nsource: https://mcp.linktr.ee/.well-known/mcp/tools.json\ndocs: https://mcp.linktr.ee/docs\nschemes:\n  - name: LinktreeMCPOAuth2\n    type: oauth2\n    provider: Descope\n    source: well-known/linktree-oauth-authorization-server.json\n    issuer: https://mcp.linktr.ee\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://ciam.linktr.ee/oauth2/v1/apps/agentic/P32ACVpudk8MNftmpf1LR1pW5k8s/MS3C64tMj5Trl5KunDJVudGIMAeGB/authorize\n        tokenUrl: https://ciam.linktr.ee/oauth2/v1/apps/agentic/P32ACVpudk8MNftmpf1LR1pW5k8s/MS3C64tMj5Trl5KunDJVudGIMAeGB/token\n        pkce: [S256]\n      - flow: clientCredentials\n        tokenUrl: https://ciam.linktr.ee/oauth2/v1/apps/agentic/P32ACVpudk8MNftmpf1LR1pW5k8s/MS3C64tMj5Trl5KunDJVudGIMAeGB/token\n      - flow: deviceCode\n        deviceAuthorizationUrl: https://ciam.linktr.ee/oauth2/v1/apps/device\nscope_count:\
  \ 30\nscopes:\n  - scope: mcp:list_accessible_profiles\n    description: \"Retrieve every Linktree profile the authenticated user can access across direct accounts and workspaces.\"\n    access: read\n    flows: [authorizationCode]\n    sources: [mcp/linktree-mcp-tools.json]\n  - scope: mcp:set_active_profile\n    description: \"Set the active Linktree profile for the current conversation so later tools target it.\"\n    access: read\n    flows: [authorizationCode]\n    sources: [mcp/linktree-mcp-tools.json]\n  - scope: mcp:get_account\n    description: \"Retrieve a Linktree profile's details (display name, bio, avatar, username).\"\n    access: read\n    flows: [authorizationCode]\n    sources: [mcp/linktree-mcp-tools.json]\n  - scope: mcp:update_account_profile\n    description: \"Update a Linktree profile's display name and/or bio.\"\n    access: write\n    flows: [authorizationCode]\n    sources: [mcp/linktree-mcp-tools.json]\n  - scope: mcp:get_suggested_bio\n    description: \"Retrieve\
  \ a suggested bio for a Linktree profile based on its existing content.\"\n    access: read\n    flows: [authorizationCode]\n    sources: [mcp/linktree-mcp-tools.json]\n  - scope: mcp:get_account_analytics\n    description: \"Retrieve account-level analytics for a Linktree profile (views, clicks, CTR, and optional breakdowns).\"\n    access: read\n    flows: [authorizationCode]\n    sources: [mcp/linktree-mcp-tools.json]\n  - scope: mcp:get_analytics_lifetime_totals\n    description: \"Retrieve lifetime analytics totals for a Linktree profile (views, clicks, CTR, earnings).\"\n    access: read\n    flows: [authorizationCode]\n    sources: [mcp/linktree-mcp-tools.json]\n  - scope: mcp:get_top_links\n    description: \"Retrieve every link on a Linktree profile ranked by clicks, including links with zero clicks.\"\n    access: read\n    flows: [authorizationCode]\n    sources: [mcp/linktree-mcp-tools.json]\n  - scope: mcp:get_profile_views\n    description: \"Retrieve profile view counts\
  \ for a Linktree profile over a recent time window.\"\n    access: read\n    flows: [authorizationCode]\n    sources: [mcp/linktree-mcp-tools.json]\n  - scope: mcp:get_social_integrations\n    description: \"Retrieve the active social integrations connected to a Linktree profile.\"\n    access: read\n    flows: [authorizationCode]\n    sources: [mcp/linktree-mcp-tools.json]\n  - scope: mcp:get_appearance\n    description: \"Retrieve a Linktree profile's appearance settings (colors, fonts, button styles, background).\"\n    access: read\n    flows: [authorizationCode]\n    sources: [mcp/linktree-mcp-tools.json]\n  - scope: mcp:update_appearance\n    description: \"Update a Linktree profile's appearance (colors, fonts, button styles, background).\"\n    access: write\n    flows: [authorizationCode]\n    sources: [mcp/linktree-mcp-tools.json]\n  - scope: mcp:get_knowledge_base\n    description: \"Retrieve a Linktree profile's knowledge base entries (business, product, policy, or FAQ information).\"\
  \n    access: read\n    flows: [authorizationCode]\n    sources: [mcp/linktree-mcp-tools.json]\n  - scope: mcp:get_workspaces_for_user\n    description: \"Retrieve every workspace the authenticated user is a member of.\"\n    access: read\n    flows: [authorizationCode]\n    sources: [mcp/linktree-mcp-tools.json]\n  - scope: mcp:get_workspace\n    description: \"Retrieve details for a workspace the authenticated user belongs to.\"\n    access: read\n    flows: [authorizationCode]\n    sources: [mcp/linktree-mcp-tools.json]\n  - scope: mcp:get_workspace_profiles\n    description: \"Retrieve every Linktree profile belonging to a workspace.\"\n    access: read\n    flows: [authorizationCode]\n    sources: [mcp/linktree-mcp-tools.json]\n  - scope: mcp:get_workspace_profiles_analytics\n    description: \"Retrieve lifetime analytics for every Linktree profile in a workspace.\"\n    access: read\n    flows: [authorizationCode]\n    sources: [mcp/linktree-mcp-tools.json]\n  - scope: mcp:get_workspace_members\n\
  \    description: \"Retrieve the members of a workspace.\"\n    access: read\n    flows: [authorizationCode]\n    sources: [mcp/linktree-mcp-tools.json]\n  - scope: mcp:get_links\n    description: \"Retrieve the ordered links on a Linktree profile, including link-app metadata.\"\n    access: read\n    flows: [authorizationCode]\n    sources: [mcp/linktree-mcp-tools.json]\n  - scope: mcp:add_link\n    description: \"Add a new URL-backed link to a Linktree profile.\"\n    access: write\n    flows: [authorizationCode]\n    sources: [mcp/linktree-mcp-tools.json]\n  - scope: mcp:create_collection\n    description: \"Create a new empty collection on a Linktree profile.\"\n    access: write\n    flows: [authorizationCode]\n    sources: [mcp/linktree-mcp-tools.json]\n  - scope: mcp:add_links_to_collection\n    description: \"Move existing top-level links into a collection on a Linktree profile.\"\n    access: write\n    flows: [authorizationCode]\n    sources: [mcp/linktree-mcp-tools.json]\n \
  \ - scope: mcp:update_link\n    description: \"Update an existing link or collection on a Linktree profile (title, URL, or active state).\"\n    access: write\n    flows: [authorizationCode]\n    sources: [mcp/linktree-mcp-tools.json]\n  - scope: mcp:reorder_link\n    description: \"Reorder a top-level link, collection, or collection item on a Linktree profile.\"\n    access: write\n    flows: [authorizationCode]\n    sources: [mcp/linktree-mcp-tools.json]\n  - scope: mcp:delete_link\n    description: \"Delete a top-level link from a Linktree profile.\"\n    access: destructive\n    flows: [authorizationCode]\n    sources: [mcp/linktree-mcp-tools.json]\n  - scope: mcp:get_link_analytics\n    description: \"Retrieve analytics for a specific link on a Linktree profile (clicks, views, CTR, trend data).\"\n    access: read\n    flows: [authorizationCode]\n    sources: [mcp/linktree-mcp-tools.json]\n  - scope: mcp:get_social_links\n    description: \"Retrieve a Linktree profile's social icon\
  \ links and their display order.\"\n    access: read\n    flows: [authorizationCode]\n    sources: [mcp/linktree-mcp-tools.json]\n  - scope: mcp:upsert_social_link\n    description: \"Create or update a social icon link on a Linktree profile for a supported platform.\"\n    access: write\n    flows: [authorizationCode]\n    sources: [mcp/linktree-mcp-tools.json]\n  - scope: mcp:reorder_social_links\n    description: \"Move a social icon link to a new position on a Linktree profile.\"\n    access: write\n    flows: [authorizationCode]\n    sources: [mcp/linktree-mcp-tools.json]\n  - scope: mcp:delete_social_link\n    description: \"Delete a social icon link from a Linktree profile by platform type.\"\n    access: destructive\n    flows: [authorizationCode]\n    sources: [mcp/linktree-mcp-tools.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linktree/refs/heads/main/scopes/linktree-scopes.yml
summary_line: 30 scopes · authorizationCode/clientCredentials/deviceCode
tags:
- Company
- Media
- Link in Bio
- Creator Economy
- Social Media
- Marketing
- Analytics
- MCP
- Agents
token_urls:
- https://ciam.linktr.ee/oauth2/v1/apps/agentic/P32ACVpudk8MNftmpf1LR1pW5k8s/MS3C64tMj5Trl5KunDJVudGIMAeGB/token
---
