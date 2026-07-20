---
authorization_urls: []
description: ''
docs: https://sdk-docs.kittl.dev/getting-started/scopes
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Kittl Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Kittl publishes 12 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Kittl API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Kittl
provider_slug: kittl
schemes: []
scope_count: 12
scope_names:
- design:state:read
- design:state:write
- uploads:create
- uploads:global:read
- ai:credit:spend
- fonts:read
- fonts:write
- fonts:read:global
- fonts:write:global
- data:mockups:read
- workspace:state:read
- workspace:state:write
scopes:
- description: Read design and editor state via SDK APIs.
  flows: []
  scope: design:state:read
- description: Update design state (for example add, remove, and update objects).
  flows: []
  scope: design:state:write
- description: Upload files with kittl.upload.image.upload({ blob }); apps can then use their own uploaded files.
  flows: []
  scope: uploads:create
- description: Allows an app to read all uploads available in the current workspace (not limited to the current user's uploads).
  flows: []
  scope: uploads:global:read
- description: Spend AI credits via kittl.ai.spendCredits.
  flows: []
  scope: ai:credit:spend
- description: Read fonts created by the extension.
  flows: []
  scope: fonts:read
- description: Create or modify fonts created by the extension via kittl.data.fonts.
  flows: []
  scope: fonts:write
- description: Read all custom fonts available to the user.
  flows: []
  scope: fonts:read:global
- description: Modify all custom fonts available to the user.
  flows: []
  scope: fonts:write:global
- description: Browse and search the mockup catalog via kittl.data.mockups.
  flows: []
  scope: data:mockups:read
- description: Reserved for workspace state reads.
  flows: []
  scope: workspace:state:read
- description: Reserved for workspace state writes.
  flows: []
  scope: workspace:state:write
slug: kittl-scopes
source_filename: kittl-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://sdk-docs.kittl.dev/getting-started/scopes\ndocs: https://sdk-docs.kittl.dev/getting-started/scopes\nschema: https://api.kittl.com/extensions/manifest/schema.json\nmodel: sdk-scopes\nmodel_note: >-\n  These are NOT OAuth 2.0 authorization-server scopes. Kittl's scope system governs which\n  SDK operations a sandboxed app may call inside the editor host. Scopes are declared\n  statically by the developer in manifest.json under `config.scopes` (a required field)\n  and enforced by the host at call time. Kittl separately supports OAuth as a *client*\n  — an app may declare third-party OAuth providers under `config.oauthProviders` and run\n  the flow via kittl.auth — but Kittl does not publish an authorization server of its own.\n  See authentication/kittl-authentication.yml.\ndeclaration:\n  file: manifest.json\n  path: config.scopes\n  required: true\n  empty_allowed: true\n  empty_behavior: >-\n    An empty array ([])\
  \ is valid; with an empty scope set many SDK calls will be denied\n    by scope checks.\nerror_behavior: >-\n  Calling a method without the required scope fails with an SDK error result\n  (isOk: false) and a permission-denied style message. Kittl advises requesting the\n  smallest scope set that covers all methods the app calls.\nscopes:\n- scope: design:state:read\n  description: Read design and editor state via SDK APIs.\n  methods:\n  - kittl.design.canvas.getPreviewImage\n  - kittl.design.canvas.getScreenshot\n  - kittl.design.canvas.getExport\n  - kittl.design.object.getObject\n  - kittl.design.object.getAllByFilter\n  - kittl.state.viewport.get\n  - kittl.state.getSelectedObjectsIds\n  - kittl.state.getSelectedLayersIds\n  - kittl.state.getSelectedArtboardIds\n  - kittl.state.getCanvasMode\n  - kittl.state.getActiveTool\n  - kittl.state.getHighlightedObjectId\n- scope: design:state:write\n  description: >-\n    Update design state (for example add, remove, and update objects).\n\
  \  methods:\n  - kittl.design.board.createStandardBoard\n  - kittl.design.board.cloneArtboard\n  - kittl.design.board.updateArtboard\n  - kittl.design.text.addText\n  - kittl.design.text.updateText\n  - kittl.design.text.updateRenderPlugin\n  - kittl.design.text.updateDecorationPlugin\n  - kittl.design.shape.createPredefinedShape\n  - kittl.design.shape.createBasicShape\n  - kittl.design.shape.updateShape\n  - kittl.design.shape.convertShapeToMask\n  - kittl.design.image.addImage\n  - kittl.design.image.updateImage\n  - kittl.design.video.addVideo\n  - kittl.design.video.updateVideo\n  - kittl.design.video.updatePlaylistItem\n  - kittl.design.video.removePlaylistItem\n  - kittl.design.object.removeObject\n  - kittl.design.object.setLockedState\n  - kittl.design.object.setHiddenState\n  - kittl.design.object.rotateObject\n  - kittl.design.object.rename\n  - kittl.design.config.setConfig\n  - kittl.design.loadingCard.createLoadingCard\n  - kittl.design.loadingCard.updateLoadingCard\n  -\
  \ kittl.design.mockupboard.addMockupBoard\n  - kittl.design.mockupboard.addMockupDesignObject\n  - kittl.design.mockupboard.updateMockupBoard\n  - kittl.state.setSelectedObjectsIds\n  - kittl.state.setSelectedLayersIds\n  - kittl.state.setSelectedArtboardIds\n  - kittl.state.setCanvasMode\n  - kittl.state.setActiveTool\n  - kittl.state.setHighlightedObjectId\n  - kittl.state.setMany\n  - kittl.state.viewport.set\n- scope: uploads:create\n  description: >-\n    Upload files with kittl.upload.image.upload({ blob }); apps can then use their own\n    uploaded files.\n  methods:\n  - kittl.upload.image.upload\n- scope: uploads:global:read\n  description: >-\n    Allows an app to read all uploads available in the current workspace (not limited to\n    the current user's uploads).\n- scope: ai:credit:spend\n  description: Spend AI credits via kittl.ai.spendCredits.\n  methods:\n  - kittl.ai.spendCredits\n  - kittl.ai.startGeneration\n  - kittl.ai.registerHandler\n- scope: fonts:read\n  description:\
  \ Read fonts created by the extension.\n  methods:\n  - kittl.data.fonts.listExtensionFonts\n  - kittl.data.fonts.get\n  - kittl.data.fonts.find\n  method_note: These methods accept fonts:read or fonts:read:global.\n- scope: fonts:write\n  description: Create or modify fonts created by the extension via kittl.data.fonts.\n  methods:\n  - kittl.data.fonts.create\n  - kittl.data.fonts.update\n  - kittl.data.fonts.delete\n  - kittl.data.fonts.destroy\n  - kittl.data.fonts.addStyle\n  - kittl.data.fonts.updateStyle\n  method_note: >-\n    kittl.data.fonts.create requires fonts:write specifically; the remaining write\n    methods accept fonts:write or fonts:write:global.\n- scope: fonts:read:global\n  description: Read all custom fonts available to the user.\n  methods:\n  - kittl.data.fonts.listUserFonts\n- scope: fonts:write:global\n  description: Modify all custom fonts available to the user.\n- scope: data:mockups:read\n  description: Browse and search the mockup catalog via kittl.data.mockups.\n\
  \  methods:\n  - kittl.data.mockups.get\n  - kittl.data.mockups.getOverview\n  - kittl.data.mockups.getGroup\n  - kittl.data.mockups.search\n  - kittl.data.mockups.getSuggestions\n- scope: workspace:state:read\n  description: Reserved for workspace state reads.\n  status: reserved\n- scope: workspace:state:write\n  description: Reserved for workspace state writes.\n  status: reserved\nexempt_methods:\n  note: Always allowed regardless of declared scopes.\n  methods:\n  - method: kittl.context.get\n    purpose: Host context (drag-and-drop offset)\n  - method: kittl.dragAndDrop.startDragImageEvent\n    purpose: Client-side drag-and-drop helper\n  - method: kittl.dragAndDrop.dropImage\n    purpose: Client-side drag-and-drop helper\n  - method: kittl.stateless.send\n    purpose: Inter-extension messaging\n  - method: kittl.stateless.subscribe\n    purpose: Inter-extension messaging\n  - method: kittl.stateless.unsubscribe\n    purpose: Inter-extension messaging\n  - method: kittl.onReady\n\
  \    purpose: SDK readiness callback\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kittl/refs/heads/main/scopes/kittl-scopes.yml
summary_line: 12 scopes
tags:
- Company
- Design
- Graphic Design
- Creative Tools
- SDK
- Developer Platform
- Extensions
- Print On Demand
- E-Commerce
- AI
- Mockups
- Typography
token_urls: []
---
