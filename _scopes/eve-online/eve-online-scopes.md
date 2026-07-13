---
api_specs:
- filename: swagger.json
  format: json
  label: EVE Swagger Interface (ESI)
  slug: eve-swagger-interface
  spec_type: OpenAPI
  url: https://esi.evetech.net/latest/swagger.json
authorization_urls:
- https://login.eveonline.com/v2/oauth/authorize
description: ''
docs: ''
flows:
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Eve Online Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'EVE Online publishes 63 OAuth 2.0 scopes via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the EVE Online API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: EVE Online
provider_slug: eve-online
schemes:
- flows:
  - authorizationUrl: https://login.eveonline.com/v2/oauth/authorize
    flow: implicit
  name: evesso
  source: openapi/eve-online-openapi.yml
scope_count: 63
scope_names:
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
- esi-corporations.read_fw_stats.v1
- esi-corporations.read_medals.v1
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
- esi-ui.open_window.v1
- esi-ui.write_waypoint.v1
- esi-universe.read_structures.v1
- esi-wallet.read_character_wallet.v1
- esi-wallet.read_corporation_wallets.v1
scopes:
- description: EVE SSO scope esi-alliances.read_contacts.v1
  flows:
  - implicit
  scope: esi-alliances.read_contacts.v1
- description: EVE SSO scope esi-assets.read_assets.v1
  flows:
  - implicit
  scope: esi-assets.read_assets.v1
- description: EVE SSO scope esi-assets.read_corporation_assets.v1
  flows:
  - implicit
  scope: esi-assets.read_corporation_assets.v1
- description: EVE SSO scope esi-calendar.read_calendar_events.v1
  flows:
  - implicit
  scope: esi-calendar.read_calendar_events.v1
- description: EVE SSO scope esi-calendar.respond_calendar_events.v1
  flows:
  - implicit
  scope: esi-calendar.respond_calendar_events.v1
- description: EVE SSO scope esi-characters.read_agents_research.v1
  flows:
  - implicit
  scope: esi-characters.read_agents_research.v1
- description: EVE SSO scope esi-characters.read_blueprints.v1
  flows:
  - implicit
  scope: esi-characters.read_blueprints.v1
- description: EVE SSO scope esi-characters.read_contacts.v1
  flows:
  - implicit
  scope: esi-characters.read_contacts.v1
- description: EVE SSO scope esi-characters.read_corporation_roles.v1
  flows:
  - implicit
  scope: esi-characters.read_corporation_roles.v1
- description: EVE SSO scope esi-characters.read_fatigue.v1
  flows:
  - implicit
  scope: esi-characters.read_fatigue.v1
- description: EVE SSO scope esi-characters.read_fw_stats.v1
  flows:
  - implicit
  scope: esi-characters.read_fw_stats.v1
- description: EVE SSO scope esi-characters.read_loyalty.v1
  flows:
  - implicit
  scope: esi-characters.read_loyalty.v1
- description: EVE SSO scope esi-characters.read_medals.v1
  flows:
  - implicit
  scope: esi-characters.read_medals.v1
- description: EVE SSO scope esi-characters.read_notifications.v1
  flows:
  - implicit
  scope: esi-characters.read_notifications.v1
- description: EVE SSO scope esi-characters.read_standings.v1
  flows:
  - implicit
  scope: esi-characters.read_standings.v1
- description: EVE SSO scope esi-characters.read_titles.v1
  flows:
  - implicit
  scope: esi-characters.read_titles.v1
- description: EVE SSO scope esi-characters.write_contacts.v1
  flows:
  - implicit
  scope: esi-characters.write_contacts.v1
- description: EVE SSO scope esi-clones.read_clones.v1
  flows:
  - implicit
  scope: esi-clones.read_clones.v1
- description: EVE SSO scope esi-clones.read_implants.v1
  flows:
  - implicit
  scope: esi-clones.read_implants.v1
- description: EVE SSO scope esi-contracts.read_character_contracts.v1
  flows:
  - implicit
  scope: esi-contracts.read_character_contracts.v1
- description: EVE SSO scope esi-contracts.read_corporation_contracts.v1
  flows:
  - implicit
  scope: esi-contracts.read_corporation_contracts.v1
- description: EVE SSO scope esi-corporations.read_blueprints.v1
  flows:
  - implicit
  scope: esi-corporations.read_blueprints.v1
- description: EVE SSO scope esi-corporations.read_contacts.v1
  flows:
  - implicit
  scope: esi-corporations.read_contacts.v1
- description: EVE SSO scope esi-corporations.read_container_logs.v1
  flows:
  - implicit
  scope: esi-corporations.read_container_logs.v1
- description: EVE SSO scope esi-corporations.read_corporation_membership.v1
  flows:
  - implicit
  scope: esi-corporations.read_corporation_membership.v1
- description: EVE SSO scope esi-corporations.read_divisions.v1
  flows:
  - implicit
  scope: esi-corporations.read_divisions.v1
- description: EVE SSO scope esi-corporations.read_facilities.v1
  flows:
  - implicit
  scope: esi-corporations.read_facilities.v1
- description: EVE SSO scope esi-corporations.read_fw_stats.v1
  flows:
  - implicit
  scope: esi-corporations.read_fw_stats.v1
- description: EVE SSO scope esi-corporations.read_medals.v1
  flows:
  - implicit
  scope: esi-corporations.read_medals.v1
- description: EVE SSO scope esi-corporations.read_standings.v1
  flows:
  - implicit
  scope: esi-corporations.read_standings.v1
- description: EVE SSO scope esi-corporations.read_starbases.v1
  flows:
  - implicit
  scope: esi-corporations.read_starbases.v1
- description: EVE SSO scope esi-corporations.read_structures.v1
  flows:
  - implicit
  scope: esi-corporations.read_structures.v1
- description: EVE SSO scope esi-corporations.read_titles.v1
  flows:
  - implicit
  scope: esi-corporations.read_titles.v1
- description: EVE SSO scope esi-corporations.track_members.v1
  flows:
  - implicit
  scope: esi-corporations.track_members.v1
- description: EVE SSO scope esi-fittings.read_fittings.v1
  flows:
  - implicit
  scope: esi-fittings.read_fittings.v1
- description: EVE SSO scope esi-fittings.write_fittings.v1
  flows:
  - implicit
  scope: esi-fittings.write_fittings.v1
- description: EVE SSO scope esi-fleets.read_fleet.v1
  flows:
  - implicit
  scope: esi-fleets.read_fleet.v1
- description: EVE SSO scope esi-fleets.write_fleet.v1
  flows:
  - implicit
  scope: esi-fleets.write_fleet.v1
- description: EVE SSO scope esi-industry.read_character_jobs.v1
  flows:
  - implicit
  scope: esi-industry.read_character_jobs.v1
- description: EVE SSO scope esi-industry.read_character_mining.v1
  flows:
  - implicit
  scope: esi-industry.read_character_mining.v1
- description: EVE SSO scope esi-industry.read_corporation_jobs.v1
  flows:
  - implicit
  scope: esi-industry.read_corporation_jobs.v1
- description: EVE SSO scope esi-industry.read_corporation_mining.v1
  flows:
  - implicit
  scope: esi-industry.read_corporation_mining.v1
- description: EVE SSO scope esi-killmails.read_corporation_killmails.v1
  flows:
  - implicit
  scope: esi-killmails.read_corporation_killmails.v1
- description: EVE SSO scope esi-killmails.read_killmails.v1
  flows:
  - implicit
  scope: esi-killmails.read_killmails.v1
- description: EVE SSO scope esi-location.read_location.v1
  flows:
  - implicit
  scope: esi-location.read_location.v1
- description: EVE SSO scope esi-location.read_online.v1
  flows:
  - implicit
  scope: esi-location.read_online.v1
- description: EVE SSO scope esi-location.read_ship_type.v1
  flows:
  - implicit
  scope: esi-location.read_ship_type.v1
- description: EVE SSO scope esi-mail.organize_mail.v1
  flows:
  - implicit
  scope: esi-mail.organize_mail.v1
- description: EVE SSO scope esi-mail.read_mail.v1
  flows:
  - implicit
  scope: esi-mail.read_mail.v1
- description: EVE SSO scope esi-mail.send_mail.v1
  flows:
  - implicit
  scope: esi-mail.send_mail.v1
- description: EVE SSO scope esi-markets.read_character_orders.v1
  flows:
  - implicit
  scope: esi-markets.read_character_orders.v1
- description: EVE SSO scope esi-markets.read_corporation_orders.v1
  flows:
  - implicit
  scope: esi-markets.read_corporation_orders.v1
- description: EVE SSO scope esi-markets.structure_markets.v1
  flows:
  - implicit
  scope: esi-markets.structure_markets.v1
- description: EVE SSO scope esi-planets.manage_planets.v1
  flows:
  - implicit
  scope: esi-planets.manage_planets.v1
- description: EVE SSO scope esi-planets.read_customs_offices.v1
  flows:
  - implicit
  scope: esi-planets.read_customs_offices.v1
- description: EVE SSO scope esi-search.search_structures.v1
  flows:
  - implicit
  scope: esi-search.search_structures.v1
- description: EVE SSO scope esi-skills.read_skillqueue.v1
  flows:
  - implicit
  scope: esi-skills.read_skillqueue.v1
- description: EVE SSO scope esi-skills.read_skills.v1
  flows:
  - implicit
  scope: esi-skills.read_skills.v1
- description: EVE SSO scope esi-ui.open_window.v1
  flows:
  - implicit
  scope: esi-ui.open_window.v1
- description: EVE SSO scope esi-ui.write_waypoint.v1
  flows:
  - implicit
  scope: esi-ui.write_waypoint.v1
- description: EVE SSO scope esi-universe.read_structures.v1
  flows:
  - implicit
  scope: esi-universe.read_structures.v1
- description: EVE SSO scope esi-wallet.read_character_wallet.v1
  flows:
  - implicit
  scope: esi-wallet.read_character_wallet.v1
- description: EVE SSO scope esi-wallet.read_corporation_wallets.v1
  flows:
  - implicit
  scope: esi-wallet.read_corporation_wallets.v1
slug: eve-online-scopes
source_filename: eve-online-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/eve-online-openapi.yml\nschemes:\n- name: evesso\n  source: openapi/eve-online-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.eveonline.com/v2/oauth/authorize\nscopes:\n- scope: esi-alliances.read_contacts.v1\n  description: EVE SSO scope esi-alliances.read_contacts.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-assets.read_assets.v1\n  description: EVE SSO scope esi-assets.read_assets.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-assets.read_corporation_assets.v1\n  description: EVE SSO scope esi-assets.read_corporation_assets.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-calendar.read_calendar_events.v1\n  description: EVE SSO scope esi-calendar.read_calendar_events.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-calendar.respond_calendar_events.v1\n\
  \  description: EVE SSO scope esi-calendar.respond_calendar_events.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-characters.read_agents_research.v1\n  description: EVE SSO scope esi-characters.read_agents_research.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-characters.read_blueprints.v1\n  description: EVE SSO scope esi-characters.read_blueprints.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-characters.read_contacts.v1\n  description: EVE SSO scope esi-characters.read_contacts.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-characters.read_corporation_roles.v1\n  description: EVE SSO scope esi-characters.read_corporation_roles.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-characters.read_fatigue.v1\n  description: EVE SSO scope esi-characters.read_fatigue.v1\n  flows:\n  - implicit\n\
  \  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-characters.read_fw_stats.v1\n  description: EVE SSO scope esi-characters.read_fw_stats.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-characters.read_loyalty.v1\n  description: EVE SSO scope esi-characters.read_loyalty.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-characters.read_medals.v1\n  description: EVE SSO scope esi-characters.read_medals.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-characters.read_notifications.v1\n  description: EVE SSO scope esi-characters.read_notifications.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-characters.read_standings.v1\n  description: EVE SSO scope esi-characters.read_standings.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-characters.read_titles.v1\n  description: EVE SSO scope\
  \ esi-characters.read_titles.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-characters.write_contacts.v1\n  description: EVE SSO scope esi-characters.write_contacts.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-clones.read_clones.v1\n  description: EVE SSO scope esi-clones.read_clones.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-clones.read_implants.v1\n  description: EVE SSO scope esi-clones.read_implants.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-contracts.read_character_contracts.v1\n  description: EVE SSO scope esi-contracts.read_character_contracts.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-contracts.read_corporation_contracts.v1\n  description: EVE SSO scope esi-contracts.read_corporation_contracts.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n\
  - scope: esi-corporations.read_blueprints.v1\n  description: EVE SSO scope esi-corporations.read_blueprints.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-corporations.read_contacts.v1\n  description: EVE SSO scope esi-corporations.read_contacts.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-corporations.read_container_logs.v1\n  description: EVE SSO scope esi-corporations.read_container_logs.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-corporations.read_corporation_membership.v1\n  description: EVE SSO scope esi-corporations.read_corporation_membership.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-corporations.read_divisions.v1\n  description: EVE SSO scope esi-corporations.read_divisions.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-corporations.read_facilities.v1\n  description:\
  \ EVE SSO scope esi-corporations.read_facilities.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-corporations.read_fw_stats.v1\n  description: EVE SSO scope esi-corporations.read_fw_stats.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-corporations.read_medals.v1\n  description: EVE SSO scope esi-corporations.read_medals.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-corporations.read_standings.v1\n  description: EVE SSO scope esi-corporations.read_standings.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-corporations.read_starbases.v1\n  description: EVE SSO scope esi-corporations.read_starbases.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-corporations.read_structures.v1\n  description: EVE SSO scope esi-corporations.read_structures.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n\
  - scope: esi-corporations.read_titles.v1\n  description: EVE SSO scope esi-corporations.read_titles.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-corporations.track_members.v1\n  description: EVE SSO scope esi-corporations.track_members.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-fittings.read_fittings.v1\n  description: EVE SSO scope esi-fittings.read_fittings.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-fittings.write_fittings.v1\n  description: EVE SSO scope esi-fittings.write_fittings.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-fleets.read_fleet.v1\n  description: EVE SSO scope esi-fleets.read_fleet.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-fleets.write_fleet.v1\n  description: EVE SSO scope esi-fleets.write_fleet.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n\
  - scope: esi-industry.read_character_jobs.v1\n  description: EVE SSO scope esi-industry.read_character_jobs.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-industry.read_character_mining.v1\n  description: EVE SSO scope esi-industry.read_character_mining.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-industry.read_corporation_jobs.v1\n  description: EVE SSO scope esi-industry.read_corporation_jobs.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-industry.read_corporation_mining.v1\n  description: EVE SSO scope esi-industry.read_corporation_mining.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-killmails.read_corporation_killmails.v1\n  description: EVE SSO scope esi-killmails.read_corporation_killmails.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-killmails.read_killmails.v1\n  description:\
  \ EVE SSO scope esi-killmails.read_killmails.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-location.read_location.v1\n  description: EVE SSO scope esi-location.read_location.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-location.read_online.v1\n  description: EVE SSO scope esi-location.read_online.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-location.read_ship_type.v1\n  description: EVE SSO scope esi-location.read_ship_type.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-mail.organize_mail.v1\n  description: EVE SSO scope esi-mail.organize_mail.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-mail.read_mail.v1\n  description: EVE SSO scope esi-mail.read_mail.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-mail.send_mail.v1\n  description:\
  \ EVE SSO scope esi-mail.send_mail.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-markets.read_character_orders.v1\n  description: EVE SSO scope esi-markets.read_character_orders.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-markets.read_corporation_orders.v1\n  description: EVE SSO scope esi-markets.read_corporation_orders.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-markets.structure_markets.v1\n  description: EVE SSO scope esi-markets.structure_markets.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-planets.manage_planets.v1\n  description: EVE SSO scope esi-planets.manage_planets.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-planets.read_customs_offices.v1\n  description: EVE SSO scope esi-planets.read_customs_offices.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n\
  - scope: esi-search.search_structures.v1\n  description: EVE SSO scope esi-search.search_structures.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-skills.read_skillqueue.v1\n  description: EVE SSO scope esi-skills.read_skillqueue.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-skills.read_skills.v1\n  description: EVE SSO scope esi-skills.read_skills.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-ui.open_window.v1\n  description: EVE SSO scope esi-ui.open_window.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-ui.write_waypoint.v1\n  description: EVE SSO scope esi-ui.write_waypoint.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-universe.read_structures.v1\n  description: EVE SSO scope esi-universe.read_structures.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n\
  - scope: esi-wallet.read_character_wallet.v1\n  description: EVE SSO scope esi-wallet.read_character_wallet.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n- scope: esi-wallet.read_corporation_wallets.v1\n  description: EVE SSO scope esi-wallet.read_corporation_wallets.v1\n  flows:\n  - implicit\n  sources:\n  - openapi/eve-online-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eve-online/refs/heads/main/scopes/eve-online-scopes.yml
summary_line: 63 scopes · implicit
tags:
- Authentication
- Authorization
- Gaming
- Images
- MMO
- OAuth2
- REST
- SSO
- Static Data
token_urls: []
---
