---
api_specs:
- filename: ccp-games-esi-openapi-original.json
  format: json
  label: EVE Swagger Interface (ESI)
  slug: eve-swagger-interface-esi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ccp-games/refs/heads/main/openapi/ccp-games-esi-openapi-original.json
authorization_urls:
- https://login.eveonline.com/v2/oauth/authorize
description: ''
docs: https://docs.esi.evetech.net/docs/sso/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Ccp Games Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'CCP Games publishes 70 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the CCP Games API on a user''s behalf.


  Tokens are issued from https://login.eveonline.com/v2/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CCP Games
provider_slug: ccp-games
schemes:
- flows:
  - authorizationUrl: https://login.eveonline.com/v2/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://login.eveonline.com/v2/oauth/token
  name: OAuth2
  source: openapi/ccp-games-esi-openapi-original.json
scope_count: 70
scope_names:
- esi-access.read_lists.v1
- esi-activities.read_character.v1
- esi-alliances.read_contacts.v1
- esi-assets.read_assets.v1
- esi-assets.read_corporation_assets.v1
- esi-calendar.read_calendar_events.v1
- esi-calendar.respond_calendar_events.v1
- esi-characters.read_agents_research.v1
- esi-characters.read_blueprints.v1
- esi-characters.read_contacts.v1
- esi-characters.read_corporation_roles.v1
- esi-characters.read_fatigue.v1
- esi-characters.read_freelance_jobs.v1
- esi-characters.read_fw_stats.v1
- esi-characters.read_loyalty.v1
- esi-characters.read_medals.v1
- esi-characters.read_notifications.v1
- esi-characters.read_standings.v1
- esi-characters.read_titles.v1
- esi-characters.write_contacts.v1
- esi-clones.read_clones.v1
- esi-clones.read_implants.v1
- esi-contracts.read_character_contracts.v1
- esi-contracts.read_corporation_contracts.v1
- esi-corporations.read_blueprints.v1
- esi-corporations.read_contacts.v1
- esi-corporations.read_container_logs.v1
- esi-corporations.read_corporation_membership.v1
- esi-corporations.read_divisions.v1
- esi-corporations.read_facilities.v1
- esi-corporations.read_freelance_jobs.v1
- esi-corporations.read_fw_stats.v1
- esi-corporations.read_medals.v1
- esi-corporations.read_projects.v1
- esi-corporations.read_standings.v1
- esi-corporations.read_starbases.v1
- esi-corporations.read_structures.v1
- esi-corporations.read_titles.v1
- esi-corporations.track_members.v1
- esi-fittings.read_fittings.v1
- esi-fittings.write_fittings.v1
- esi-fleets.read_fleet.v1
- esi-fleets.write_fleet.v1
- esi-industry.read_character_jobs.v1
- esi-industry.read_character_mining.v1
- esi-industry.read_corporation_jobs.v1
- esi-industry.read_corporation_mining.v1
- esi-killmails.read_corporation_killmails.v1
- esi-killmails.read_killmails.v1
- esi-location.read_location.v1
- esi-location.read_online.v1
- esi-location.read_ship_type.v1
- esi-mail.organize_mail.v1
- esi-mail.read_mail.v1
- esi-mail.send_mail.v1
- esi-markets.read_character_orders.v1
- esi-markets.read_corporation_orders.v1
- esi-markets.structure_markets.v1
- esi-planets.manage_planets.v1
- esi-planets.read_customs_offices.v1
- esi-search.search_structures.v1
- esi-skills.read_skillqueue.v1
- esi-skills.read_skills.v1
- esi-structures.read_character.v1
- esi-structures.read_corporation.v1
- esi-ui.open_window.v1
- esi-ui.write_waypoint.v1
- esi-universe.read_structures.v1
- esi-wallet.read_character_wallet.v1
- esi-wallet.read_corporation_wallets.v1
scopes:
- description: esi-access.read_lists.v1
  flows:
  - authorizationCode
  scope: esi-access.read_lists.v1
- description: esi-activities.read_character.v1
  flows:
  - authorizationCode
  scope: esi-activities.read_character.v1
- description: esi-alliances.read_contacts.v1
  flows:
  - authorizationCode
  scope: esi-alliances.read_contacts.v1
- description: esi-assets.read_assets.v1
  flows:
  - authorizationCode
  scope: esi-assets.read_assets.v1
- description: esi-assets.read_corporation_assets.v1
  flows:
  - authorizationCode
  scope: esi-assets.read_corporation_assets.v1
- description: esi-calendar.read_calendar_events.v1
  flows:
  - authorizationCode
  scope: esi-calendar.read_calendar_events.v1
- description: esi-calendar.respond_calendar_events.v1
  flows:
  - authorizationCode
  scope: esi-calendar.respond_calendar_events.v1
- description: esi-characters.read_agents_research.v1
  flows:
  - authorizationCode
  scope: esi-characters.read_agents_research.v1
- description: esi-characters.read_blueprints.v1
  flows:
  - authorizationCode
  scope: esi-characters.read_blueprints.v1
- description: esi-characters.read_contacts.v1
  flows:
  - authorizationCode
  scope: esi-characters.read_contacts.v1
- description: esi-characters.read_corporation_roles.v1
  flows:
  - authorizationCode
  scope: esi-characters.read_corporation_roles.v1
- description: esi-characters.read_fatigue.v1
  flows:
  - authorizationCode
  scope: esi-characters.read_fatigue.v1
- description: esi-characters.read_freelance_jobs.v1
  flows:
  - authorizationCode
  scope: esi-characters.read_freelance_jobs.v1
- description: esi-characters.read_fw_stats.v1
  flows:
  - authorizationCode
  scope: esi-characters.read_fw_stats.v1
- description: esi-characters.read_loyalty.v1
  flows:
  - authorizationCode
  scope: esi-characters.read_loyalty.v1
- description: esi-characters.read_medals.v1
  flows:
  - authorizationCode
  scope: esi-characters.read_medals.v1
- description: esi-characters.read_notifications.v1
  flows:
  - authorizationCode
  scope: esi-characters.read_notifications.v1
- description: esi-characters.read_standings.v1
  flows:
  - authorizationCode
  scope: esi-characters.read_standings.v1
- description: esi-characters.read_titles.v1
  flows:
  - authorizationCode
  scope: esi-characters.read_titles.v1
- description: esi-characters.write_contacts.v1
  flows:
  - authorizationCode
  scope: esi-characters.write_contacts.v1
- description: esi-clones.read_clones.v1
  flows:
  - authorizationCode
  scope: esi-clones.read_clones.v1
- description: esi-clones.read_implants.v1
  flows:
  - authorizationCode
  scope: esi-clones.read_implants.v1
- description: esi-contracts.read_character_contracts.v1
  flows:
  - authorizationCode
  scope: esi-contracts.read_character_contracts.v1
- description: esi-contracts.read_corporation_contracts.v1
  flows:
  - authorizationCode
  scope: esi-contracts.read_corporation_contracts.v1
- description: esi-corporations.read_blueprints.v1
  flows:
  - authorizationCode
  scope: esi-corporations.read_blueprints.v1
- description: esi-corporations.read_contacts.v1
  flows:
  - authorizationCode
  scope: esi-corporations.read_contacts.v1
- description: esi-corporations.read_container_logs.v1
  flows:
  - authorizationCode
  scope: esi-corporations.read_container_logs.v1
- description: esi-corporations.read_corporation_membership.v1
  flows:
  - authorizationCode
  scope: esi-corporations.read_corporation_membership.v1
- description: esi-corporations.read_divisions.v1
  flows:
  - authorizationCode
  scope: esi-corporations.read_divisions.v1
- description: esi-corporations.read_facilities.v1
  flows:
  - authorizationCode
  scope: esi-corporations.read_facilities.v1
- description: esi-corporations.read_freelance_jobs.v1
  flows:
  - authorizationCode
  scope: esi-corporations.read_freelance_jobs.v1
- description: esi-corporations.read_fw_stats.v1
  flows:
  - authorizationCode
  scope: esi-corporations.read_fw_stats.v1
- description: esi-corporations.read_medals.v1
  flows:
  - authorizationCode
  scope: esi-corporations.read_medals.v1
- description: esi-corporations.read_projects.v1
  flows:
  - authorizationCode
  scope: esi-corporations.read_projects.v1
- description: esi-corporations.read_standings.v1
  flows:
  - authorizationCode
  scope: esi-corporations.read_standings.v1
- description: esi-corporations.read_starbases.v1
  flows:
  - authorizationCode
  scope: esi-corporations.read_starbases.v1
- description: esi-corporations.read_structures.v1
  flows:
  - authorizationCode
  scope: esi-corporations.read_structures.v1
- description: esi-corporations.read_titles.v1
  flows:
  - authorizationCode
  scope: esi-corporations.read_titles.v1
- description: esi-corporations.track_members.v1
  flows:
  - authorizationCode
  scope: esi-corporations.track_members.v1
- description: esi-fittings.read_fittings.v1
  flows:
  - authorizationCode
  scope: esi-fittings.read_fittings.v1
- description: esi-fittings.write_fittings.v1
  flows:
  - authorizationCode
  scope: esi-fittings.write_fittings.v1
- description: esi-fleets.read_fleet.v1
  flows:
  - authorizationCode
  scope: esi-fleets.read_fleet.v1
- description: esi-fleets.write_fleet.v1
  flows:
  - authorizationCode
  scope: esi-fleets.write_fleet.v1
- description: esi-industry.read_character_jobs.v1
  flows:
  - authorizationCode
  scope: esi-industry.read_character_jobs.v1
- description: esi-industry.read_character_mining.v1
  flows:
  - authorizationCode
  scope: esi-industry.read_character_mining.v1
- description: esi-industry.read_corporation_jobs.v1
  flows:
  - authorizationCode
  scope: esi-industry.read_corporation_jobs.v1
- description: esi-industry.read_corporation_mining.v1
  flows:
  - authorizationCode
  scope: esi-industry.read_corporation_mining.v1
- description: esi-killmails.read_corporation_killmails.v1
  flows:
  - authorizationCode
  scope: esi-killmails.read_corporation_killmails.v1
- description: esi-killmails.read_killmails.v1
  flows:
  - authorizationCode
  scope: esi-killmails.read_killmails.v1
- description: esi-location.read_location.v1
  flows:
  - authorizationCode
  scope: esi-location.read_location.v1
- description: esi-location.read_online.v1
  flows:
  - authorizationCode
  scope: esi-location.read_online.v1
- description: esi-location.read_ship_type.v1
  flows:
  - authorizationCode
  scope: esi-location.read_ship_type.v1
- description: esi-mail.organize_mail.v1
  flows:
  - authorizationCode
  scope: esi-mail.organize_mail.v1
- description: esi-mail.read_mail.v1
  flows:
  - authorizationCode
  scope: esi-mail.read_mail.v1
- description: esi-mail.send_mail.v1
  flows:
  - authorizationCode
  scope: esi-mail.send_mail.v1
- description: esi-markets.read_character_orders.v1
  flows:
  - authorizationCode
  scope: esi-markets.read_character_orders.v1
- description: esi-markets.read_corporation_orders.v1
  flows:
  - authorizationCode
  scope: esi-markets.read_corporation_orders.v1
- description: esi-markets.structure_markets.v1
  flows:
  - authorizationCode
  scope: esi-markets.structure_markets.v1
- description: esi-planets.manage_planets.v1
  flows:
  - authorizationCode
  scope: esi-planets.manage_planets.v1
- description: esi-planets.read_customs_offices.v1
  flows:
  - authorizationCode
  scope: esi-planets.read_customs_offices.v1
- description: esi-search.search_structures.v1
  flows:
  - authorizationCode
  scope: esi-search.search_structures.v1
- description: esi-skills.read_skillqueue.v1
  flows:
  - authorizationCode
  scope: esi-skills.read_skillqueue.v1
- description: esi-skills.read_skills.v1
  flows:
  - authorizationCode
  scope: esi-skills.read_skills.v1
- description: esi-structures.read_character.v1
  flows:
  - authorizationCode
  scope: esi-structures.read_character.v1
- description: esi-structures.read_corporation.v1
  flows:
  - authorizationCode
  scope: esi-structures.read_corporation.v1
- description: esi-ui.open_window.v1
  flows:
  - authorizationCode
  scope: esi-ui.open_window.v1
- description: esi-ui.write_waypoint.v1
  flows:
  - authorizationCode
  scope: esi-ui.write_waypoint.v1
- description: esi-universe.read_structures.v1
  flows:
  - authorizationCode
  scope: esi-universe.read_structures.v1
- description: esi-wallet.read_character_wallet.v1
  flows:
  - authorizationCode
  scope: esi-wallet.read_character_wallet.v1
- description: esi-wallet.read_corporation_wallets.v1
  flows:
  - authorizationCode
  scope: esi-wallet.read_corporation_wallets.v1
slug: ccp-games-scopes
source_filename: ccp-games-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/ccp-games-esi-openapi-original.json\nschemes:\n- name: OAuth2\n  source: openapi/ccp-games-esi-openapi-original.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.eveonline.com/v2/oauth/authorize\n    tokenUrl: https://login.eveonline.com/v2/oauth/token\nscopes:\n- scope: esi-access.read_lists.v1\n  description: esi-access.read_lists.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-activities.read_character.v1\n  description: esi-activities.read_character.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-alliances.read_contacts.v1\n  description: esi-alliances.read_contacts.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-assets.read_assets.v1\n  description: esi-assets.read_assets.v1\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-assets.read_corporation_assets.v1\n  description: esi-assets.read_corporation_assets.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-calendar.read_calendar_events.v1\n  description: esi-calendar.read_calendar_events.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-calendar.respond_calendar_events.v1\n  description: esi-calendar.respond_calendar_events.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-characters.read_agents_research.v1\n  description: esi-characters.read_agents_research.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-characters.read_blueprints.v1\n  description: esi-characters.read_blueprints.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n\
  - scope: esi-characters.read_contacts.v1\n  description: esi-characters.read_contacts.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-characters.read_corporation_roles.v1\n  description: esi-characters.read_corporation_roles.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-characters.read_fatigue.v1\n  description: esi-characters.read_fatigue.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-characters.read_freelance_jobs.v1\n  description: esi-characters.read_freelance_jobs.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-characters.read_fw_stats.v1\n  description: esi-characters.read_fw_stats.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-characters.read_loyalty.v1\n  description:\
  \ esi-characters.read_loyalty.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-characters.read_medals.v1\n  description: esi-characters.read_medals.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-characters.read_notifications.v1\n  description: esi-characters.read_notifications.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-characters.read_standings.v1\n  description: esi-characters.read_standings.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-characters.read_titles.v1\n  description: esi-characters.read_titles.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-characters.write_contacts.v1\n  description: esi-characters.write_contacts.v1\n  flows:\n  - authorizationCode\n  sources:\n\
  \  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-clones.read_clones.v1\n  description: esi-clones.read_clones.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-clones.read_implants.v1\n  description: esi-clones.read_implants.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-contracts.read_character_contracts.v1\n  description: esi-contracts.read_character_contracts.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-contracts.read_corporation_contracts.v1\n  description: esi-contracts.read_corporation_contracts.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-corporations.read_blueprints.v1\n  description: esi-corporations.read_blueprints.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n\
  - scope: esi-corporations.read_contacts.v1\n  description: esi-corporations.read_contacts.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-corporations.read_container_logs.v1\n  description: esi-corporations.read_container_logs.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-corporations.read_corporation_membership.v1\n  description: esi-corporations.read_corporation_membership.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-corporations.read_divisions.v1\n  description: esi-corporations.read_divisions.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-corporations.read_facilities.v1\n  description: esi-corporations.read_facilities.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-corporations.read_freelance_jobs.v1\n\
  \  description: esi-corporations.read_freelance_jobs.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-corporations.read_fw_stats.v1\n  description: esi-corporations.read_fw_stats.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-corporations.read_medals.v1\n  description: esi-corporations.read_medals.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-corporations.read_projects.v1\n  description: esi-corporations.read_projects.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-corporations.read_standings.v1\n  description: esi-corporations.read_standings.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-corporations.read_starbases.v1\n  description: esi-corporations.read_starbases.v1\n  flows:\n\
  \  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-corporations.read_structures.v1\n  description: esi-corporations.read_structures.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-corporations.read_titles.v1\n  description: esi-corporations.read_titles.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-corporations.track_members.v1\n  description: esi-corporations.track_members.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-fittings.read_fittings.v1\n  description: esi-fittings.read_fittings.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-fittings.write_fittings.v1\n  description: esi-fittings.write_fittings.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n\
  - scope: esi-fleets.read_fleet.v1\n  description: esi-fleets.read_fleet.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-fleets.write_fleet.v1\n  description: esi-fleets.write_fleet.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-industry.read_character_jobs.v1\n  description: esi-industry.read_character_jobs.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-industry.read_character_mining.v1\n  description: esi-industry.read_character_mining.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-industry.read_corporation_jobs.v1\n  description: esi-industry.read_corporation_jobs.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-industry.read_corporation_mining.v1\n  description: esi-industry.read_corporation_mining.v1\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-killmails.read_corporation_killmails.v1\n  description: esi-killmails.read_corporation_killmails.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-killmails.read_killmails.v1\n  description: esi-killmails.read_killmails.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-location.read_location.v1\n  description: esi-location.read_location.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-location.read_online.v1\n  description: esi-location.read_online.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-location.read_ship_type.v1\n  description: esi-location.read_ship_type.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n\
  - scope: esi-mail.organize_mail.v1\n  description: esi-mail.organize_mail.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-mail.read_mail.v1\n  description: esi-mail.read_mail.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-mail.send_mail.v1\n  description: esi-mail.send_mail.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-markets.read_character_orders.v1\n  description: esi-markets.read_character_orders.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-markets.read_corporation_orders.v1\n  description: esi-markets.read_corporation_orders.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-markets.structure_markets.v1\n  description: esi-markets.structure_markets.v1\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-planets.manage_planets.v1\n  description: esi-planets.manage_planets.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-planets.read_customs_offices.v1\n  description: esi-planets.read_customs_offices.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-search.search_structures.v1\n  description: esi-search.search_structures.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-skills.read_skillqueue.v1\n  description: esi-skills.read_skillqueue.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-skills.read_skills.v1\n  description: esi-skills.read_skills.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-structures.read_character.v1\n\
  \  description: esi-structures.read_character.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-structures.read_corporation.v1\n  description: esi-structures.read_corporation.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-ui.open_window.v1\n  description: esi-ui.open_window.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-ui.write_waypoint.v1\n  description: esi-ui.write_waypoint.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-universe.read_structures.v1\n  description: esi-universe.read_structures.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n- scope: esi-wallet.read_character_wallet.v1\n  description: esi-wallet.read_character_wallet.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\n\
  - scope: esi-wallet.read_corporation_wallets.v1\n  description: esi-wallet.read_corporation_wallets.v1\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ccp-games-esi-openapi-original.json\ndocs: https://docs.esi.evetech.net/docs/sso/\nscope_selection: https://developers.eveonline.com/applications (scopes chosen per\n  application)\noidc:\n  issuer: https://login.eveonline.com\n  authorization_endpoint: https://login.eveonline.com/v2/oauth/authorize\n  token_endpoint: https://login.eveonline.com/v2/oauth/token\n  pkce: S256\n  discovery: https://login.eveonline.com/.well-known/openid-configuration\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ccp-games/refs/heads/main/scopes/ccp-games-scopes.yml
summary_line: 70 scopes · authorizationCode
tags:
- Company
- Gaming
- Games
- MMO
- EVE Online
- Developer Platform
- OAuth
- OpenID Connect
- Player Data
- Virtual Economy
token_urls:
- https://login.eveonline.com/v2/oauth/token
---
