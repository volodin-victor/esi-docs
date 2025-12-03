---
title: EVE Stable Infrastructure (ESI) - tranquility v2025-11-06
language_tabs:
  - shell: Shell
  - http: HTTP
  - javascript: JavaScript
language_clients:
  - shell: ""
  - http: ""
  - javascript: ""
toc_footers: []
includes: []
search: true
highlight_theme: darkula
headingLevel: 2

---

<!-- Generator: Widdershins v4.0.1 -->

<h1 id="eve-stable-infrastructure-esi-tranquility">EVE Stable Infrastructure (ESI) - tranquility v2025-11-06</h1>

> Scroll down for code samples, example requests and responses. Select a language for code samples from the tabs above or the mobile navigation menu.

Base URLs:

* <a href="https://esi.evetech.net">https://esi.evetech.net</a>

<a href="https://support.eveonline.com/hc/en-us/articles/8414770561948-EVE-Online-Terms-of-Service">Terms of service</a>
Web: <a href="https://developers.eveonline.com/docs/support/">ESI Support</a> 
License: <a href="https://developers.eveonline.com/license-agreement">EVE Developer License</a>

# Authentication

- oAuth2 authentication. 

    - Flow: authorizationCode
    - Authorization URL = [https://login.eveonline.com/v2/oauth/authorize](https://login.eveonline.com/v2/oauth/authorize)
    - Token URL = [https://login.eveonline.com/v2/oauth/token](https://login.eveonline.com/v2/oauth/token)

|Scope|Scope Description|
|---|---|
|esi-alliances.read_contacts.v1|esi-alliances.read_contacts.v1|
|esi-assets.read_assets.v1|esi-assets.read_assets.v1|
|esi-assets.read_corporation_assets.v1|esi-assets.read_corporation_assets.v1|
|esi-calendar.read_calendar_events.v1|esi-calendar.read_calendar_events.v1|
|esi-calendar.respond_calendar_events.v1|esi-calendar.respond_calendar_events.v1|
|esi-characters.read_agents_research.v1|esi-characters.read_agents_research.v1|
|esi-characters.read_blueprints.v1|esi-characters.read_blueprints.v1|
|esi-characters.read_contacts.v1|esi-characters.read_contacts.v1|
|esi-characters.read_corporation_roles.v1|esi-characters.read_corporation_roles.v1|
|esi-characters.read_fatigue.v1|esi-characters.read_fatigue.v1|
|esi-characters.read_freelance_jobs.v1|esi-characters.read_freelance_jobs.v1|
|esi-characters.read_fw_stats.v1|esi-characters.read_fw_stats.v1|
|esi-characters.read_loyalty.v1|esi-characters.read_loyalty.v1|
|esi-characters.read_medals.v1|esi-characters.read_medals.v1|
|esi-characters.read_notifications.v1|esi-characters.read_notifications.v1|
|esi-characters.read_standings.v1|esi-characters.read_standings.v1|
|esi-characters.read_titles.v1|esi-characters.read_titles.v1|
|esi-characters.write_contacts.v1|esi-characters.write_contacts.v1|
|esi-clones.read_clones.v1|esi-clones.read_clones.v1|
|esi-clones.read_implants.v1|esi-clones.read_implants.v1|
|esi-contracts.read_character_contracts.v1|esi-contracts.read_character_contracts.v1|
|esi-contracts.read_corporation_contracts.v1|esi-contracts.read_corporation_contracts.v1|
|esi-corporations.read_blueprints.v1|esi-corporations.read_blueprints.v1|
|esi-corporations.read_contacts.v1|esi-corporations.read_contacts.v1|
|esi-corporations.read_container_logs.v1|esi-corporations.read_container_logs.v1|
|esi-corporations.read_corporation_membership.v1|esi-corporations.read_corporation_membership.v1|
|esi-corporations.read_divisions.v1|esi-corporations.read_divisions.v1|
|esi-corporations.read_facilities.v1|esi-corporations.read_facilities.v1|
|esi-corporations.read_freelance_jobs.v1|esi-corporations.read_freelance_jobs.v1|
|esi-corporations.read_fw_stats.v1|esi-corporations.read_fw_stats.v1|
|esi-corporations.read_medals.v1|esi-corporations.read_medals.v1|
|esi-corporations.read_projects.v1|esi-corporations.read_projects.v1|
|esi-corporations.read_standings.v1|esi-corporations.read_standings.v1|
|esi-corporations.read_starbases.v1|esi-corporations.read_starbases.v1|
|esi-corporations.read_structures.v1|esi-corporations.read_structures.v1|
|esi-corporations.read_titles.v1|esi-corporations.read_titles.v1|
|esi-corporations.track_members.v1|esi-corporations.track_members.v1|
|esi-fittings.read_fittings.v1|esi-fittings.read_fittings.v1|
|esi-fittings.write_fittings.v1|esi-fittings.write_fittings.v1|
|esi-fleets.read_fleet.v1|esi-fleets.read_fleet.v1|
|esi-fleets.write_fleet.v1|esi-fleets.write_fleet.v1|
|esi-industry.read_character_jobs.v1|esi-industry.read_character_jobs.v1|
|esi-industry.read_character_mining.v1|esi-industry.read_character_mining.v1|
|esi-industry.read_corporation_jobs.v1|esi-industry.read_corporation_jobs.v1|
|esi-industry.read_corporation_mining.v1|esi-industry.read_corporation_mining.v1|
|esi-killmails.read_corporation_killmails.v1|esi-killmails.read_corporation_killmails.v1|
|esi-killmails.read_killmails.v1|esi-killmails.read_killmails.v1|
|esi-location.read_location.v1|esi-location.read_location.v1|
|esi-location.read_online.v1|esi-location.read_online.v1|
|esi-location.read_ship_type.v1|esi-location.read_ship_type.v1|
|esi-mail.organize_mail.v1|esi-mail.organize_mail.v1|
|esi-mail.read_mail.v1|esi-mail.read_mail.v1|
|esi-mail.send_mail.v1|esi-mail.send_mail.v1|
|esi-markets.read_character_orders.v1|esi-markets.read_character_orders.v1|
|esi-markets.read_corporation_orders.v1|esi-markets.read_corporation_orders.v1|
|esi-markets.structure_markets.v1|esi-markets.structure_markets.v1|
|esi-planets.manage_planets.v1|esi-planets.manage_planets.v1|
|esi-planets.read_customs_offices.v1|esi-planets.read_customs_offices.v1|
|esi-search.search_structures.v1|esi-search.search_structures.v1|
|esi-skills.read_skillqueue.v1|esi-skills.read_skillqueue.v1|
|esi-skills.read_skills.v1|esi-skills.read_skills.v1|
|esi-ui.open_window.v1|esi-ui.open_window.v1|
|esi-ui.write_waypoint.v1|esi-ui.write_waypoint.v1|
|esi-universe.read_structures.v1|esi-universe.read_structures.v1|
|esi-wallet.read_character_wallet.v1|esi-wallet.read_character_wallet.v1|
|esi-wallet.read_corporation_wallets.v1|esi-wallet.read_corporation_wallets.v1|

<h1 id="eve-stable-infrastructure-esi-tranquility-alliance">Alliance</h1>

## GetAlliances

<a id="opIdGetAlliances"></a>

`GET /alliances`

*List all alliances*

List all active player alliances

<h3 id="getalliances-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  0
]
```

<h3 id="getalliances-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[AlliancesGet](#schemaalliancesget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetAlliancesAllianceId

<a id="opIdGetAlliancesAllianceId"></a>

`GET /alliances/{alliance_id}`

*Get alliance information*

Public information about an alliance

<h3 id="getalliancesallianceid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|alliance_id|path|[AllianceID](#schemaallianceid)|true|The ID of the alliance|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "creator_corporation_id": 0,
  "creator_id": 0,
  "date_founded": "2019-08-24T14:15:22Z",
  "executor_corporation_id": 0,
  "faction_id": 0,
  "name": "string",
  "ticker": "string"
}
```

<h3 id="getalliancesallianceid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[AlliancesAllianceIdGet](#schemaalliancesallianceidget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetAlliancesAllianceIdCorporations

<a id="opIdGetAlliancesAllianceIdCorporations"></a>

`GET /alliances/{alliance_id}/corporations`

*List alliance's corporations*

List all current member corporations of an alliance

<h3 id="getalliancesallianceidcorporations-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|alliance_id|path|[AllianceID](#schemaallianceid)|true|The ID of the alliance|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  0
]
```

<h3 id="getalliancesallianceidcorporations-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[AlliancesAllianceIdCorporationsGet](#schemaalliancesallianceidcorporationsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetAlliancesAllianceIdIcons

<a id="opIdGetAlliancesAllianceIdIcons"></a>

`GET /alliances/{alliance_id}/icons`

*Get alliance icon*

Get the icon urls for a alliance

This route expires daily at 11:05

<h3 id="getalliancesallianceidicons-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|alliance_id|path|[AllianceID](#schemaallianceid)|true|The ID of the alliance|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "px128x128": "string",
  "px64x64": "string"
}
```

<h3 id="getalliancesallianceidicons-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[AlliancesAllianceIdIconsGet](#schemaalliancesallianceidiconsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

<h1 id="eve-stable-infrastructure-esi-tranquility-assets">Assets</h1>

## GetCharactersCharacterIdAssets

<a id="opIdGetCharactersCharacterIdAssets"></a>

`GET /characters/{character_id}/assets`

*Get character assets*

Return a list of the characters assets

<h3 id="getcharacterscharacteridassets-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|page|query|integer(int32)|false|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "is_blueprint_copy": true,
    "is_singleton": true,
    "item_id": 0,
    "location_flag": "AssetSafety",
    "location_id": 0,
    "location_type": "station",
    "quantity": 0,
    "type_id": 0
  }
]
```

<h3 id="getcharacterscharacteridassets-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CharactersCharacterIdAssetsGet](#schemacharacterscharacteridassetsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|
|200|X-Pages|integer|int64|The total number of pages in the result set.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-assets.read_assets.v1 )
</aside>

## PostCharactersCharacterIdAssetsLocations

<a id="opIdPostCharactersCharacterIdAssetsLocations"></a>

`POST /characters/{character_id}/assets/locations`

*Get character asset locations*

Return locations for a set of item ids, which you can get from character assets endpoint. Coordinates for items in hangars or stations are set to (0,0,0)

> Body parameter

```json
[
  0
]
```

<h3 id="postcharacterscharacteridassetslocations-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|
|body|body|array[integer]|true|none|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "item_id": 0,
    "position": {
      "x": 0.1,
      "y": 0.1,
      "z": 0.1
    }
  }
]
```

<h3 id="postcharacterscharacteridassetslocations-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CharactersCharacterIdAssetsLocationsPost](#schemacharacterscharacteridassetslocationspost)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-assets.read_assets.v1 )
</aside>

## PostCharactersCharacterIdAssetsNames

<a id="opIdPostCharactersCharacterIdAssetsNames"></a>

`POST /characters/{character_id}/assets/names`

*Get character asset names*

Return names for a set of item ids, which you can get from character assets endpoint. Typically used for items that can customize names, like containers or ships.

> Body parameter

```json
[
  0
]
```

<h3 id="postcharacterscharacteridassetsnames-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|
|body|body|array[integer]|true|none|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "item_id": 0,
    "name": "string"
  }
]
```

<h3 id="postcharacterscharacteridassetsnames-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CharactersCharacterIdAssetsNamesPost](#schemacharacterscharacteridassetsnamespost)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-assets.read_assets.v1 )
</aside>

## GetCorporationsCorporationIdAssets

<a id="opIdGetCorporationsCorporationIdAssets"></a>

`GET /corporations/{corporation_id}/assets`

*Get corporation assets*

Return a list of the corporation assets

<h3 id="getcorporationscorporationidassets-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|corporation_id|path|[CorporationID](#schemacorporationid)|true|The ID of the corporation|
|page|query|integer(int32)|false|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "is_blueprint_copy": true,
    "is_singleton": true,
    "item_id": 0,
    "location_flag": "AssetSafety",
    "location_id": 0,
    "location_type": "station",
    "quantity": 0,
    "type_id": 0
  }
]
```

<h3 id="getcorporationscorporationidassets-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CorporationsCorporationIdAssetsGet](#schemacorporationscorporationidassetsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|
|200|X-Pages|integer|int64|The total number of pages in the result set.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-assets.read_corporation_assets.v1 )
</aside>

## PostCorporationsCorporationIdAssetsLocations

<a id="opIdPostCorporationsCorporationIdAssetsLocations"></a>

`POST /corporations/{corporation_id}/assets/locations`

*Get corporation asset locations*

Return locations for a set of item ids, which you can get from corporation assets endpoint. Coordinates for items in hangars or stations are set to (0,0,0)

> Body parameter

```json
[
  0
]
```

<h3 id="postcorporationscorporationidassetslocations-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|corporation_id|path|[CorporationID](#schemacorporationid)|true|The ID of the corporation|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|
|body|body|array[integer]|true|none|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "item_id": 0,
    "position": {
      "x": 0.1,
      "y": 0.1,
      "z": 0.1
    }
  }
]
```

<h3 id="postcorporationscorporationidassetslocations-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CorporationsCorporationIdAssetsLocationsPost](#schemacorporationscorporationidassetslocationspost)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-assets.read_corporation_assets.v1 )
</aside>

## PostCorporationsCorporationIdAssetsNames

<a id="opIdPostCorporationsCorporationIdAssetsNames"></a>

`POST /corporations/{corporation_id}/assets/names`

*Get corporation asset names*

Return names for a set of item ids, which you can get from corporation assets endpoint. Only valid for items that can customize names, like containers or ships

> Body parameter

```json
[
  0
]
```

<h3 id="postcorporationscorporationidassetsnames-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|corporation_id|path|[CorporationID](#schemacorporationid)|true|The ID of the corporation|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|
|body|body|array[integer]|true|none|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "item_id": 0,
    "name": "string"
  }
]
```

<h3 id="postcorporationscorporationidassetsnames-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CorporationsCorporationIdAssetsNamesPost](#schemacorporationscorporationidassetsnamespost)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-assets.read_corporation_assets.v1 )
</aside>

<h1 id="eve-stable-infrastructure-esi-tranquility-calendar">Calendar</h1>

## GetCharactersCharacterIdCalendar

<a id="opIdGetCharactersCharacterIdCalendar"></a>

`GET /characters/{character_id}/calendar`

*List calendar event summaries*

Get 50 event summaries from the calendar. If no from_event ID is given, the resource will return the next 50 chronological event summaries from now. If a from_event ID is specified, it will return the next 50 chronological event summaries from after that event

<h3 id="getcharacterscharacteridcalendar-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|from_event|query|integer(int64)|false|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "event_date": "2019-08-24T14:15:22Z",
    "event_id": 0,
    "event_response": "declined",
    "importance": 0,
    "title": "string"
  }
]
```

<h3 id="getcharacterscharacteridcalendar-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CharactersCharacterIdCalendarGet](#schemacharacterscharacteridcalendarget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-calendar.read_calendar_events.v1 )
</aside>

## GetCharactersCharacterIdCalendarEventId

<a id="opIdGetCharactersCharacterIdCalendarEventId"></a>

`GET /characters/{character_id}/calendar/{event_id}`

*Get an event*

Get all the information for a specific event

<h3 id="getcharacterscharacteridcalendareventid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|event_id|path|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "date": "2019-08-24T14:15:22Z",
  "duration": 0,
  "event_id": 0,
  "importance": 0,
  "owner_id": 0,
  "owner_name": "string",
  "owner_type": "eve_server",
  "response": "string",
  "text": "string",
  "title": "string"
}
```

<h3 id="getcharacterscharacteridcalendareventid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CharactersCharacterIdCalendarEventIdGet](#schemacharacterscharacteridcalendareventidget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-calendar.read_calendar_events.v1 )
</aside>

## PutCharactersCharacterIdCalendarEventId

<a id="opIdPutCharactersCharacterIdCalendarEventId"></a>

`PUT /characters/{character_id}/calendar/{event_id}`

*Respond to an event*

Set your response status to an event

> Body parameter

```json
{
  "response": "accepted"
}
```

<h3 id="putcharacterscharacteridcalendareventid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|event_id|path|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|
|body|body|object|true|none|
|» response|body|string|true|none|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|
|» response|accepted|
|» response|declined|
|» response|tentative|

> Example responses

> default Response

```json
{
  "details": [
    {
      "location": "string",
      "message": "string",
      "value": null
    }
  ],
  "error": "string"
}
```

<h3 id="putcharacterscharacteridcalendareventid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|204|[No Content](https://tools.ietf.org/html/rfc7231#section-6.3.5)|Event updated|None|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|204|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|204|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|204|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-calendar.respond_calendar_events.v1 )
</aside>

## GetCharactersCharacterIdCalendarEventIdAttendees

<a id="opIdGetCharactersCharacterIdCalendarEventIdAttendees"></a>

`GET /characters/{character_id}/calendar/{event_id}/attendees`

*Get attendees*

Get all invited attendees for a given event

<h3 id="getcharacterscharacteridcalendareventidattendees-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|event_id|path|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "character_id": 0,
    "event_response": "declined"
  }
]
```

<h3 id="getcharacterscharacteridcalendareventidattendees-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CharactersCharacterIdCalendarEventIdAttendeesGet](#schemacharacterscharacteridcalendareventidattendeesget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-calendar.read_calendar_events.v1 )
</aside>

<h1 id="eve-stable-infrastructure-esi-tranquility-character">Character</h1>

## PostCharactersAffiliation

<a id="opIdPostCharactersAffiliation"></a>

`POST /characters/affiliation`

*Character affiliation*

Bulk lookup of character IDs to corporation, alliance and faction

> Body parameter

```json
[
  0
]
```

<h3 id="postcharactersaffiliation-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|
|body|body|array[integer]|true|none|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "alliance_id": 0,
    "character_id": 0,
    "corporation_id": 0,
    "faction_id": 0
  }
]
```

<h3 id="postcharactersaffiliation-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CharactersAffiliationPost](#schemacharactersaffiliationpost)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetCharactersCharacterId

<a id="opIdGetCharactersCharacterId"></a>

`GET /characters/{character_id}`

*Get character's public information*

Public information about a character

<h3 id="getcharacterscharacterid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "alliance_id": 0,
  "birthday": "2019-08-24T14:15:22Z",
  "bloodline_id": 0,
  "corporation_id": 0,
  "description": "string",
  "faction_id": 0,
  "gender": "female",
  "name": "string",
  "race_id": 0,
  "security_status": 0.1,
  "title": "string"
}
```

<h3 id="getcharacterscharacterid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CharactersCharacterIdGet](#schemacharacterscharacteridget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetCharactersCharacterIdAgentsResearch

<a id="opIdGetCharactersCharacterIdAgentsResearch"></a>

`GET /characters/{character_id}/agents_research`

*Get agents research*

Return a list of agents research information for a character. The formula for finding the current research points with an agent is: currentPoints = remainderPoints + pointsPerDay * days(currentTime - researchStartDate)

<h3 id="getcharacterscharacteridagentsresearch-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "agent_id": 0,
    "points_per_day": 0.1,
    "remainder_points": 0.1,
    "skill_type_id": 0,
    "started_at": "2019-08-24T14:15:22Z"
  }
]
```

<h3 id="getcharacterscharacteridagentsresearch-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CharactersCharacterIdAgentsResearchGet](#schemacharacterscharacteridagentsresearchget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-characters.read_agents_research.v1 )
</aside>

## GetCharactersCharacterIdBlueprints

<a id="opIdGetCharactersCharacterIdBlueprints"></a>

`GET /characters/{character_id}/blueprints`

*Get blueprints*

Return a list of blueprints the character owns

<h3 id="getcharacterscharacteridblueprints-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|page|query|integer(int32)|false|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "item_id": 0,
    "location_flag": "AutoFit",
    "location_id": 0,
    "material_efficiency": 0,
    "quantity": 0,
    "runs": 0,
    "time_efficiency": 0,
    "type_id": 0
  }
]
```

<h3 id="getcharacterscharacteridblueprints-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CharactersCharacterIdBlueprintsGet](#schemacharacterscharacteridblueprintsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|
|200|X-Pages|integer|int64|The total number of pages in the result set.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-characters.read_blueprints.v1 )
</aside>

## GetCharactersCharacterIdCorporationhistory

<a id="opIdGetCharactersCharacterIdCorporationhistory"></a>

`GET /characters/{character_id}/corporationhistory`

*Get corporation history*

Get a list of all the corporations a character has been a member of

<h3 id="getcharacterscharacteridcorporationhistory-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "corporation_id": 0,
    "is_deleted": true,
    "record_id": 0,
    "start_date": "2019-08-24T14:15:22Z"
  }
]
```

<h3 id="getcharacterscharacteridcorporationhistory-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CharactersCharacterIdCorporationhistoryGet](#schemacharacterscharacteridcorporationhistoryget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## PostCharactersCharacterIdCspa

<a id="opIdPostCharactersCharacterIdCspa"></a>

`POST /characters/{character_id}/cspa`

*Calculate a CSPA charge cost*

Takes a source character ID in the url and a set of target character ID's in the body, returns a CSPA charge cost

> Body parameter

```json
[
  0
]
```

<h3 id="postcharacterscharacteridcspa-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|
|body|body|array[integer]|true|none|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 201 Response

```json
0.1
```

<h3 id="postcharacterscharacteridcspa-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|[CharactersCharacterIdCspaPost](#schemacharacterscharacteridcspapost)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|201|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|201|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|201|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-characters.read_contacts.v1 )
</aside>

## GetCharactersCharacterIdFatigue

<a id="opIdGetCharactersCharacterIdFatigue"></a>

`GET /characters/{character_id}/fatigue`

*Get jump fatigue*

Return a character's jump activation and fatigue information

<h3 id="getcharacterscharacteridfatigue-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "jump_fatigue_expire_date": "2019-08-24T14:15:22Z",
  "last_jump_date": "2019-08-24T14:15:22Z",
  "last_update_date": "2019-08-24T14:15:22Z"
}
```

<h3 id="getcharacterscharacteridfatigue-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CharactersCharacterIdFatigueGet](#schemacharacterscharacteridfatigueget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-characters.read_fatigue.v1 )
</aside>

## GetCharactersCharacterIdMedals

<a id="opIdGetCharactersCharacterIdMedals"></a>

`GET /characters/{character_id}/medals`

*Get medals*

Return a list of medals the character has

<h3 id="getcharacterscharacteridmedals-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "corporation_id": 0,
    "date": "2019-08-24T14:15:22Z",
    "description": "string",
    "graphics": [
      {
        "color": 0,
        "graphic": "string",
        "layer": 0,
        "part": 0
      }
    ],
    "issuer_id": 0,
    "medal_id": 0,
    "reason": "string",
    "status": "public",
    "title": "string"
  }
]
```

<h3 id="getcharacterscharacteridmedals-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CharactersCharacterIdMedalsGet](#schemacharacterscharacteridmedalsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-characters.read_medals.v1 )
</aside>

## GetCharactersCharacterIdNotifications

<a id="opIdGetCharactersCharacterIdNotifications"></a>

`GET /characters/{character_id}/notifications`

*Get character notifications*

Return character notifications

<h3 id="getcharacterscharacteridnotifications-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "is_read": true,
    "notification_id": 0,
    "sender_id": 0,
    "sender_type": "character",
    "text": "string",
    "timestamp": "2019-08-24T14:15:22Z",
    "type": "AcceptedAlly"
  }
]
```

<h3 id="getcharacterscharacteridnotifications-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CharactersCharacterIdNotificationsGet](#schemacharacterscharacteridnotificationsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-characters.read_notifications.v1 )
</aside>

## GetCharactersCharacterIdNotificationsContacts

<a id="opIdGetCharactersCharacterIdNotificationsContacts"></a>

`GET /characters/{character_id}/notifications/contacts`

*Get new contact notifications*

Return notifications about having been added to someone's contact list

<h3 id="getcharacterscharacteridnotificationscontacts-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "message": "string",
    "notification_id": 0,
    "send_date": "2019-08-24T14:15:22Z",
    "sender_character_id": 0,
    "standing_level": 0.1
  }
]
```

<h3 id="getcharacterscharacteridnotificationscontacts-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CharactersCharacterIdNotificationsContactsGet](#schemacharacterscharacteridnotificationscontactsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-characters.read_notifications.v1 )
</aside>

## GetCharactersCharacterIdPortrait

<a id="opIdGetCharactersCharacterIdPortrait"></a>

`GET /characters/{character_id}/portrait`

*Get character portraits*

Get portrait urls for a character

This route expires daily at 11:05

<h3 id="getcharacterscharacteridportrait-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "px128x128": "string",
  "px256x256": "string",
  "px512x512": "string",
  "px64x64": "string"
}
```

<h3 id="getcharacterscharacteridportrait-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CharactersCharacterIdPortraitGet](#schemacharacterscharacteridportraitget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetCharactersCharacterIdRoles

<a id="opIdGetCharactersCharacterIdRoles"></a>

`GET /characters/{character_id}/roles`

*Get character corporation roles*

Returns a character's corporation roles

<h3 id="getcharacterscharacteridroles-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "roles": [
    "Account_Take_1"
  ],
  "roles_at_base": [
    "Account_Take_1"
  ],
  "roles_at_hq": [
    "Account_Take_1"
  ],
  "roles_at_other": [
    "Account_Take_1"
  ]
}
```

<h3 id="getcharacterscharacteridroles-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CharactersCharacterIdRolesGet](#schemacharacterscharacteridrolesget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-characters.read_corporation_roles.v1 )
</aside>

## GetCharactersCharacterIdStandings

<a id="opIdGetCharactersCharacterIdStandings"></a>

`GET /characters/{character_id}/standings`

*Get standings*

Return character standings from agents, NPC corporations, and factions

<h3 id="getcharacterscharacteridstandings-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "from_id": 0,
    "from_type": "agent",
    "standing": 0.1
  }
]
```

<h3 id="getcharacterscharacteridstandings-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CharactersCharacterIdStandingsGet](#schemacharacterscharacteridstandingsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-characters.read_standings.v1 )
</aside>

## GetCharactersCharacterIdTitles

<a id="opIdGetCharactersCharacterIdTitles"></a>

`GET /characters/{character_id}/titles`

*Get character corporation titles*

Returns a character's titles

<h3 id="getcharacterscharacteridtitles-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "name": "string",
    "title_id": 0
  }
]
```

<h3 id="getcharacterscharacteridtitles-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CharactersCharacterIdTitlesGet](#schemacharacterscharacteridtitlesget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-characters.read_titles.v1 )
</aside>

<h1 id="eve-stable-infrastructure-esi-tranquility-clones">Clones</h1>

## GetCharactersCharacterIdClones

<a id="opIdGetCharactersCharacterIdClones"></a>

`GET /characters/{character_id}/clones`

*Get clones*

A list of the character's clones

<h3 id="getcharacterscharacteridclones-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "home_location": {
    "location_id": 0,
    "location_type": "station"
  },
  "jump_clones": [
    {
      "implants": [
        0
      ],
      "jump_clone_id": 0,
      "location_id": 0,
      "location_type": "station",
      "name": "string"
    }
  ],
  "last_clone_jump_date": "2019-08-24T14:15:22Z",
  "last_station_change_date": "2019-08-24T14:15:22Z"
}
```

<h3 id="getcharacterscharacteridclones-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CharactersCharacterIdClonesGet](#schemacharacterscharacteridclonesget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-clones.read_clones.v1 )
</aside>

## GetCharactersCharacterIdImplants

<a id="opIdGetCharactersCharacterIdImplants"></a>

`GET /characters/{character_id}/implants`

*Get active implants*

Return implants on the active clone of a character

<h3 id="getcharacterscharacteridimplants-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  0
]
```

<h3 id="getcharacterscharacteridimplants-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CharactersCharacterIdImplantsGet](#schemacharacterscharacteridimplantsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-clones.read_implants.v1 )
</aside>

<h1 id="eve-stable-infrastructure-esi-tranquility-contacts">Contacts</h1>

## GetAlliancesAllianceIdContacts

<a id="opIdGetAlliancesAllianceIdContacts"></a>

`GET /alliances/{alliance_id}/contacts`

*Get alliance contacts*

Return contacts of an alliance

<h3 id="getalliancesallianceidcontacts-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|alliance_id|path|[AllianceID](#schemaallianceid)|true|The ID of the alliance|
|page|query|integer(int32)|false|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "contact_id": 0,
    "contact_type": "character",
    "label_ids": [
      0
    ],
    "standing": 0.1
  }
]
```

<h3 id="getalliancesallianceidcontacts-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[AlliancesAllianceIdContactsGet](#schemaalliancesallianceidcontactsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|
|200|X-Pages|integer|int64|The total number of pages in the result set.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-alliances.read_contacts.v1 )
</aside>

## GetAlliancesAllianceIdContactsLabels

<a id="opIdGetAlliancesAllianceIdContactsLabels"></a>

`GET /alliances/{alliance_id}/contacts/labels`

*Get alliance contact labels*

Return custom labels for an alliance's contacts

<h3 id="getalliancesallianceidcontactslabels-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|alliance_id|path|[AllianceID](#schemaallianceid)|true|The ID of the alliance|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "label_id": 0,
    "label_name": "string"
  }
]
```

<h3 id="getalliancesallianceidcontactslabels-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[AlliancesAllianceIdContactsLabelsGet](#schemaalliancesallianceidcontactslabelsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-alliances.read_contacts.v1 )
</aside>

## DeleteCharactersCharacterIdContacts

<a id="opIdDeleteCharactersCharacterIdContacts"></a>

`DELETE /characters/{character_id}/contacts`

*Delete contacts*

Bulk delete contacts

<h3 id="deletecharacterscharacteridcontacts-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|contact_ids|query|array[integer]|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> default Response

```json
{
  "details": [
    {
      "location": "string",
      "message": "string",
      "value": null
    }
  ],
  "error": "string"
}
```

<h3 id="deletecharacterscharacteridcontacts-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|204|[No Content](https://tools.ietf.org/html/rfc7231#section-6.3.5)|Contacts deleted|None|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|204|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|204|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|204|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-characters.write_contacts.v1 )
</aside>

## GetCharactersCharacterIdContacts

<a id="opIdGetCharactersCharacterIdContacts"></a>

`GET /characters/{character_id}/contacts`

*Get contacts*

Return contacts of a character

<h3 id="getcharacterscharacteridcontacts-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|page|query|integer(int32)|false|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "contact_id": 0,
    "contact_type": "character",
    "is_blocked": true,
    "is_watched": true,
    "label_ids": [
      0
    ],
    "standing": 0.1
  }
]
```

<h3 id="getcharacterscharacteridcontacts-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CharactersCharacterIdContactsGet](#schemacharacterscharacteridcontactsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|
|200|X-Pages|integer|int64|The total number of pages in the result set.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-characters.read_contacts.v1 )
</aside>

## PostCharactersCharacterIdContacts

<a id="opIdPostCharactersCharacterIdContacts"></a>

`POST /characters/{character_id}/contacts`

*Add contacts*

Bulk add contacts with same settings

> Body parameter

```json
[
  0
]
```

<h3 id="postcharacterscharacteridcontacts-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|label_ids|query|array[integer]|false|none|
|standing|query|number(double)|true|none|
|watched|query|boolean|false|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|
|body|body|array[integer]|true|none|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 201 Response

```json
[
  0
]
```

<h3 id="postcharacterscharacteridcontacts-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|[CharactersCharacterIdContactsPost](#schemacharacterscharacteridcontactspost)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|201|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|201|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|201|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-characters.write_contacts.v1 )
</aside>

## PutCharactersCharacterIdContacts

<a id="opIdPutCharactersCharacterIdContacts"></a>

`PUT /characters/{character_id}/contacts`

*Edit contacts*

Bulk edit contacts with same settings

> Body parameter

```json
[
  0
]
```

<h3 id="putcharacterscharacteridcontacts-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|label_ids|query|array[integer]|false|none|
|standing|query|number(double)|true|none|
|watched|query|boolean|false|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|
|body|body|array[integer]|true|none|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> default Response

```json
{
  "details": [
    {
      "location": "string",
      "message": "string",
      "value": null
    }
  ],
  "error": "string"
}
```

<h3 id="putcharacterscharacteridcontacts-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|204|[No Content](https://tools.ietf.org/html/rfc7231#section-6.3.5)|Contacts updated|None|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|204|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|204|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|204|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-characters.write_contacts.v1 )
</aside>

## GetCharactersCharacterIdContactsLabels

<a id="opIdGetCharactersCharacterIdContactsLabels"></a>

`GET /characters/{character_id}/contacts/labels`

*Get contact labels*

Return custom labels for a character's contacts

<h3 id="getcharacterscharacteridcontactslabels-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "label_id": 0,
    "label_name": "string"
  }
]
```

<h3 id="getcharacterscharacteridcontactslabels-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CharactersCharacterIdContactsLabelsGet](#schemacharacterscharacteridcontactslabelsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-characters.read_contacts.v1 )
</aside>

## GetCorporationsCorporationIdContacts

<a id="opIdGetCorporationsCorporationIdContacts"></a>

`GET /corporations/{corporation_id}/contacts`

*Get corporation contacts*

Return contacts of a corporation

<h3 id="getcorporationscorporationidcontacts-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|corporation_id|path|[CorporationID](#schemacorporationid)|true|The ID of the corporation|
|page|query|integer(int32)|false|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "contact_id": 0,
    "contact_type": "character",
    "is_watched": true,
    "label_ids": [
      0
    ],
    "standing": 0.1
  }
]
```

<h3 id="getcorporationscorporationidcontacts-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CorporationsCorporationIdContactsGet](#schemacorporationscorporationidcontactsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|
|200|X-Pages|integer|int64|The total number of pages in the result set.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-corporations.read_contacts.v1 )
</aside>

## GetCorporationsCorporationIdContactsLabels

<a id="opIdGetCorporationsCorporationIdContactsLabels"></a>

`GET /corporations/{corporation_id}/contacts/labels`

*Get corporation contact labels*

Return custom labels for a corporation's contacts

<h3 id="getcorporationscorporationidcontactslabels-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|corporation_id|path|[CorporationID](#schemacorporationid)|true|The ID of the corporation|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "label_id": 0,
    "label_name": "string"
  }
]
```

<h3 id="getcorporationscorporationidcontactslabels-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CorporationsCorporationIdContactsLabelsGet](#schemacorporationscorporationidcontactslabelsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-corporations.read_contacts.v1 )
</aside>

<h1 id="eve-stable-infrastructure-esi-tranquility-contracts">Contracts</h1>

## GetCharactersCharacterIdContracts

<a id="opIdGetCharactersCharacterIdContracts"></a>

`GET /characters/{character_id}/contracts`

*Get contracts*

Returns contracts available to a character, only if the character is issuer, acceptor or assignee. Only returns contracts no older than 30 days, or if the status is "in_progress".

<h3 id="getcharacterscharacteridcontracts-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|page|query|integer(int32)|false|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "acceptor_id": 0,
    "assignee_id": 0,
    "availability": "public",
    "buyout": 0.1,
    "collateral": 0.1,
    "contract_id": 0,
    "date_accepted": "2019-08-24T14:15:22Z",
    "date_completed": "2019-08-24T14:15:22Z",
    "date_expired": "2019-08-24T14:15:22Z",
    "date_issued": "2019-08-24T14:15:22Z",
    "days_to_complete": 0,
    "end_location_id": 0,
    "for_corporation": true,
    "issuer_corporation_id": 0,
    "issuer_id": 0,
    "price": 0.1,
    "reward": 0.1,
    "start_location_id": 0,
    "status": "outstanding",
    "title": "string",
    "type": "unknown",
    "volume": 0.1
  }
]
```

<h3 id="getcharacterscharacteridcontracts-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CharactersCharacterIdContractsGet](#schemacharacterscharacteridcontractsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|
|200|X-Pages|integer|int64|The total number of pages in the result set.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-contracts.read_character_contracts.v1 )
</aside>

## GetCharactersCharacterIdContractsContractIdBids

<a id="opIdGetCharactersCharacterIdContractsContractIdBids"></a>

`GET /characters/{character_id}/contracts/{contract_id}/bids`

*Get contract bids*

Lists bids on a particular auction contract

<h3 id="getcharacterscharacteridcontractscontractidbids-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|contract_id|path|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "amount": 0.1,
    "bid_id": 0,
    "bidder_id": 0,
    "date_bid": "2019-08-24T14:15:22Z"
  }
]
```

<h3 id="getcharacterscharacteridcontractscontractidbids-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CharactersCharacterIdContractsContractIdBidsGet](#schemacharacterscharacteridcontractscontractidbidsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-contracts.read_character_contracts.v1 )
</aside>

## GetCharactersCharacterIdContractsContractIdItems

<a id="opIdGetCharactersCharacterIdContractsContractIdItems"></a>

`GET /characters/{character_id}/contracts/{contract_id}/items`

*Get contract items*

Lists items of a particular contract

<h3 id="getcharacterscharacteridcontractscontractiditems-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|contract_id|path|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "is_included": true,
    "is_singleton": true,
    "quantity": 0,
    "raw_quantity": 0,
    "record_id": 0,
    "type_id": 0
  }
]
```

<h3 id="getcharacterscharacteridcontractscontractiditems-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CharactersCharacterIdContractsContractIdItemsGet](#schemacharacterscharacteridcontractscontractiditemsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-contracts.read_character_contracts.v1 )
</aside>

## GetContractsPublicBidsContractId

<a id="opIdGetContractsPublicBidsContractId"></a>

`GET /contracts/public/bids/{contract_id}`

*Get public contract bids*

Lists bids on a public auction contract

<h3 id="getcontractspublicbidscontractid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|contract_id|path|integer(int64)|true|none|
|page|query|integer(int32)|false|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "amount": 0.1,
    "bid_id": 0,
    "date_bid": "2019-08-24T14:15:22Z"
  }
]
```

<h3 id="getcontractspublicbidscontractid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[ContractsPublicBidsContractIdGet](#schemacontractspublicbidscontractidget)|
|204|[No Content](https://tools.ietf.org/html/rfc7231#section-6.3.5)|Contract expired or recently accepted by player|Inline|

<h3 id="getcontractspublicbidscontractid-responseschema">Response Schema</h3>

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|
|200|X-Pages|integer|int64|The total number of pages in the result set.|
|204|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|204|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|204|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetContractsPublicItemsContractId

<a id="opIdGetContractsPublicItemsContractId"></a>

`GET /contracts/public/items/{contract_id}`

*Get public contract items*

Lists items of a public contract

<h3 id="getcontractspublicitemscontractid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|contract_id|path|integer(int64)|true|none|
|page|query|integer(int32)|false|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "is_blueprint_copy": true,
    "is_included": true,
    "item_id": 0,
    "material_efficiency": 0,
    "quantity": 0,
    "record_id": 0,
    "runs": 0,
    "time_efficiency": 0,
    "type_id": 0
  }
]
```

<h3 id="getcontractspublicitemscontractid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[ContractsPublicItemsContractIdGet](#schemacontractspublicitemscontractidget)|
|204|[No Content](https://tools.ietf.org/html/rfc7231#section-6.3.5)|Contract expired or recently accepted by player|Inline|

<h3 id="getcontractspublicitemscontractid-responseschema">Response Schema</h3>

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|
|200|X-Pages|integer|int64|The total number of pages in the result set.|
|204|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|204|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|204|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetContractsPublicRegionId

<a id="opIdGetContractsPublicRegionId"></a>

`GET /contracts/public/{region_id}`

*Get public contracts*

Returns a paginated list of all public contracts in the given region

<h3 id="getcontractspublicregionid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|page|query|integer(int32)|false|none|
|region_id|path|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "buyout": 0.1,
    "collateral": 0.1,
    "contract_id": 0,
    "date_expired": "2019-08-24T14:15:22Z",
    "date_issued": "2019-08-24T14:15:22Z",
    "days_to_complete": 0,
    "end_location_id": 0,
    "for_corporation": true,
    "issuer_corporation_id": 0,
    "issuer_id": 0,
    "price": 0.1,
    "reward": 0.1,
    "start_location_id": 0,
    "title": "string",
    "type": "unknown",
    "volume": 0.1
  }
]
```

<h3 id="getcontractspublicregionid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[ContractsPublicRegionIdGet](#schemacontractspublicregionidget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|
|200|X-Pages|integer|int64|The total number of pages in the result set.|

<aside class="success">
This operation does not require authentication
</aside>

## GetCorporationsCorporationIdContracts

<a id="opIdGetCorporationsCorporationIdContracts"></a>

`GET /corporations/{corporation_id}/contracts`

*Get corporation contracts*

Returns contracts available to a corporation, only if the corporation is issuer, acceptor or assignee. Only returns contracts no older than 30 days, or if the status is "in_progress".

<h3 id="getcorporationscorporationidcontracts-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|corporation_id|path|[CorporationID](#schemacorporationid)|true|The ID of the corporation|
|page|query|integer(int32)|false|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "acceptor_id": 0,
    "assignee_id": 0,
    "availability": "public",
    "buyout": 0.1,
    "collateral": 0.1,
    "contract_id": 0,
    "date_accepted": "2019-08-24T14:15:22Z",
    "date_completed": "2019-08-24T14:15:22Z",
    "date_expired": "2019-08-24T14:15:22Z",
    "date_issued": "2019-08-24T14:15:22Z",
    "days_to_complete": 0,
    "end_location_id": 0,
    "for_corporation": true,
    "issuer_corporation_id": 0,
    "issuer_id": 0,
    "price": 0.1,
    "reward": 0.1,
    "start_location_id": 0,
    "status": "outstanding",
    "title": "string",
    "type": "unknown",
    "volume": 0.1
  }
]
```

<h3 id="getcorporationscorporationidcontracts-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CorporationsCorporationIdContractsGet](#schemacorporationscorporationidcontractsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|
|200|X-Pages|integer|int64|The total number of pages in the result set.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-contracts.read_corporation_contracts.v1 )
</aside>

## GetCorporationsCorporationIdContractsContractIdBids

<a id="opIdGetCorporationsCorporationIdContractsContractIdBids"></a>

`GET /corporations/{corporation_id}/contracts/{contract_id}/bids`

*Get corporation contract bids*

Lists bids on a particular auction contract

<h3 id="getcorporationscorporationidcontractscontractidbids-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|contract_id|path|integer(int64)|true|none|
|corporation_id|path|[CorporationID](#schemacorporationid)|true|The ID of the corporation|
|page|query|integer(int32)|false|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "amount": 0.1,
    "bid_id": 0,
    "bidder_id": 0,
    "date_bid": "2019-08-24T14:15:22Z"
  }
]
```

<h3 id="getcorporationscorporationidcontractscontractidbids-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CorporationsCorporationIdContractsContractIdBidsGet](#schemacorporationscorporationidcontractscontractidbidsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|
|200|X-Pages|integer|int64|The total number of pages in the result set.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-contracts.read_corporation_contracts.v1 )
</aside>

## GetCorporationsCorporationIdContractsContractIdItems

<a id="opIdGetCorporationsCorporationIdContractsContractIdItems"></a>

`GET /corporations/{corporation_id}/contracts/{contract_id}/items`

*Get corporation contract items*

Lists items of a particular contract

<h3 id="getcorporationscorporationidcontractscontractiditems-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|contract_id|path|integer(int64)|true|none|
|corporation_id|path|[CorporationID](#schemacorporationid)|true|The ID of the corporation|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "is_included": true,
    "is_singleton": true,
    "quantity": 0,
    "raw_quantity": 0,
    "record_id": 0,
    "type_id": 0
  }
]
```

<h3 id="getcorporationscorporationidcontractscontractiditems-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CorporationsCorporationIdContractsContractIdItemsGet](#schemacorporationscorporationidcontractscontractiditemsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-contracts.read_corporation_contracts.v1 )
</aside>

<h1 id="eve-stable-infrastructure-esi-tranquility-corporation">Corporation</h1>

## GetCorporationsNpccorps

<a id="opIdGetCorporationsNpccorps"></a>

`GET /corporations/npccorps`

*Get npc corporations*

Get a list of npc corporations

This route expires daily at 11:05

<h3 id="getcorporationsnpccorps-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  0
]
```

<h3 id="getcorporationsnpccorps-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CorporationsNpccorpsGet](#schemacorporationsnpccorpsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetCorporationsCorporationId

<a id="opIdGetCorporationsCorporationId"></a>

`GET /corporations/{corporation_id}`

*Get corporation information*

Public information about a corporation

<h3 id="getcorporationscorporationid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|corporation_id|path|[CorporationID](#schemacorporationid)|true|The ID of the corporation|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "alliance_id": 0,
  "ceo_id": 0,
  "creator_id": 0,
  "date_founded": "2019-08-24T14:15:22Z",
  "description": "string",
  "faction_id": 0,
  "home_station_id": 0,
  "member_count": 0,
  "name": "string",
  "shares": 0,
  "tax_rate": 0.1,
  "ticker": "string",
  "url": "string",
  "war_eligible": true
}
```

<h3 id="getcorporationscorporationid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CorporationsCorporationIdGet](#schemacorporationscorporationidget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetCorporationsCorporationIdAlliancehistory

<a id="opIdGetCorporationsCorporationIdAlliancehistory"></a>

`GET /corporations/{corporation_id}/alliancehistory`

*Get alliance history*

Get a list of all the alliances a corporation has been a member of

<h3 id="getcorporationscorporationidalliancehistory-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|corporation_id|path|[CorporationID](#schemacorporationid)|true|The ID of the corporation|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "alliance_id": 0,
    "is_deleted": true,
    "record_id": 0,
    "start_date": "2019-08-24T14:15:22Z"
  }
]
```

<h3 id="getcorporationscorporationidalliancehistory-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CorporationsCorporationIdAlliancehistoryGet](#schemacorporationscorporationidalliancehistoryget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetCorporationsCorporationIdBlueprints

<a id="opIdGetCorporationsCorporationIdBlueprints"></a>

`GET /corporations/{corporation_id}/blueprints`

*Get corporation blueprints*

Returns a list of blueprints the corporation owns

<h3 id="getcorporationscorporationidblueprints-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|corporation_id|path|[CorporationID](#schemacorporationid)|true|The ID of the corporation|
|page|query|integer(int32)|false|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "item_id": 0,
    "location_flag": "AssetSafety",
    "location_id": 0,
    "material_efficiency": 0,
    "quantity": 0,
    "runs": 0,
    "time_efficiency": 0,
    "type_id": 0
  }
]
```

<h3 id="getcorporationscorporationidblueprints-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CorporationsCorporationIdBlueprintsGet](#schemacorporationscorporationidblueprintsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|
|200|X-Pages|integer|int64|The total number of pages in the result set.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-corporations.read_blueprints.v1 )
</aside>

## GetCorporationsCorporationIdContainersLogs

<a id="opIdGetCorporationsCorporationIdContainersLogs"></a>

`GET /corporations/{corporation_id}/containers/logs`

*Get all corporation ALSC logs*

Returns logs recorded in the past seven days from all audit log secure containers (ALSC) owned by a given corporation

<h3 id="getcorporationscorporationidcontainerslogs-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|corporation_id|path|[CorporationID](#schemacorporationid)|true|The ID of the corporation|
|page|query|integer(int32)|false|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "action": "add",
    "character_id": 0,
    "container_id": 0,
    "container_type_id": 0,
    "location_flag": "AssetSafety",
    "location_id": 0,
    "logged_at": "2019-08-24T14:15:22Z",
    "new_config_bitmask": 0,
    "old_config_bitmask": 0,
    "password_type": "config",
    "quantity": 0,
    "type_id": 0
  }
]
```

<h3 id="getcorporationscorporationidcontainerslogs-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CorporationsCorporationIdContainersLogsGet](#schemacorporationscorporationidcontainerslogsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|
|200|X-Pages|integer|int64|The total number of pages in the result set.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-corporations.read_container_logs.v1 )
</aside>

## GetCorporationsCorporationIdDivisions

<a id="opIdGetCorporationsCorporationIdDivisions"></a>

`GET /corporations/{corporation_id}/divisions`

*Get corporation divisions*

Return corporation hangar and wallet division names, only show if a division is not using the default name

<h3 id="getcorporationscorporationiddivisions-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|corporation_id|path|[CorporationID](#schemacorporationid)|true|The ID of the corporation|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "hangar": [
    {
      "division": 0,
      "name": "string"
    }
  ],
  "wallet": [
    {
      "division": 0,
      "name": "string"
    }
  ]
}
```

<h3 id="getcorporationscorporationiddivisions-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CorporationsCorporationIdDivisionsGet](#schemacorporationscorporationiddivisionsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-corporations.read_divisions.v1 )
</aside>

## GetCorporationsCorporationIdFacilities

<a id="opIdGetCorporationsCorporationIdFacilities"></a>

`GET /corporations/{corporation_id}/facilities`

*Get corporation facilities*

Return a corporation's facilities

<h3 id="getcorporationscorporationidfacilities-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|corporation_id|path|[CorporationID](#schemacorporationid)|true|The ID of the corporation|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "facility_id": 0,
    "system_id": 0,
    "type_id": 0
  }
]
```

<h3 id="getcorporationscorporationidfacilities-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CorporationsCorporationIdFacilitiesGet](#schemacorporationscorporationidfacilitiesget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-corporations.read_facilities.v1 )
</aside>

## GetCorporationsCorporationIdIcons

<a id="opIdGetCorporationsCorporationIdIcons"></a>

`GET /corporations/{corporation_id}/icons`

*Get corporation icon*

Get the icon urls for a corporation

<h3 id="getcorporationscorporationidicons-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|corporation_id|path|[CorporationID](#schemacorporationid)|true|The ID of the corporation|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "px128x128": "string",
  "px256x256": "string",
  "px64x64": "string"
}
```

<h3 id="getcorporationscorporationidicons-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CorporationsCorporationIdIconsGet](#schemacorporationscorporationidiconsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetCorporationsCorporationIdMedals

<a id="opIdGetCorporationsCorporationIdMedals"></a>

`GET /corporations/{corporation_id}/medals`

*Get corporation medals*

Returns a corporation's medals

<h3 id="getcorporationscorporationidmedals-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|corporation_id|path|[CorporationID](#schemacorporationid)|true|The ID of the corporation|
|page|query|integer(int32)|false|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "created_at": "2019-08-24T14:15:22Z",
    "creator_id": 0,
    "description": "string",
    "medal_id": 0,
    "title": "string"
  }
]
```

<h3 id="getcorporationscorporationidmedals-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CorporationsCorporationIdMedalsGet](#schemacorporationscorporationidmedalsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|
|200|X-Pages|integer|int64|The total number of pages in the result set.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-corporations.read_medals.v1 )
</aside>

## GetCorporationsCorporationIdMedalsIssued

<a id="opIdGetCorporationsCorporationIdMedalsIssued"></a>

`GET /corporations/{corporation_id}/medals/issued`

*Get corporation issued medals*

Returns medals issued by a corporation

<h3 id="getcorporationscorporationidmedalsissued-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|corporation_id|path|[CorporationID](#schemacorporationid)|true|The ID of the corporation|
|page|query|integer(int32)|false|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "character_id": 0,
    "issued_at": "2019-08-24T14:15:22Z",
    "issuer_id": 0,
    "medal_id": 0,
    "reason": "string",
    "status": "private"
  }
]
```

<h3 id="getcorporationscorporationidmedalsissued-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CorporationsCorporationIdMedalsIssuedGet](#schemacorporationscorporationidmedalsissuedget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|
|200|X-Pages|integer|int64|The total number of pages in the result set.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-corporations.read_medals.v1 )
</aside>

## GetCorporationsCorporationIdMembers

<a id="opIdGetCorporationsCorporationIdMembers"></a>

`GET /corporations/{corporation_id}/members`

*Get corporation members*

Return the current member list of a corporation, the token's character need to be a member of the corporation.

<h3 id="getcorporationscorporationidmembers-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|corporation_id|path|[CorporationID](#schemacorporationid)|true|The ID of the corporation|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  0
]
```

<h3 id="getcorporationscorporationidmembers-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CorporationsCorporationIdMembersGet](#schemacorporationscorporationidmembersget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-corporations.read_corporation_membership.v1 )
</aside>

## GetCorporationsCorporationIdMembersLimit

<a id="opIdGetCorporationsCorporationIdMembersLimit"></a>

`GET /corporations/{corporation_id}/members/limit`

*Get corporation member limit*

Return a corporation's member limit, not including CEO himself

<h3 id="getcorporationscorporationidmemberslimit-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|corporation_id|path|[CorporationID](#schemacorporationid)|true|The ID of the corporation|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
0
```

<h3 id="getcorporationscorporationidmemberslimit-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CorporationsCorporationIdMembersLimitGet](#schemacorporationscorporationidmemberslimitget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-corporations.track_members.v1 )
</aside>

## GetCorporationsCorporationIdMembersTitles

<a id="opIdGetCorporationsCorporationIdMembersTitles"></a>

`GET /corporations/{corporation_id}/members/titles`

*Get corporation's members' titles*

Returns a corporation's members' titles

<h3 id="getcorporationscorporationidmemberstitles-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|corporation_id|path|[CorporationID](#schemacorporationid)|true|The ID of the corporation|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "character_id": 0,
    "titles": [
      0
    ]
  }
]
```

<h3 id="getcorporationscorporationidmemberstitles-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CorporationsCorporationIdMembersTitlesGet](#schemacorporationscorporationidmemberstitlesget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-corporations.read_titles.v1 )
</aside>

## GetCorporationsCorporationIdMembertracking

<a id="opIdGetCorporationsCorporationIdMembertracking"></a>

`GET /corporations/{corporation_id}/membertracking`

*Track corporation members*

Returns additional information about a corporation's members which helps tracking their activities

<h3 id="getcorporationscorporationidmembertracking-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|corporation_id|path|[CorporationID](#schemacorporationid)|true|The ID of the corporation|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "base_id": 0,
    "character_id": 0,
    "location_id": 0,
    "logoff_date": "2019-08-24T14:15:22Z",
    "logon_date": "2019-08-24T14:15:22Z",
    "ship_type_id": 0,
    "start_date": "2019-08-24T14:15:22Z"
  }
]
```

<h3 id="getcorporationscorporationidmembertracking-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CorporationsCorporationIdMembertrackingGet](#schemacorporationscorporationidmembertrackingget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-corporations.track_members.v1 )
</aside>

## GetCorporationsCorporationIdRoles

<a id="opIdGetCorporationsCorporationIdRoles"></a>

`GET /corporations/{corporation_id}/roles`

*Get corporation member roles*

Return the roles of all members if the character has the personnel manager role or any grantable role.

<h3 id="getcorporationscorporationidroles-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|corporation_id|path|[CorporationID](#schemacorporationid)|true|The ID of the corporation|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "character_id": 0,
    "grantable_roles": [
      "Account_Take_1"
    ],
    "grantable_roles_at_base": [
      "Account_Take_1"
    ],
    "grantable_roles_at_hq": [
      "Account_Take_1"
    ],
    "grantable_roles_at_other": [
      "Account_Take_1"
    ],
    "roles": [
      "Account_Take_1"
    ],
    "roles_at_base": [
      "Account_Take_1"
    ],
    "roles_at_hq": [
      "Account_Take_1"
    ],
    "roles_at_other": [
      "Account_Take_1"
    ]
  }
]
```

<h3 id="getcorporationscorporationidroles-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CorporationsCorporationIdRolesGet](#schemacorporationscorporationidrolesget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-corporations.read_corporation_membership.v1 )
</aside>

## GetCorporationsCorporationIdRolesHistory

<a id="opIdGetCorporationsCorporationIdRolesHistory"></a>

`GET /corporations/{corporation_id}/roles/history`

*Get corporation member roles history*

Return how roles have changed for a coporation's members, up to a month

<h3 id="getcorporationscorporationidroleshistory-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|corporation_id|path|[CorporationID](#schemacorporationid)|true|The ID of the corporation|
|page|query|integer(int32)|false|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "changed_at": "2019-08-24T14:15:22Z",
    "character_id": 0,
    "issuer_id": 0,
    "new_roles": [
      "Account_Take_1"
    ],
    "old_roles": [
      "Account_Take_1"
    ],
    "role_type": "grantable_roles"
  }
]
```

<h3 id="getcorporationscorporationidroleshistory-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CorporationsCorporationIdRolesHistoryGet](#schemacorporationscorporationidroleshistoryget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|
|200|X-Pages|integer|int64|The total number of pages in the result set.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-corporations.read_corporation_membership.v1 )
</aside>

## GetCorporationsCorporationIdShareholders

<a id="opIdGetCorporationsCorporationIdShareholders"></a>

`GET /corporations/{corporation_id}/shareholders`

*Get corporation shareholders*

Return the current shareholders of a corporation.

<h3 id="getcorporationscorporationidshareholders-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|corporation_id|path|[CorporationID](#schemacorporationid)|true|The ID of the corporation|
|page|query|integer(int32)|false|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "share_count": 0,
    "shareholder_id": 0,
    "shareholder_type": "character"
  }
]
```

<h3 id="getcorporationscorporationidshareholders-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CorporationsCorporationIdShareholdersGet](#schemacorporationscorporationidshareholdersget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|
|200|X-Pages|integer|int64|The total number of pages in the result set.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-wallet.read_corporation_wallets.v1 )
</aside>

## GetCorporationsCorporationIdStandings

<a id="opIdGetCorporationsCorporationIdStandings"></a>

`GET /corporations/{corporation_id}/standings`

*Get corporation standings*

Return corporation standings from agents, NPC corporations, and factions

<h3 id="getcorporationscorporationidstandings-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|corporation_id|path|[CorporationID](#schemacorporationid)|true|The ID of the corporation|
|page|query|integer(int32)|false|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "from_id": 0,
    "from_type": "agent",
    "standing": 0.1
  }
]
```

<h3 id="getcorporationscorporationidstandings-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CorporationsCorporationIdStandingsGet](#schemacorporationscorporationidstandingsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|
|200|X-Pages|integer|int64|The total number of pages in the result set.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-corporations.read_standings.v1 )
</aside>

## GetCorporationsCorporationIdStarbases

<a id="opIdGetCorporationsCorporationIdStarbases"></a>

`GET /corporations/{corporation_id}/starbases`

*Get corporation starbases (POSes)*

Returns list of corporation starbases (POSes)

<h3 id="getcorporationscorporationidstarbases-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|corporation_id|path|[CorporationID](#schemacorporationid)|true|The ID of the corporation|
|page|query|integer(int32)|false|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "moon_id": 0,
    "onlined_since": "2019-08-24T14:15:22Z",
    "reinforced_until": "2019-08-24T14:15:22Z",
    "starbase_id": 0,
    "state": "offline",
    "system_id": 0,
    "type_id": 0,
    "unanchor_at": "2019-08-24T14:15:22Z"
  }
]
```

<h3 id="getcorporationscorporationidstarbases-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CorporationsCorporationIdStarbasesGet](#schemacorporationscorporationidstarbasesget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|
|200|X-Pages|integer|int64|The total number of pages in the result set.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-corporations.read_starbases.v1 )
</aside>

## GetCorporationsCorporationIdStarbasesStarbaseId

<a id="opIdGetCorporationsCorporationIdStarbasesStarbaseId"></a>

`GET /corporations/{corporation_id}/starbases/{starbase_id}`

*Get starbase (POS) detail*

Returns various settings and fuels of a starbase (POS)

<h3 id="getcorporationscorporationidstarbasesstarbaseid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|corporation_id|path|[CorporationID](#schemacorporationid)|true|The ID of the corporation|
|starbase_id|path|integer(int64)|true|none|
|system_id|query|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "allow_alliance_members": true,
  "allow_corporation_members": true,
  "anchor": "alliance_member",
  "attack_if_at_war": true,
  "attack_if_other_security_status_dropping": true,
  "attack_security_status_threshold": 0.1,
  "attack_standing_threshold": 0.1,
  "fuel_bay_take": "alliance_member",
  "fuel_bay_view": "alliance_member",
  "fuels": [
    {
      "quantity": 0,
      "type_id": 0
    }
  ],
  "offline": "alliance_member",
  "online": "alliance_member",
  "unanchor": "alliance_member",
  "use_alliance_standings": true
}
```

<h3 id="getcorporationscorporationidstarbasesstarbaseid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CorporationsCorporationIdStarbasesStarbaseIdGet](#schemacorporationscorporationidstarbasesstarbaseidget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-corporations.read_starbases.v1 )
</aside>

## GetCorporationsCorporationIdStructures

<a id="opIdGetCorporationsCorporationIdStructures"></a>

`GET /corporations/{corporation_id}/structures`

*Get corporation structures*

Get a list of corporation structures. This route's version includes the changes to structures detailed in this blog: https://www.eveonline.com/article/upwell-2.0-structures-changes-coming-on-february-13th

<h3 id="getcorporationscorporationidstructures-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|corporation_id|path|[CorporationID](#schemacorporationid)|true|The ID of the corporation|
|page|query|integer(int32)|false|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "corporation_id": 0,
    "fuel_expires": "2019-08-24T14:15:22Z",
    "name": "string",
    "next_reinforce_apply": "2019-08-24T14:15:22Z",
    "next_reinforce_hour": 0,
    "profile_id": 0,
    "reinforce_hour": 0,
    "services": [
      {
        "name": "string",
        "state": "online"
      }
    ],
    "state": "anchor_vulnerable",
    "state_timer_end": "2019-08-24T14:15:22Z",
    "state_timer_start": "2019-08-24T14:15:22Z",
    "structure_id": 0,
    "system_id": 0,
    "type_id": 0,
    "unanchors_at": "2019-08-24T14:15:22Z"
  }
]
```

<h3 id="getcorporationscorporationidstructures-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CorporationsCorporationIdStructuresGet](#schemacorporationscorporationidstructuresget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|Content-Language|string||The language used in the response.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|
|200|X-Pages|integer|int64|The total number of pages in the result set.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-corporations.read_structures.v1 )
</aside>

## GetCorporationsCorporationIdTitles

<a id="opIdGetCorporationsCorporationIdTitles"></a>

`GET /corporations/{corporation_id}/titles`

*Get corporation titles*

Returns a corporation's titles

<h3 id="getcorporationscorporationidtitles-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|corporation_id|path|[CorporationID](#schemacorporationid)|true|The ID of the corporation|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "grantable_roles": [
      "Account_Take_1"
    ],
    "grantable_roles_at_base": [
      "Account_Take_1"
    ],
    "grantable_roles_at_hq": [
      "Account_Take_1"
    ],
    "grantable_roles_at_other": [
      "Account_Take_1"
    ],
    "name": "string",
    "roles": [
      "Account_Take_1"
    ],
    "roles_at_base": [
      "Account_Take_1"
    ],
    "roles_at_hq": [
      "Account_Take_1"
    ],
    "roles_at_other": [
      "Account_Take_1"
    ],
    "title_id": 0
  }
]
```

<h3 id="getcorporationscorporationidtitles-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CorporationsCorporationIdTitlesGet](#schemacorporationscorporationidtitlesget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-corporations.read_titles.v1 )
</aside>

<h1 id="eve-stable-infrastructure-esi-tranquility-corporation-projects">Corporation Projects</h1>

## GetCorporationsProjectsListing

<a id="opIdGetCorporationsProjectsListing"></a>

`GET /corporations/{corporation_id}/projects`

*List corporation projects*

Listing of all (active) corporation projects.

<h3 id="getcorporationsprojectslisting-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|after|query|string|false|Return records from after this cursor (mutual exclusive with 'before'). '0' to start from the beginning.|
|before|query|string|false|Return records from before this cursor (mutual exclusive with 'after'). '0' to start from the end.|
|limit|query|integer(int64)|false|The amount of records to retrieve per request.|
|corporation_id|path|[CorporationID](#schemacorporationid)|true|The ID of the corporation|
|state|query|string|false|Filter by state|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|state|All|
|state|Active|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "cursor": {
    "after": "string",
    "before": "string"
  },
  "projects": [
    {
      "id": "3868eaed-8278-4cb7-9709-7d7de9c20dc7",
      "last_modified": "2025-06-01T00:00:00Z",
      "name": "Project Name",
      "progress": {
        "current": 50,
        "desired": 100
      },
      "reward": {
        "initial": 12345.5,
        "remaining": 5432.1
      },
      "state": "Active"
    }
  ]
}
```

<h3 id="getcorporationsprojectslisting-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CorporationsProjectsListing](#schemacorporationsprojectslisting)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|
|default|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|default|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|default|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-corporations.read_projects.v1 )
</aside>

## GetCorporationsProjectsDetail

<a id="opIdGetCorporationsProjectsDetail"></a>

`GET /corporations/{corporation_id}/projects/{project_id}`

*Get project details*

Get the details of a corporation project.

<h3 id="getcorporationsprojectsdetail-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|If-Modified-Since|header|string|false|The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date.|
|corporation_id|path|[CorporationID](#schemacorporationid)|true|The ID of the corporation|
|project_id|path|[UUID](#schemauuid)|true|The ID of the project|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "configuration": {
    "capture_fw_complex": {
      "archetypes": [
        {
          "archetype_id": 33
        }
      ],
      "factions": [
        {
          "faction_id": 500002
        }
      ],
      "locations": [
        {
          "solar_system_id": 30000001
        }
      ]
    }
  },
  "contribution": {
    "participation_limit": 1000,
    "reward_per_contribution": 123.5,
    "submission_limit": 100,
    "submission_multiplier": 1.5
  },
  "creator": {
    "id": 90000001,
    "name": "Creator Name"
  },
  "details": {
    "career": "Explorer",
    "created": "2025-06-01T00:00:00Z",
    "description": "Project Description",
    "expires": "2025-06-01T00:01:00Z",
    "finished": "2025-06-01T00:00:00Z"
  },
  "id": "3868eaed-8278-4cb7-9709-7d7de9c20dc7",
  "last_modified": "2025-06-01T00:00:00Z",
  "name": "Project Name",
  "progress": {
    "current": 50,
    "desired": 100
  },
  "reward": {
    "initial": 12345.5,
    "remaining": 5432.1
  },
  "state": "Active"
}
```

<h3 id="getcorporationsprojectsdetail-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CorporationsProjectsDetail](#schemacorporationsprojectsdetail)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|
|default|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|default|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|default|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-corporations.read_projects.v1 )
</aside>

## GetCorporationsProjectsContribution

<a id="opIdGetCorporationsProjectsContribution"></a>

`GET /corporations/{corporation_id}/projects/{project_id}/contribution/{character_id}`

*Get your project contribution*

Show your contribution to a corporation project.

<h3 id="getcorporationsprojectscontribution-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|If-Modified-Since|header|string|false|The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date.|
|corporation_id|path|[CorporationID](#schemacorporationid)|true|The ID of the corporation|
|project_id|path|[UUID](#schemauuid)|true|The ID of the project|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "contributed": 10,
  "last_modified": "2025-08-26T00:00:00Z"
}
```

<h3 id="getcorporationsprojectscontribution-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CorporationsProjectsContribution](#schemacorporationsprojectscontribution)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|
|default|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|default|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|default|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-corporations.read_projects.v1 )
</aside>

## GetCorporationsProjectsContributors

<a id="opIdGetCorporationsProjectsContributors"></a>

`GET /corporations/{corporation_id}/projects/{project_id}/contributors`

*List project contributors*

Listing of all contributors to a corporation project.

<h3 id="getcorporationsprojectscontributors-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|after|query|string|false|Return records from after this cursor (mutual exclusive with 'before'). '0' to start from the beginning.|
|before|query|string|false|Return records from before this cursor (mutual exclusive with 'after'). '0' to start from the end.|
|limit|query|integer(int64)|false|The amount of records to retrieve per request.|
|corporation_id|path|[CorporationID](#schemacorporationid)|true|The ID of the corporation|
|project_id|path|[UUID](#schemauuid)|true|The ID of the project|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "contributors": [
    {
      "contributed": 10,
      "id": 90000001,
      "name": "Contributor Name"
    }
  ],
  "cursor": {
    "after": "string",
    "before": "string"
  }
}
```

<h3 id="getcorporationsprojectscontributors-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CorporationsProjectsContributors](#schemacorporationsprojectscontributors)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|
|default|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|default|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|default|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-corporations.read_projects.v1 )
</aside>

<h1 id="eve-stable-infrastructure-esi-tranquility-dogma">Dogma</h1>

## GetDogmaAttributes

<a id="opIdGetDogmaAttributes"></a>

`GET /dogma/attributes`

*Get attributes*

Get a list of dogma attribute ids

This route expires daily at 11:05

<h3 id="getdogmaattributes-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  0
]
```

<h3 id="getdogmaattributes-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[DogmaAttributesGet](#schemadogmaattributesget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetDogmaAttributesAttributeId

<a id="opIdGetDogmaAttributesAttributeId"></a>

`GET /dogma/attributes/{attribute_id}`

*Get attribute information*

Get information on a dogma attribute

This route expires daily at 11:05

<h3 id="getdogmaattributesattributeid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|attribute_id|path|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "attribute_id": 0,
  "default_value": 0.1,
  "description": "string",
  "display_name": "string",
  "high_is_good": true,
  "icon_id": 0,
  "name": "string",
  "published": true,
  "stackable": true,
  "unit_id": 0
}
```

<h3 id="getdogmaattributesattributeid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[DogmaAttributesAttributeIdGet](#schemadogmaattributesattributeidget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetDogmaDynamicItemsTypeIdItemId

<a id="opIdGetDogmaDynamicItemsTypeIdItemId"></a>

`GET /dogma/dynamic/items/{type_id}/{item_id}`

*Get dynamic item information*

Returns info about a dynamic item resulting from mutation with a mutaplasmid.

This route expires daily at 11:05

<h3 id="getdogmadynamicitemstypeiditemid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|item_id|path|integer(int64)|true|none|
|type_id|path|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "created_by": 0,
  "dogma_attributes": [
    {
      "attribute_id": 0,
      "value": 0.1
    }
  ],
  "dogma_effects": [
    {
      "effect_id": 0,
      "is_default": true
    }
  ],
  "mutator_type_id": 0,
  "source_type_id": 0
}
```

<h3 id="getdogmadynamicitemstypeiditemid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[DogmaDynamicItemsTypeIdItemIdGet](#schemadogmadynamicitemstypeiditemidget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetDogmaEffects

<a id="opIdGetDogmaEffects"></a>

`GET /dogma/effects`

*Get effects*

Get a list of dogma effect ids

This route expires daily at 11:05

<h3 id="getdogmaeffects-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  0
]
```

<h3 id="getdogmaeffects-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[DogmaEffectsGet](#schemadogmaeffectsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetDogmaEffectsEffectId

<a id="opIdGetDogmaEffectsEffectId"></a>

`GET /dogma/effects/{effect_id}`

*Get effect information*

Get information on a dogma effect

This route expires daily at 11:05

<h3 id="getdogmaeffectseffectid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|effect_id|path|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "description": "string",
  "disallow_auto_repeat": true,
  "discharge_attribute_id": 0,
  "display_name": "string",
  "duration_attribute_id": 0,
  "effect_category": 0,
  "effect_id": 0,
  "electronic_chance": true,
  "falloff_attribute_id": 0,
  "icon_id": 0,
  "is_assistance": true,
  "is_offensive": true,
  "is_warp_safe": true,
  "modifiers": [
    {
      "domain": "string",
      "effect_id": 0,
      "func": "string",
      "modified_attribute_id": 0,
      "modifying_attribute_id": 0,
      "operator": 0
    }
  ],
  "name": "string",
  "post_expression": 0,
  "pre_expression": 0,
  "published": true,
  "range_attribute_id": 0,
  "range_chance": true,
  "tracking_speed_attribute_id": 0
}
```

<h3 id="getdogmaeffectseffectid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[DogmaEffectsEffectIdGet](#schemadogmaeffectseffectidget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

<h1 id="eve-stable-infrastructure-esi-tranquility-faction-warfare">Faction Warfare</h1>

## GetCharactersCharacterIdFwStats

<a id="opIdGetCharactersCharacterIdFwStats"></a>

`GET /characters/{character_id}/fw/stats`

*Overview of a character involved in faction warfare*

Statistical overview of a character involved in faction warfare

This route expires daily at 11:05

<h3 id="getcharacterscharacteridfwstats-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "current_rank": 0,
  "enlisted_on": "2019-08-24T14:15:22Z",
  "faction_id": 0,
  "highest_rank": 0,
  "kills": {
    "last_week": 0,
    "total": 0,
    "yesterday": 0
  },
  "victory_points": {
    "last_week": 0,
    "total": 0,
    "yesterday": 0
  }
}
```

<h3 id="getcharacterscharacteridfwstats-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CharactersCharacterIdFwStatsGet](#schemacharacterscharacteridfwstatsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-characters.read_fw_stats.v1 )
</aside>

## GetCorporationsCorporationIdFwStats

<a id="opIdGetCorporationsCorporationIdFwStats"></a>

`GET /corporations/{corporation_id}/fw/stats`

*Overview of a corporation involved in faction warfare*

Statistics about a corporation involved in faction warfare

This route expires daily at 11:05

<h3 id="getcorporationscorporationidfwstats-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|corporation_id|path|[CorporationID](#schemacorporationid)|true|The ID of the corporation|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "enlisted_on": "2019-08-24T14:15:22Z",
  "faction_id": 0,
  "kills": {
    "last_week": 0,
    "total": 0,
    "yesterday": 0
  },
  "pilots": 0,
  "victory_points": {
    "last_week": 0,
    "total": 0,
    "yesterday": 0
  }
}
```

<h3 id="getcorporationscorporationidfwstats-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CorporationsCorporationIdFwStatsGet](#schemacorporationscorporationidfwstatsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-corporations.read_fw_stats.v1 )
</aside>

## GetFwLeaderboards

<a id="opIdGetFwLeaderboards"></a>

`GET /fw/leaderboards`

*List of the top factions in faction warfare*

Top 4 leaderboard of factions for kills and victory points separated by total, last week and yesterday

This route expires daily at 11:05

<h3 id="getfwleaderboards-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "kills": {
    "active_total": [
      {
        "amount": 0,
        "faction_id": 0
      }
    ],
    "last_week": [
      {
        "amount": 0,
        "faction_id": 0
      }
    ],
    "yesterday": [
      {
        "amount": 0,
        "faction_id": 0
      }
    ]
  },
  "victory_points": {
    "active_total": [
      {
        "amount": 0,
        "faction_id": 0
      }
    ],
    "last_week": [
      {
        "amount": 0,
        "faction_id": 0
      }
    ],
    "yesterday": [
      {
        "amount": 0,
        "faction_id": 0
      }
    ]
  }
}
```

<h3 id="getfwleaderboards-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[FwLeaderboardsGet](#schemafwleaderboardsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetFwLeaderboardsCharacters

<a id="opIdGetFwLeaderboardsCharacters"></a>

`GET /fw/leaderboards/characters`

*List of the top pilots in faction warfare*

Top 100 leaderboard of pilots for kills and victory points separated by total, last week and yesterday

This route expires daily at 11:05

<h3 id="getfwleaderboardscharacters-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "kills": {
    "active_total": [
      {
        "amount": 0,
        "character_id": 0
      }
    ],
    "last_week": [
      {
        "amount": 0,
        "character_id": 0
      }
    ],
    "yesterday": [
      {
        "amount": 0,
        "character_id": 0
      }
    ]
  },
  "victory_points": {
    "active_total": [
      {
        "amount": 0,
        "character_id": 0
      }
    ],
    "last_week": [
      {
        "amount": 0,
        "character_id": 0
      }
    ],
    "yesterday": [
      {
        "amount": 0,
        "character_id": 0
      }
    ]
  }
}
```

<h3 id="getfwleaderboardscharacters-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[FwLeaderboardsCharactersGet](#schemafwleaderboardscharactersget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetFwLeaderboardsCorporations

<a id="opIdGetFwLeaderboardsCorporations"></a>

`GET /fw/leaderboards/corporations`

*List of the top corporations in faction warfare*

Top 10 leaderboard of corporations for kills and victory points separated by total, last week and yesterday

This route expires daily at 11:05

<h3 id="getfwleaderboardscorporations-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "kills": {
    "active_total": [
      {
        "amount": 0,
        "corporation_id": 0
      }
    ],
    "last_week": [
      {
        "amount": 0,
        "corporation_id": 0
      }
    ],
    "yesterday": [
      {
        "amount": 0,
        "corporation_id": 0
      }
    ]
  },
  "victory_points": {
    "active_total": [
      {
        "amount": 0,
        "corporation_id": 0
      }
    ],
    "last_week": [
      {
        "amount": 0,
        "corporation_id": 0
      }
    ],
    "yesterday": [
      {
        "amount": 0,
        "corporation_id": 0
      }
    ]
  }
}
```

<h3 id="getfwleaderboardscorporations-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[FwLeaderboardsCorporationsGet](#schemafwleaderboardscorporationsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetFwStats

<a id="opIdGetFwStats"></a>

`GET /fw/stats`

*An overview of statistics about factions involved in faction warfare*

Statistical overviews of factions involved in faction warfare

This route expires daily at 11:05

<h3 id="getfwstats-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "faction_id": 0,
    "kills": {
      "last_week": 0,
      "total": 0,
      "yesterday": 0
    },
    "pilots": 0,
    "systems_controlled": 0,
    "victory_points": {
      "last_week": 0,
      "total": 0,
      "yesterday": 0
    }
  }
]
```

<h3 id="getfwstats-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[FwStatsGet](#schemafwstatsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetFwSystems

<a id="opIdGetFwSystems"></a>

`GET /fw/systems`

*Ownership of faction warfare systems*

An overview of the current ownership of faction warfare solar systems

<h3 id="getfwsystems-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "contested": "captured",
    "occupier_faction_id": 0,
    "owner_faction_id": 0,
    "solar_system_id": 0,
    "victory_points": 0,
    "victory_points_threshold": 0
  }
]
```

<h3 id="getfwsystems-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[FwSystemsGet](#schemafwsystemsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetFwWars

<a id="opIdGetFwWars"></a>

`GET /fw/wars`

*Data about which NPC factions are at war*

Data about which NPC factions are at war

This route expires daily at 11:05

<h3 id="getfwwars-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "against_id": 0,
    "faction_id": 0
  }
]
```

<h3 id="getfwwars-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[FwWarsGet](#schemafwwarsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

<h1 id="eve-stable-infrastructure-esi-tranquility-fittings">Fittings</h1>

## GetCharactersCharacterIdFittings

<a id="opIdGetCharactersCharacterIdFittings"></a>

`GET /characters/{character_id}/fittings`

*Get fittings*

Return fittings of a character

<h3 id="getcharacterscharacteridfittings-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "description": "string",
    "fitting_id": 0,
    "items": [
      {
        "flag": "Cargo",
        "quantity": 0,
        "type_id": 0
      }
    ],
    "name": "string",
    "ship_type_id": 0
  }
]
```

<h3 id="getcharacterscharacteridfittings-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CharactersCharacterIdFittingsGet](#schemacharacterscharacteridfittingsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-fittings.read_fittings.v1 )
</aside>

## PostCharactersCharacterIdFittings

<a id="opIdPostCharactersCharacterIdFittings"></a>

`POST /characters/{character_id}/fittings`

*Create fitting*

Save a new fitting for a character

> Body parameter

```json
{
  "description": "string",
  "items": [
    {
      "flag": "Cargo",
      "quantity": 0,
      "type_id": 0
    }
  ],
  "name": "string",
  "ship_type_id": 0
}
```

<h3 id="postcharacterscharacteridfittings-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|
|body|body|object|true|none|
|» description|body|string|true|none|
|» items|body|[object]|true|none|
|»» flag|body|string|true|Fitting location for the item. Entries placed in 'Invalid' will be discarded. If this leaves the fitting with nothing, it will cause an error.|
|»» quantity|body|integer(int64)|true|none|
|»» type_id|body|integer(int64)|true|none|
|» name|body|string|true|none|
|» ship_type_id|body|integer(int64)|true|none|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|
|»» flag|Cargo|
|»» flag|DroneBay|
|»» flag|FighterBay|
|»» flag|HiSlot0|
|»» flag|HiSlot1|
|»» flag|HiSlot2|
|»» flag|HiSlot3|
|»» flag|HiSlot4|
|»» flag|HiSlot5|
|»» flag|HiSlot6|
|»» flag|HiSlot7|
|»» flag|Invalid|
|»» flag|LoSlot0|
|»» flag|LoSlot1|
|»» flag|LoSlot2|
|»» flag|LoSlot3|
|»» flag|LoSlot4|
|»» flag|LoSlot5|
|»» flag|LoSlot6|
|»» flag|LoSlot7|
|»» flag|MedSlot0|
|»» flag|MedSlot1|
|»» flag|MedSlot2|
|»» flag|MedSlot3|
|»» flag|MedSlot4|
|»» flag|MedSlot5|
|»» flag|MedSlot6|
|»» flag|MedSlot7|
|»» flag|RigSlot0|
|»» flag|RigSlot1|
|»» flag|RigSlot2|
|»» flag|ServiceSlot0|
|»» flag|ServiceSlot1|
|»» flag|ServiceSlot2|
|»» flag|ServiceSlot3|
|»» flag|ServiceSlot4|
|»» flag|ServiceSlot5|
|»» flag|ServiceSlot6|
|»» flag|ServiceSlot7|
|»» flag|SubSystemSlot0|
|»» flag|SubSystemSlot1|
|»» flag|SubSystemSlot2|
|»» flag|SubSystemSlot3|

> Example responses

> 201 Response

```json
{
  "fitting_id": 0
}
```

<h3 id="postcharacterscharacteridfittings-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|[CharactersCharacterIdFittingsPost](#schemacharacterscharacteridfittingspost)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|201|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|201|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|201|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-fittings.write_fittings.v1 )
</aside>

## DeleteCharactersCharacterIdFittingsFittingId

<a id="opIdDeleteCharactersCharacterIdFittingsFittingId"></a>

`DELETE /characters/{character_id}/fittings/{fitting_id}`

*Delete fitting*

Delete a fitting from a character

<h3 id="deletecharacterscharacteridfittingsfittingid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|fitting_id|path|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> default Response

```json
{
  "details": [
    {
      "location": "string",
      "message": "string",
      "value": null
    }
  ],
  "error": "string"
}
```

<h3 id="deletecharacterscharacteridfittingsfittingid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|204|[No Content](https://tools.ietf.org/html/rfc7231#section-6.3.5)|Fitting deleted|None|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|204|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|204|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|204|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-fittings.write_fittings.v1 )
</aside>

<h1 id="eve-stable-infrastructure-esi-tranquility-fleets">Fleets</h1>

## GetCharactersCharacterIdFleet

<a id="opIdGetCharactersCharacterIdFleet"></a>

`GET /characters/{character_id}/fleet`

*Get character fleet info*

Return the fleet ID the character is in, if any.

<h3 id="getcharacterscharacteridfleet-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "fleet_boss_id": 0,
  "fleet_id": 0,
  "role": "fleet_commander",
  "squad_id": 0,
  "wing_id": 0
}
```

<h3 id="getcharacterscharacteridfleet-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CharactersCharacterIdFleetGet](#schemacharacterscharacteridfleetget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-fleets.read_fleet.v1 )
</aside>

## GetFleetsFleetId

<a id="opIdGetFleetsFleetId"></a>

`GET /fleets/{fleet_id}`

*Get fleet information*

Return details about a fleet

<h3 id="getfleetsfleetid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|fleet_id|path|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "is_free_move": true,
  "is_registered": true,
  "is_voice_enabled": true,
  "motd": "string"
}
```

<h3 id="getfleetsfleetid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[FleetsFleetIdGet](#schemafleetsfleetidget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-fleets.read_fleet.v1 )
</aside>

## PutFleetsFleetId

<a id="opIdPutFleetsFleetId"></a>

`PUT /fleets/{fleet_id}`

*Update fleet*

Update settings about a fleet

> Body parameter

```json
{
  "is_free_move": true,
  "motd": "string"
}
```

<h3 id="putfleetsfleetid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|fleet_id|path|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|
|body|body|object|true|none|
|» is_free_move|body|boolean|false|Should free-move be enabled in the fleet|
|» motd|body|string|false|New fleet MOTD in CCP flavoured HTML|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> default Response

```json
{
  "details": [
    {
      "location": "string",
      "message": "string",
      "value": null
    }
  ],
  "error": "string"
}
```

<h3 id="putfleetsfleetid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|204|[No Content](https://tools.ietf.org/html/rfc7231#section-6.3.5)|Fleet updated|None|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|204|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|204|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|204|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-fleets.write_fleet.v1 )
</aside>

## GetFleetsFleetIdMembers

<a id="opIdGetFleetsFleetIdMembers"></a>

`GET /fleets/{fleet_id}/members`

*Get fleet members*

Return information about fleet members

<h3 id="getfleetsfleetidmembers-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|fleet_id|path|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "character_id": 0,
    "join_time": "2019-08-24T14:15:22Z",
    "role": "fleet_commander",
    "role_name": "string",
    "ship_type_id": 0,
    "solar_system_id": 0,
    "squad_id": 0,
    "station_id": 0,
    "takes_fleet_warp": true,
    "wing_id": 0
  }
]
```

<h3 id="getfleetsfleetidmembers-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[FleetsFleetIdMembersGet](#schemafleetsfleetidmembersget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|Content-Language|string||The language used in the response.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-fleets.read_fleet.v1 )
</aside>

## PostFleetsFleetIdMembers

<a id="opIdPostFleetsFleetIdMembers"></a>

`POST /fleets/{fleet_id}/members`

*Create fleet invitation*

Invite a character into the fleet. If a character has a CSPA charge set it is not possible to invite them to the fleet using ESI

> Body parameter

```json
{
  "character_id": 0,
  "role": "fleet_commander",
  "squad_id": 0,
  "wing_id": 0
}
```

<h3 id="postfleetsfleetidmembers-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|fleet_id|path|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|
|body|body|object|true|none|
|» character_id|body|integer(int64)|true|The character you want to invite|
|» role|body|string|true|If a character is invited with the `fleet_commander` role, neither `wing_id` or `squad_id` should be specified. If a character is invited with the `wing_commander` role, only `wing_id` should be specified. If a character is invited with the `squad_commander` role, both `wing_id` and `squad_id` should be specified. If a character is invited with the `squad_member` role, `wing_id` and `squad_id` should either both be specified or not specified at all. If they aren’t specified, the invited character will join any squad with available positions.|
|» squad_id|body|integer(int64)|false|none|
|» wing_id|body|integer(int64)|false|none|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|
|» role|fleet_commander|
|» role|wing_commander|
|» role|squad_commander|
|» role|squad_member|

> Example responses

> default Response

```json
{
  "details": [
    {
      "location": "string",
      "message": "string",
      "value": null
    }
  ],
  "error": "string"
}
```

<h3 id="postfleetsfleetidmembers-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|204|[No Content](https://tools.ietf.org/html/rfc7231#section-6.3.5)|Fleet invitation sent|None|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|204|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|204|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|204|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-fleets.write_fleet.v1 )
</aside>

## DeleteFleetsFleetIdMembersMemberId

<a id="opIdDeleteFleetsFleetIdMembersMemberId"></a>

`DELETE /fleets/{fleet_id}/members/{member_id}`

*Kick fleet member*

Kick a fleet member

<h3 id="deletefleetsfleetidmembersmemberid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|fleet_id|path|integer(int64)|true|none|
|member_id|path|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> default Response

```json
{
  "details": [
    {
      "location": "string",
      "message": "string",
      "value": null
    }
  ],
  "error": "string"
}
```

<h3 id="deletefleetsfleetidmembersmemberid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|204|[No Content](https://tools.ietf.org/html/rfc7231#section-6.3.5)|Fleet member kicked|None|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|204|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|204|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|204|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-fleets.write_fleet.v1 )
</aside>

## PutFleetsFleetIdMembersMemberId

<a id="opIdPutFleetsFleetIdMembersMemberId"></a>

`PUT /fleets/{fleet_id}/members/{member_id}`

*Move fleet member*

Move a fleet member around

> Body parameter

```json
{
  "role": "fleet_commander",
  "squad_id": 0,
  "wing_id": 0
}
```

<h3 id="putfleetsfleetidmembersmemberid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|fleet_id|path|integer(int64)|true|none|
|member_id|path|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|
|body|body|object|true|none|
|» role|body|string|true|If a character is moved to the `fleet_commander` role, neither `wing_id` or `squad_id` should be specified. If a character is moved to the `wing_commander` role, only `wing_id` should be specified. If a character is moved to the `squad_commander` role, both `wing_id` and `squad_id` should be specified. If a character is moved to the `squad_member` role, both `wing_id` and `squad_id` should be specified.|
|» squad_id|body|integer(int64)|false|none|
|» wing_id|body|integer(int64)|false|none|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|
|» role|fleet_commander|
|» role|wing_commander|
|» role|squad_commander|
|» role|squad_member|

> Example responses

> default Response

```json
{
  "details": [
    {
      "location": "string",
      "message": "string",
      "value": null
    }
  ],
  "error": "string"
}
```

<h3 id="putfleetsfleetidmembersmemberid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|204|[No Content](https://tools.ietf.org/html/rfc7231#section-6.3.5)|Fleet invitation sent|None|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|204|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|204|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|204|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-fleets.write_fleet.v1 )
</aside>

## DeleteFleetsFleetIdSquadsSquadId

<a id="opIdDeleteFleetsFleetIdSquadsSquadId"></a>

`DELETE /fleets/{fleet_id}/squads/{squad_id}`

*Delete fleet squad*

Delete a fleet squad, only empty squads can be deleted

<h3 id="deletefleetsfleetidsquadssquadid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|fleet_id|path|integer(int64)|true|none|
|squad_id|path|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> default Response

```json
{
  "details": [
    {
      "location": "string",
      "message": "string",
      "value": null
    }
  ],
  "error": "string"
}
```

<h3 id="deletefleetsfleetidsquadssquadid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|204|[No Content](https://tools.ietf.org/html/rfc7231#section-6.3.5)|Squad deleted|None|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|204|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|204|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|204|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-fleets.write_fleet.v1 )
</aside>

## PutFleetsFleetIdSquadsSquadId

<a id="opIdPutFleetsFleetIdSquadsSquadId"></a>

`PUT /fleets/{fleet_id}/squads/{squad_id}`

*Rename fleet squad*

Rename a fleet squad

> Body parameter

```json
{
  "name": "string"
}
```

<h3 id="putfleetsfleetidsquadssquadid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|fleet_id|path|integer(int64)|true|none|
|squad_id|path|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|
|body|body|object|true|none|
|» name|body|string|true|none|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> default Response

```json
{
  "details": [
    {
      "location": "string",
      "message": "string",
      "value": null
    }
  ],
  "error": "string"
}
```

<h3 id="putfleetsfleetidsquadssquadid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|204|[No Content](https://tools.ietf.org/html/rfc7231#section-6.3.5)|Squad renamed|None|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|204|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|204|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|204|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-fleets.write_fleet.v1 )
</aside>

## GetFleetsFleetIdWings

<a id="opIdGetFleetsFleetIdWings"></a>

`GET /fleets/{fleet_id}/wings`

*Get fleet wings*

Return information about wings in a fleet

<h3 id="getfleetsfleetidwings-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|fleet_id|path|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "id": 0,
    "name": "string",
    "squads": [
      {
        "id": 0,
        "name": "string"
      }
    ]
  }
]
```

<h3 id="getfleetsfleetidwings-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[FleetsFleetIdWingsGet](#schemafleetsfleetidwingsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|Content-Language|string||The language used in the response.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-fleets.read_fleet.v1 )
</aside>

## PostFleetsFleetIdWings

<a id="opIdPostFleetsFleetIdWings"></a>

`POST /fleets/{fleet_id}/wings`

*Create fleet wing*

Create a new wing in a fleet

<h3 id="postfleetsfleetidwings-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|fleet_id|path|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 201 Response

```json
{
  "wing_id": 0
}
```

<h3 id="postfleetsfleetidwings-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|[FleetsFleetIdWingsPost](#schemafleetsfleetidwingspost)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|201|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|201|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|201|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-fleets.write_fleet.v1 )
</aside>

## DeleteFleetsFleetIdWingsWingId

<a id="opIdDeleteFleetsFleetIdWingsWingId"></a>

`DELETE /fleets/{fleet_id}/wings/{wing_id}`

*Delete fleet wing*

Delete a fleet wing, only empty wings can be deleted. The wing may contain squads, but the squads must be empty

<h3 id="deletefleetsfleetidwingswingid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|fleet_id|path|integer(int64)|true|none|
|wing_id|path|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> default Response

```json
{
  "details": [
    {
      "location": "string",
      "message": "string",
      "value": null
    }
  ],
  "error": "string"
}
```

<h3 id="deletefleetsfleetidwingswingid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|204|[No Content](https://tools.ietf.org/html/rfc7231#section-6.3.5)|Wing deleted|None|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|204|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|204|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|204|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-fleets.write_fleet.v1 )
</aside>

## PutFleetsFleetIdWingsWingId

<a id="opIdPutFleetsFleetIdWingsWingId"></a>

`PUT /fleets/{fleet_id}/wings/{wing_id}`

*Rename fleet wing*

Rename a fleet wing

> Body parameter

```json
{
  "name": "string"
}
```

<h3 id="putfleetsfleetidwingswingid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|fleet_id|path|integer(int64)|true|none|
|wing_id|path|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|
|body|body|object|true|none|
|» name|body|string|true|none|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> default Response

```json
{
  "details": [
    {
      "location": "string",
      "message": "string",
      "value": null
    }
  ],
  "error": "string"
}
```

<h3 id="putfleetsfleetidwingswingid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|204|[No Content](https://tools.ietf.org/html/rfc7231#section-6.3.5)|Wing renamed|None|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|204|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|204|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|204|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-fleets.write_fleet.v1 )
</aside>

## PostFleetsFleetIdWingsWingIdSquads

<a id="opIdPostFleetsFleetIdWingsWingIdSquads"></a>

`POST /fleets/{fleet_id}/wings/{wing_id}/squads`

*Create fleet squad*

Create a new squad in a fleet

<h3 id="postfleetsfleetidwingswingidsquads-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|fleet_id|path|integer(int64)|true|none|
|wing_id|path|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 201 Response

```json
{
  "squad_id": 0
}
```

<h3 id="postfleetsfleetidwingswingidsquads-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|[FleetsFleetIdWingsWingIdSquadsPost](#schemafleetsfleetidwingswingidsquadspost)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|201|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|201|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|201|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-fleets.write_fleet.v1 )
</aside>

<h1 id="eve-stable-infrastructure-esi-tranquility-incursions">Incursions</h1>

## GetIncursions

<a id="opIdGetIncursions"></a>

`GET /incursions`

*List incursions*

Return a list of current incursions

<h3 id="getincursions-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "constellation_id": 0,
    "faction_id": 0,
    "has_boss": true,
    "infested_solar_systems": [
      0
    ],
    "influence": 0.1,
    "staging_solar_system_id": 0,
    "state": "withdrawing",
    "type": "string"
  }
]
```

<h3 id="getincursions-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[IncursionsGet](#schemaincursionsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

<h1 id="eve-stable-infrastructure-esi-tranquility-industry">Industry</h1>

## GetCharactersCharacterIdIndustryJobs

<a id="opIdGetCharactersCharacterIdIndustryJobs"></a>

`GET /characters/{character_id}/industry/jobs`

*List character industry jobs*

List industry jobs placed by a character

<h3 id="getcharacterscharacteridindustryjobs-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|include_completed|query|boolean|false|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "activity_id": 0,
    "blueprint_id": 0,
    "blueprint_location_id": 0,
    "blueprint_type_id": 0,
    "completed_character_id": 0,
    "completed_date": "2019-08-24T14:15:22Z",
    "cost": 0.1,
    "duration": 0,
    "end_date": "2019-08-24T14:15:22Z",
    "facility_id": 0,
    "installer_id": 0,
    "job_id": 0,
    "licensed_runs": 0,
    "output_location_id": 0,
    "pause_date": "2019-08-24T14:15:22Z",
    "probability": 0.1,
    "product_type_id": 0,
    "runs": 0,
    "start_date": "2019-08-24T14:15:22Z",
    "station_id": 0,
    "status": "active",
    "successful_runs": 0
  }
]
```

<h3 id="getcharacterscharacteridindustryjobs-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CharactersCharacterIdIndustryJobsGet](#schemacharacterscharacteridindustryjobsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-industry.read_character_jobs.v1 )
</aside>

## GetCharactersCharacterIdMining

<a id="opIdGetCharactersCharacterIdMining"></a>

`GET /characters/{character_id}/mining`

*Character mining ledger*

Paginated record of all mining done by a character for the past 30 days

<h3 id="getcharacterscharacteridmining-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|page|query|integer(int32)|false|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "date": "2019-08-24",
    "quantity": 0,
    "solar_system_id": 0,
    "type_id": 0
  }
]
```

<h3 id="getcharacterscharacteridmining-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CharactersCharacterIdMiningGet](#schemacharacterscharacteridminingget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|
|200|X-Pages|integer|int64|The total number of pages in the result set.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-industry.read_character_mining.v1 )
</aside>

## GetCorporationCorporationIdMiningExtractions

<a id="opIdGetCorporationCorporationIdMiningExtractions"></a>

`GET /corporation/{corporation_id}/mining/extractions`

*Moon extraction timers*

Extraction timers for all moon chunks being extracted by refineries belonging to a corporation.

<h3 id="getcorporationcorporationidminingextractions-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|corporation_id|path|[CorporationID](#schemacorporationid)|true|The ID of the corporation|
|page|query|integer(int32)|false|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "chunk_arrival_time": "2019-08-24T14:15:22Z",
    "extraction_start_time": "2019-08-24T14:15:22Z",
    "moon_id": 0,
    "natural_decay_time": "2019-08-24T14:15:22Z",
    "structure_id": 0
  }
]
```

<h3 id="getcorporationcorporationidminingextractions-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CorporationCorporationIdMiningExtractionsGet](#schemacorporationcorporationidminingextractionsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|
|200|X-Pages|integer|int64|The total number of pages in the result set.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-industry.read_corporation_mining.v1 )
</aside>

## GetCorporationCorporationIdMiningObservers

<a id="opIdGetCorporationCorporationIdMiningObservers"></a>

`GET /corporation/{corporation_id}/mining/observers`

*Corporation mining observers*

Paginated list of all entities capable of observing and recording mining for a corporation

<h3 id="getcorporationcorporationidminingobservers-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|corporation_id|path|[CorporationID](#schemacorporationid)|true|The ID of the corporation|
|page|query|integer(int32)|false|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "last_updated": "2019-08-24",
    "observer_id": 0,
    "observer_type": "structure"
  }
]
```

<h3 id="getcorporationcorporationidminingobservers-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CorporationCorporationIdMiningObserversGet](#schemacorporationcorporationidminingobserversget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|
|200|X-Pages|integer|int64|The total number of pages in the result set.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-industry.read_corporation_mining.v1 )
</aside>

## GetCorporationCorporationIdMiningObserversObserverId

<a id="opIdGetCorporationCorporationIdMiningObserversObserverId"></a>

`GET /corporation/{corporation_id}/mining/observers/{observer_id}`

*Observed corporation mining*

Paginated record of all mining seen by an observer

<h3 id="getcorporationcorporationidminingobserversobserverid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|corporation_id|path|[CorporationID](#schemacorporationid)|true|The ID of the corporation|
|observer_id|path|integer(int64)|true|none|
|page|query|integer(int32)|false|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "character_id": 0,
    "last_updated": "2019-08-24",
    "quantity": 0,
    "recorded_corporation_id": 0,
    "type_id": 0
  }
]
```

<h3 id="getcorporationcorporationidminingobserversobserverid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CorporationCorporationIdMiningObserversObserverIdGet](#schemacorporationcorporationidminingobserversobserveridget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|
|200|X-Pages|integer|int64|The total number of pages in the result set.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-industry.read_corporation_mining.v1 )
</aside>

## GetCorporationsCorporationIdIndustryJobs

<a id="opIdGetCorporationsCorporationIdIndustryJobs"></a>

`GET /corporations/{corporation_id}/industry/jobs`

*List corporation industry jobs*

List industry jobs run by a corporation

<h3 id="getcorporationscorporationidindustryjobs-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|corporation_id|path|[CorporationID](#schemacorporationid)|true|The ID of the corporation|
|include_completed|query|boolean|false|none|
|page|query|integer(int32)|false|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "activity_id": 0,
    "blueprint_id": 0,
    "blueprint_location_id": 0,
    "blueprint_type_id": 0,
    "completed_character_id": 0,
    "completed_date": "2019-08-24T14:15:22Z",
    "cost": 0.1,
    "duration": 0,
    "end_date": "2019-08-24T14:15:22Z",
    "facility_id": 0,
    "installer_id": 0,
    "job_id": 0,
    "licensed_runs": 0,
    "location_id": 0,
    "output_location_id": 0,
    "pause_date": "2019-08-24T14:15:22Z",
    "probability": 0.1,
    "product_type_id": 0,
    "runs": 0,
    "start_date": "2019-08-24T14:15:22Z",
    "status": "active",
    "successful_runs": 0
  }
]
```

<h3 id="getcorporationscorporationidindustryjobs-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CorporationsCorporationIdIndustryJobsGet](#schemacorporationscorporationidindustryjobsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|
|200|X-Pages|integer|int64|The total number of pages in the result set.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-industry.read_corporation_jobs.v1 )
</aside>

## GetIndustryFacilities

<a id="opIdGetIndustryFacilities"></a>

`GET /industry/facilities`

*List industry facilities*

Return a list of industry facilities

<h3 id="getindustryfacilities-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "facility_id": 0,
    "owner_id": 0,
    "region_id": 0,
    "solar_system_id": 0,
    "tax": 0.1,
    "type_id": 0
  }
]
```

<h3 id="getindustryfacilities-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[IndustryFacilitiesGet](#schemaindustryfacilitiesget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetIndustrySystems

<a id="opIdGetIndustrySystems"></a>

`GET /industry/systems`

*List solar system cost indices*

Return cost indices for solar systems

<h3 id="getindustrysystems-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "cost_indices": [
      {
        "activity": "copying",
        "cost_index": 0.1
      }
    ],
    "solar_system_id": 0
  }
]
```

<h3 id="getindustrysystems-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[IndustrySystemsGet](#schemaindustrysystemsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

<h1 id="eve-stable-infrastructure-esi-tranquility-insurance">Insurance</h1>

## GetInsurancePrices

<a id="opIdGetInsurancePrices"></a>

`GET /insurance/prices`

*List insurance levels*

Return available insurance levels for all ship types

<h3 id="getinsuranceprices-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "levels": [
      {
        "cost": 0.1,
        "name": "string",
        "payout": 0.1
      }
    ],
    "type_id": 0
  }
]
```

<h3 id="getinsuranceprices-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[InsurancePricesGet](#schemainsurancepricesget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|Content-Language|string||The language used in the response.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

<h1 id="eve-stable-infrastructure-esi-tranquility-killmails">Killmails</h1>

## GetCharactersCharacterIdKillmailsRecent

<a id="opIdGetCharactersCharacterIdKillmailsRecent"></a>

`GET /characters/{character_id}/killmails/recent`

*Get a character's recent kills and losses*

Return a list of a character's kills and losses going back 90 days

<h3 id="getcharacterscharacteridkillmailsrecent-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|page|query|integer(int32)|false|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "killmail_hash": "string",
    "killmail_id": 0
  }
]
```

<h3 id="getcharacterscharacteridkillmailsrecent-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CharactersCharacterIdKillmailsRecentGet](#schemacharacterscharacteridkillmailsrecentget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|
|200|X-Pages|integer|int64|The total number of pages in the result set.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-killmails.read_killmails.v1 )
</aside>

## GetCorporationsCorporationIdKillmailsRecent

<a id="opIdGetCorporationsCorporationIdKillmailsRecent"></a>

`GET /corporations/{corporation_id}/killmails/recent`

*Get a corporation's recent kills and losses*

Get a list of a corporation's kills and losses going back 90 days

<h3 id="getcorporationscorporationidkillmailsrecent-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|corporation_id|path|[CorporationID](#schemacorporationid)|true|The ID of the corporation|
|page|query|integer(int32)|false|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "killmail_hash": "string",
    "killmail_id": 0
  }
]
```

<h3 id="getcorporationscorporationidkillmailsrecent-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CorporationsCorporationIdKillmailsRecentGet](#schemacorporationscorporationidkillmailsrecentget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|
|200|X-Pages|integer|int64|The total number of pages in the result set.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-killmails.read_corporation_killmails.v1 )
</aside>

## GetKillmailsKillmailIdKillmailHash

<a id="opIdGetKillmailsKillmailIdKillmailHash"></a>

`GET /killmails/{killmail_id}/{killmail_hash}`

*Get a single killmail*

Return a single killmail from its ID and hash

<h3 id="getkillmailskillmailidkillmailhash-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|killmail_hash|path|string|true|none|
|killmail_id|path|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "attackers": [
    {
      "alliance_id": 0,
      "character_id": 0,
      "corporation_id": 0,
      "damage_done": 0,
      "faction_id": 0,
      "final_blow": true,
      "security_status": 0.1,
      "ship_type_id": 0,
      "weapon_type_id": 0
    }
  ],
  "killmail_id": 0,
  "killmail_time": "2019-08-24T14:15:22Z",
  "moon_id": 0,
  "solar_system_id": 0,
  "victim": {
    "alliance_id": 0,
    "character_id": 0,
    "corporation_id": 0,
    "damage_taken": 0,
    "faction_id": 0,
    "items": [
      {
        "flag": 0,
        "item_type_id": 0,
        "items": [
          {
            "flag": 0,
            "item_type_id": 0,
            "quantity_destroyed": 0,
            "quantity_dropped": 0,
            "singleton": 0
          }
        ],
        "quantity_destroyed": 0,
        "quantity_dropped": 0,
        "singleton": 0
      }
    ],
    "position": {
      "x": 0.1,
      "y": 0.1,
      "z": 0.1
    },
    "ship_type_id": 0
  },
  "war_id": 0
}
```

<h3 id="getkillmailskillmailidkillmailhash-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[KillmailsKillmailIdKillmailHashGet](#schemakillmailskillmailidkillmailhashget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

<h1 id="eve-stable-infrastructure-esi-tranquility-location">Location</h1>

## GetCharactersCharacterIdLocation

<a id="opIdGetCharactersCharacterIdLocation"></a>

`GET /characters/{character_id}/location`

*Get character location*

Information about the characters current location. Returns the current solar system id, and also the current station or structure ID if applicable

<h3 id="getcharacterscharacteridlocation-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "solar_system_id": 0,
  "station_id": 0,
  "structure_id": 0
}
```

<h3 id="getcharacterscharacteridlocation-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CharactersCharacterIdLocationGet](#schemacharacterscharacteridlocationget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-location.read_location.v1 )
</aside>

## GetCharactersCharacterIdOnline

<a id="opIdGetCharactersCharacterIdOnline"></a>

`GET /characters/{character_id}/online`

*Get character online*

Checks if the character is currently online

<h3 id="getcharacterscharacteridonline-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "last_login": "2019-08-24T14:15:22Z",
  "last_logout": "2019-08-24T14:15:22Z",
  "logins": 0,
  "online": true
}
```

<h3 id="getcharacterscharacteridonline-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CharactersCharacterIdOnlineGet](#schemacharacterscharacteridonlineget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-location.read_online.v1 )
</aside>

## GetCharactersCharacterIdShip

<a id="opIdGetCharactersCharacterIdShip"></a>

`GET /characters/{character_id}/ship`

*Get current ship*

Get the current ship type, name and id

<h3 id="getcharacterscharacteridship-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "ship_item_id": 0,
  "ship_name": "string",
  "ship_type_id": 0
}
```

<h3 id="getcharacterscharacteridship-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CharactersCharacterIdShipGet](#schemacharacterscharacteridshipget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-location.read_ship_type.v1 )
</aside>

<h1 id="eve-stable-infrastructure-esi-tranquility-loyalty">Loyalty</h1>

## GetCharactersCharacterIdLoyaltyPoints

<a id="opIdGetCharactersCharacterIdLoyaltyPoints"></a>

`GET /characters/{character_id}/loyalty/points`

*Get loyalty points*

Return a list of loyalty points for all corporations the character has worked for

<h3 id="getcharacterscharacteridloyaltypoints-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "corporation_id": 0,
    "loyalty_points": 0
  }
]
```

<h3 id="getcharacterscharacteridloyaltypoints-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CharactersCharacterIdLoyaltyPointsGet](#schemacharacterscharacteridloyaltypointsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-characters.read_loyalty.v1 )
</aside>

## GetLoyaltyStoresCorporationIdOffers

<a id="opIdGetLoyaltyStoresCorporationIdOffers"></a>

`GET /loyalty/stores/{corporation_id}/offers`

*List loyalty store offers*

Return a list of offers from a specific corporation's loyalty store

This route expires daily at 11:05

<h3 id="getloyaltystorescorporationidoffers-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|corporation_id|path|[CorporationID](#schemacorporationid)|true|The ID of the corporation|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "ak_cost": 0,
    "isk_cost": 0,
    "lp_cost": 0,
    "offer_id": 0,
    "quantity": 0,
    "required_items": [
      {
        "quantity": 0,
        "type_id": 0
      }
    ],
    "type_id": 0
  }
]
```

<h3 id="getloyaltystorescorporationidoffers-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[LoyaltyStoresCorporationIdOffersGet](#schemaloyaltystorescorporationidoffersget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

<h1 id="eve-stable-infrastructure-esi-tranquility-mail">Mail</h1>

## GetCharactersCharacterIdMail

<a id="opIdGetCharactersCharacterIdMail"></a>

`GET /characters/{character_id}/mail`

*Return mail headers*

Return the 50 most recent mail headers belonging to the character that match the query criteria. Queries can be filtered by label, and last_mail_id can be used to paginate backwards

<h3 id="getcharacterscharacteridmail-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|labels|query|array[integer]|false|none|
|last_mail_id|query|integer(int64)|false|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "from": 0,
    "is_read": true,
    "labels": [
      0
    ],
    "mail_id": 0,
    "recipients": [
      {
        "recipient_id": 0,
        "recipient_type": "alliance"
      }
    ],
    "subject": "string",
    "timestamp": "2019-08-24T14:15:22Z"
  }
]
```

<h3 id="getcharacterscharacteridmail-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CharactersCharacterIdMailGet](#schemacharacterscharacteridmailget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-mail.read_mail.v1 )
</aside>

## PostCharactersCharacterIdMail

<a id="opIdPostCharactersCharacterIdMail"></a>

`POST /characters/{character_id}/mail`

*Send a new mail*

Create and send a new mail

> Body parameter

```json
{
  "approved_cost": 0,
  "body": "string",
  "recipients": [
    {
      "recipient_id": 0,
      "recipient_type": "alliance"
    }
  ],
  "subject": "string"
}
```

<h3 id="postcharacterscharacteridmail-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|
|body|body|object|true|none|
|» approved_cost|body|integer(int64)|false|none|
|» body|body|string|true|none|
|» recipients|body|[object]|true|none|
|»» recipient_id|body|integer(int64)|true|none|
|»» recipient_type|body|string|true|none|
|» subject|body|string|true|none|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|
|»» recipient_type|alliance|
|»» recipient_type|character|
|»» recipient_type|corporation|
|»» recipient_type|mailing_list|

> Example responses

> 201 Response

```json
0
```

<h3 id="postcharacterscharacteridmail-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|[CharactersCharacterIdMailPost](#schemacharacterscharacteridmailpost)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|201|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|201|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|201|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-mail.send_mail.v1 )
</aside>

## GetCharactersCharacterIdMailLabels

<a id="opIdGetCharactersCharacterIdMailLabels"></a>

`GET /characters/{character_id}/mail/labels`

*Get mail labels and unread counts*

Return a list of the users mail labels, unread counts for each label and a total unread count.

<h3 id="getcharacterscharacteridmaillabels-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "labels": [
    {
      "color": "#0000fe",
      "label_id": 0,
      "name": "string",
      "unread_count": 0
    }
  ],
  "total_unread_count": 0
}
```

<h3 id="getcharacterscharacteridmaillabels-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CharactersCharacterIdMailLabelsGet](#schemacharacterscharacteridmaillabelsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-mail.read_mail.v1 )
</aside>

## PostCharactersCharacterIdMailLabels

<a id="opIdPostCharactersCharacterIdMailLabels"></a>

`POST /characters/{character_id}/mail/labels`

*Create a mail label*

Create a mail label

> Body parameter

```json
{
  "color": "#0000fe",
  "name": "string"
}
```

<h3 id="postcharacterscharacteridmaillabels-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|
|body|body|object|true|none|
|» color|body|string|false|Hexadecimal string representing label color, in RGB format|
|» name|body|string|true|none|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|
|» color|#0000fe|
|» color|#006634|
|» color|#0099ff|
|» color|#00ff33|
|» color|#01ffff|
|» color|#349800|
|» color|#660066|
|» color|#666666|
|» color|#999999|
|» color|#99ffff|
|» color|#9a0000|
|» color|#ccff9a|
|» color|#e6e6e6|
|» color|#fe0000|
|» color|#ff6600|
|» color|#ffff01|
|» color|#ffffcd|
|» color|#ffffff|

> Example responses

> 201 Response

```json
0
```

<h3 id="postcharacterscharacteridmaillabels-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|[CharactersCharacterIdMailLabelsPost](#schemacharacterscharacteridmaillabelspost)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|201|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|201|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|201|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-mail.organize_mail.v1 )
</aside>

## DeleteCharactersCharacterIdMailLabelsLabelId

<a id="opIdDeleteCharactersCharacterIdMailLabelsLabelId"></a>

`DELETE /characters/{character_id}/mail/labels/{label_id}`

*Delete a mail label*

Delete a mail label

<h3 id="deletecharacterscharacteridmaillabelslabelid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|label_id|path|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> default Response

```json
{
  "details": [
    {
      "location": "string",
      "message": "string",
      "value": null
    }
  ],
  "error": "string"
}
```

<h3 id="deletecharacterscharacteridmaillabelslabelid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|204|[No Content](https://tools.ietf.org/html/rfc7231#section-6.3.5)|Label deleted|None|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|204|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|204|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|204|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-mail.organize_mail.v1 )
</aside>

## GetCharactersCharacterIdMailLists

<a id="opIdGetCharactersCharacterIdMailLists"></a>

`GET /characters/{character_id}/mail/lists`

*Return mailing list subscriptions*

Return all mailing lists that the character is subscribed to

<h3 id="getcharacterscharacteridmaillists-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "mailing_list_id": 0,
    "name": "string"
  }
]
```

<h3 id="getcharacterscharacteridmaillists-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CharactersCharacterIdMailListsGet](#schemacharacterscharacteridmaillistsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-mail.read_mail.v1 )
</aside>

## DeleteCharactersCharacterIdMailMailId

<a id="opIdDeleteCharactersCharacterIdMailMailId"></a>

`DELETE /characters/{character_id}/mail/{mail_id}`

*Delete a mail*

Delete a mail

<h3 id="deletecharacterscharacteridmailmailid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|mail_id|path|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> default Response

```json
{
  "details": [
    {
      "location": "string",
      "message": "string",
      "value": null
    }
  ],
  "error": "string"
}
```

<h3 id="deletecharacterscharacteridmailmailid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|204|[No Content](https://tools.ietf.org/html/rfc7231#section-6.3.5)|Mail deleted|None|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|204|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|204|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|204|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-mail.organize_mail.v1 )
</aside>

## GetCharactersCharacterIdMailMailId

<a id="opIdGetCharactersCharacterIdMailMailId"></a>

`GET /characters/{character_id}/mail/{mail_id}`

*Return a mail*

Return the contents of an EVE mail

<h3 id="getcharacterscharacteridmailmailid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|mail_id|path|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "body": "string",
  "from": 0,
  "labels": [
    0
  ],
  "read": true,
  "recipients": [
    {
      "recipient_id": 0,
      "recipient_type": "alliance"
    }
  ],
  "subject": "string",
  "timestamp": "2019-08-24T14:15:22Z"
}
```

<h3 id="getcharacterscharacteridmailmailid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CharactersCharacterIdMailMailIdGet](#schemacharacterscharacteridmailmailidget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-mail.read_mail.v1 )
</aside>

## PutCharactersCharacterIdMailMailId

<a id="opIdPutCharactersCharacterIdMailMailId"></a>

`PUT /characters/{character_id}/mail/{mail_id}`

*Update metadata about a mail*

Update metadata about a mail

> Body parameter

```json
{
  "labels": [
    0
  ],
  "read": true
}
```

<h3 id="putcharacterscharacteridmailmailid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|mail_id|path|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|
|body|body|object|true|none|
|» labels|body|[integer]|false|Labels to assign to the mail. Pre-existing labels are unassigned.|
|» read|body|boolean|false|Whether the mail is flagged as read|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> default Response

```json
{
  "details": [
    {
      "location": "string",
      "message": "string",
      "value": null
    }
  ],
  "error": "string"
}
```

<h3 id="putcharacterscharacteridmailmailid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|204|[No Content](https://tools.ietf.org/html/rfc7231#section-6.3.5)|Mail updated|None|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|204|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|204|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|204|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-mail.organize_mail.v1 )
</aside>

<h1 id="eve-stable-infrastructure-esi-tranquility-market">Market</h1>

## GetCharactersCharacterIdOrders

<a id="opIdGetCharactersCharacterIdOrders"></a>

`GET /characters/{character_id}/orders`

*List open orders from a character*

List open market orders placed by a character

<h3 id="getcharacterscharacteridorders-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "duration": 0,
    "escrow": 0.1,
    "is_buy_order": true,
    "is_corporation": true,
    "issued": "2019-08-24T14:15:22Z",
    "location_id": 0,
    "min_volume": 0,
    "order_id": 0,
    "price": 0.1,
    "range": "1",
    "region_id": 0,
    "type_id": 0,
    "volume_remain": 0,
    "volume_total": 0
  }
]
```

<h3 id="getcharacterscharacteridorders-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CharactersCharacterIdOrdersGet](#schemacharacterscharacteridordersget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-markets.read_character_orders.v1 )
</aside>

## GetCharactersCharacterIdOrdersHistory

<a id="opIdGetCharactersCharacterIdOrdersHistory"></a>

`GET /characters/{character_id}/orders/history`

*List historical orders by a character*

List cancelled and expired market orders placed by a character up to 90 days in the past.

<h3 id="getcharacterscharacteridordershistory-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|page|query|integer(int32)|false|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "duration": 0,
    "escrow": 0.1,
    "is_buy_order": true,
    "is_corporation": true,
    "issued": "2019-08-24T14:15:22Z",
    "location_id": 0,
    "min_volume": 0,
    "order_id": 0,
    "price": 0.1,
    "range": "1",
    "region_id": 0,
    "state": "cancelled",
    "type_id": 0,
    "volume_remain": 0,
    "volume_total": 0
  }
]
```

<h3 id="getcharacterscharacteridordershistory-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CharactersCharacterIdOrdersHistoryGet](#schemacharacterscharacteridordershistoryget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|
|200|X-Pages|integer|int64|The total number of pages in the result set.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-markets.read_character_orders.v1 )
</aside>

## GetCorporationsCorporationIdOrders

<a id="opIdGetCorporationsCorporationIdOrders"></a>

`GET /corporations/{corporation_id}/orders`

*List open orders from a corporation*

List open market orders placed on behalf of a corporation

<h3 id="getcorporationscorporationidorders-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|corporation_id|path|[CorporationID](#schemacorporationid)|true|The ID of the corporation|
|page|query|integer(int32)|false|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "duration": 0,
    "escrow": 0.1,
    "is_buy_order": true,
    "issued": "2019-08-24T14:15:22Z",
    "issued_by": 0,
    "location_id": 0,
    "min_volume": 0,
    "order_id": 0,
    "price": 0.1,
    "range": "1",
    "region_id": 0,
    "type_id": 0,
    "volume_remain": 0,
    "volume_total": 0,
    "wallet_division": 0
  }
]
```

<h3 id="getcorporationscorporationidorders-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CorporationsCorporationIdOrdersGet](#schemacorporationscorporationidordersget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|
|200|X-Pages|integer|int64|The total number of pages in the result set.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-markets.read_corporation_orders.v1 )
</aside>

## GetCorporationsCorporationIdOrdersHistory

<a id="opIdGetCorporationsCorporationIdOrdersHistory"></a>

`GET /corporations/{corporation_id}/orders/history`

*List historical orders from a corporation*

List cancelled and expired market orders placed on behalf of a corporation up to 90 days in the past.

<h3 id="getcorporationscorporationidordershistory-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|corporation_id|path|[CorporationID](#schemacorporationid)|true|The ID of the corporation|
|page|query|integer(int32)|false|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "duration": 0,
    "escrow": 0.1,
    "is_buy_order": true,
    "issued": "2019-08-24T14:15:22Z",
    "issued_by": 0,
    "location_id": 0,
    "min_volume": 0,
    "order_id": 0,
    "price": 0.1,
    "range": "1",
    "region_id": 0,
    "state": "cancelled",
    "type_id": 0,
    "volume_remain": 0,
    "volume_total": 0,
    "wallet_division": 0
  }
]
```

<h3 id="getcorporationscorporationidordershistory-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CorporationsCorporationIdOrdersHistoryGet](#schemacorporationscorporationidordershistoryget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|
|200|X-Pages|integer|int64|The total number of pages in the result set.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-markets.read_corporation_orders.v1 )
</aside>

## GetMarketsGroups

<a id="opIdGetMarketsGroups"></a>

`GET /markets/groups`

*Get item groups*

Get a list of item groups

This route expires daily at 11:05

<h3 id="getmarketsgroups-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  0
]
```

<h3 id="getmarketsgroups-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[MarketsGroupsGet](#schemamarketsgroupsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetMarketsGroupsMarketGroupId

<a id="opIdGetMarketsGroupsMarketGroupId"></a>

`GET /markets/groups/{market_group_id}`

*Get item group information*

Get information on an item group

This route expires daily at 11:05

<h3 id="getmarketsgroupsmarketgroupid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|market_group_id|path|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "description": "string",
  "market_group_id": 0,
  "name": "string",
  "parent_group_id": 0,
  "types": [
    0
  ]
}
```

<h3 id="getmarketsgroupsmarketgroupid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[MarketsGroupsMarketGroupIdGet](#schemamarketsgroupsmarketgroupidget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|Content-Language|string||The language used in the response.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetMarketsPrices

<a id="opIdGetMarketsPrices"></a>

`GET /markets/prices`

*List market prices*

Return a list of prices

<h3 id="getmarketsprices-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "adjusted_price": 0.1,
    "average_price": 0.1,
    "type_id": 0
  }
]
```

<h3 id="getmarketsprices-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[MarketsPricesGet](#schemamarketspricesget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetMarketsStructuresStructureId

<a id="opIdGetMarketsStructuresStructureId"></a>

`GET /markets/structures/{structure_id}`

*List orders in a structure*

Return all orders in a structure

<h3 id="getmarketsstructuresstructureid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|page|query|integer(int32)|false|none|
|structure_id|path|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "duration": 0,
    "is_buy_order": true,
    "issued": "2019-08-24T14:15:22Z",
    "location_id": 0,
    "min_volume": 0,
    "order_id": 0,
    "price": 0.1,
    "range": "station",
    "type_id": 0,
    "volume_remain": 0,
    "volume_total": 0
  }
]
```

<h3 id="getmarketsstructuresstructureid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[MarketsStructuresStructureIdGet](#schemamarketsstructuresstructureidget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|
|200|X-Pages|integer|int64|The total number of pages in the result set.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-markets.structure_markets.v1 )
</aside>

## GetMarketsRegionIdHistory

<a id="opIdGetMarketsRegionIdHistory"></a>

`GET /markets/{region_id}/history`

*List historical market statistics in a region*

Return a list of historical market statistics for the specified type in a region

This route expires daily at 11:05

<h3 id="getmarketsregionidhistory-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|region_id|path|integer(int64)|true|none|
|type_id|query|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "average": 0.1,
    "date": "2019-08-24",
    "highest": 0.1,
    "lowest": 0.1,
    "order_count": 0,
    "volume": 0
  }
]
```

<h3 id="getmarketsregionidhistory-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[MarketsRegionIdHistoryGet](#schemamarketsregionidhistoryget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetMarketsRegionIdOrders

<a id="opIdGetMarketsRegionIdOrders"></a>

`GET /markets/{region_id}/orders`

*List orders in a region*

Return a list of orders in a region

<h3 id="getmarketsregionidorders-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|order_type|query|string|true|none|
|page|query|integer(int32)|false|none|
|region_id|path|integer(int64)|true|none|
|type_id|query|integer(int64)|false|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|order_type|buy|
|order_type|sell|
|order_type|all|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "duration": 0,
    "is_buy_order": true,
    "issued": "2019-08-24T14:15:22Z",
    "location_id": 0,
    "min_volume": 0,
    "order_id": 0,
    "price": 0.1,
    "range": "station",
    "system_id": 0,
    "type_id": 0,
    "volume_remain": 0,
    "volume_total": 0
  }
]
```

<h3 id="getmarketsregionidorders-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[MarketsRegionIdOrdersGet](#schemamarketsregionidordersget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|
|200|X-Pages|integer|int64|The total number of pages in the result set.|

<aside class="success">
This operation does not require authentication
</aside>

## GetMarketsRegionIdTypes

<a id="opIdGetMarketsRegionIdTypes"></a>

`GET /markets/{region_id}/types`

*List type IDs relevant to a market*

Return a list of type IDs that have active orders in the region, for efficient market indexing.

<h3 id="getmarketsregionidtypes-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|page|query|integer(int32)|false|none|
|region_id|path|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  0
]
```

<h3 id="getmarketsregionidtypes-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[MarketsRegionIdTypesGet](#schemamarketsregionidtypesget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|
|200|X-Pages|integer|int64|The total number of pages in the result set.|

<aside class="success">
This operation does not require authentication
</aside>

<h1 id="eve-stable-infrastructure-esi-tranquility-meta">Meta</h1>

## GetMetaChangelog

<a id="opIdGetMetaChangelog"></a>

`GET /meta/changelog`

*Get changelog*

Get the changelog of this API.

<h3 id="getmetachangelog-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "changelog": {
    "property1": [
      {
        "compatibility_date": "2025-08-26",
        "description": "Updated response schema.",
        "method": "GET",
        "path": "/meta/changelog",
        "type": "breaking"
      }
    ],
    "property2": [
      {
        "compatibility_date": "2025-08-26",
        "description": "Updated response schema.",
        "method": "GET",
        "path": "/meta/changelog",
        "type": "breaking"
      }
    ]
  }
}
```

<h3 id="getmetachangelog-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[MetaChangelog](#schemametachangelog)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|
|default|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|default|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|default|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetMetaCompatibilityDates

<a id="opIdGetMetaCompatibilityDates"></a>

`GET /meta/compatibility-dates`

*Get compatibility dates*

Get a list of compatibility dates.

<h3 id="getmetacompatibilitydates-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "compatibility_dates": [
    "2025-08-26"
  ]
}
```

<h3 id="getmetacompatibilitydates-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[MetaCompatibilityDates](#schemametacompatibilitydates)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|
|default|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|default|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|default|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetMetaStatus

<a id="opIdGetMetaStatus"></a>

`GET /meta/status`

*Get health status*

Get the health status of each API route.

<h3 id="getmetastatus-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "routes": [
    {
      "method": "GET",
      "path": "string",
      "status": "Unknown"
    }
  ]
}
```

<h3 id="getmetastatus-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[MetaStatus](#schemametastatus)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|
|default|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|default|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|default|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

<h1 id="eve-stable-infrastructure-esi-tranquility-planetary-interaction">Planetary Interaction</h1>

## GetCharactersCharacterIdPlanets

<a id="opIdGetCharactersCharacterIdPlanets"></a>

`GET /characters/{character_id}/planets`

*Get colonies*

Returns a list of all planetary colonies owned by a character.

<h3 id="getcharacterscharacteridplanets-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "last_update": "2019-08-24T14:15:22Z",
    "num_pins": 0,
    "owner_id": 0,
    "planet_id": 0,
    "planet_type": "temperate",
    "solar_system_id": 0,
    "upgrade_level": 0
  }
]
```

<h3 id="getcharacterscharacteridplanets-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CharactersCharacterIdPlanetsGet](#schemacharacterscharacteridplanetsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-planets.manage_planets.v1 )
</aside>

## GetCharactersCharacterIdPlanetsPlanetId

<a id="opIdGetCharactersCharacterIdPlanetsPlanetId"></a>

`GET /characters/{character_id}/planets/{planet_id}`

*Get colony layout*

Returns full details on the layout of a single planetary colony, including links, pins and routes. Note: Planetary information is only recalculated when the colony is viewed through the client. Information will not update until this criteria is met.

<h3 id="getcharacterscharacteridplanetsplanetid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|planet_id|path|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "links": [
    {
      "destination_pin_id": 0,
      "link_level": 0,
      "source_pin_id": 0
    }
  ],
  "pins": [
    {
      "contents": [
        {
          "amount": 0,
          "type_id": 0
        }
      ],
      "expiry_time": "2019-08-24T14:15:22Z",
      "extractor_details": {
        "cycle_time": 0,
        "head_radius": 0.1,
        "heads": [
          {
            "head_id": 0,
            "latitude": 0.1,
            "longitude": 0.1
          }
        ],
        "product_type_id": 0,
        "qty_per_cycle": 0
      },
      "factory_details": {
        "schematic_id": 0
      },
      "install_time": "2019-08-24T14:15:22Z",
      "last_cycle_start": "2019-08-24T14:15:22Z",
      "latitude": 0.1,
      "longitude": 0.1,
      "pin_id": 0,
      "schematic_id": 0,
      "type_id": 0
    }
  ],
  "routes": [
    {
      "content_type_id": 0,
      "destination_pin_id": 0,
      "quantity": 0.1,
      "route_id": 0,
      "source_pin_id": 0,
      "waypoints": [
        0
      ]
    }
  ]
}
```

<h3 id="getcharacterscharacteridplanetsplanetid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CharactersCharacterIdPlanetsPlanetIdGet](#schemacharacterscharacteridplanetsplanetidget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-planets.manage_planets.v1 )
</aside>

## GetCorporationsCorporationIdCustomsOffices

<a id="opIdGetCorporationsCorporationIdCustomsOffices"></a>

`GET /corporations/{corporation_id}/customs_offices`

*List corporation customs offices*

List customs offices owned by a corporation

<h3 id="getcorporationscorporationidcustomsoffices-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|corporation_id|path|[CorporationID](#schemacorporationid)|true|The ID of the corporation|
|page|query|integer(int32)|false|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "alliance_tax_rate": 0.1,
    "allow_access_with_standings": true,
    "allow_alliance_access": true,
    "bad_standing_tax_rate": 0.1,
    "corporation_tax_rate": 0.1,
    "excellent_standing_tax_rate": 0.1,
    "good_standing_tax_rate": 0.1,
    "neutral_standing_tax_rate": 0.1,
    "office_id": 0,
    "reinforce_exit_end": 0,
    "reinforce_exit_start": 0,
    "standing_level": "bad",
    "system_id": 0,
    "terrible_standing_tax_rate": 0.1
  }
]
```

<h3 id="getcorporationscorporationidcustomsoffices-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CorporationsCorporationIdCustomsOfficesGet](#schemacorporationscorporationidcustomsofficesget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|
|200|X-Pages|integer|int64|The total number of pages in the result set.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-planets.read_customs_offices.v1 )
</aside>

## GetUniverseSchematicsSchematicId

<a id="opIdGetUniverseSchematicsSchematicId"></a>

`GET /universe/schematics/{schematic_id}`

*Get schematic information*

Get information on a planetary factory schematic

<h3 id="getuniverseschematicsschematicid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|schematic_id|path|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "cycle_time": 0,
  "schematic_name": "string"
}
```

<h3 id="getuniverseschematicsschematicid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[UniverseSchematicsSchematicIdGet](#schemauniverseschematicsschematicidget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

<h1 id="eve-stable-infrastructure-esi-tranquility-routes">Routes</h1>

## PostRoute

<a id="opIdPostRoute"></a>

`POST /route/{origin_system_id}/{destination_system_id}`

*Get route between two systems*

Calculate the systems between the given origin and destination.

> Body parameter

```json
{
  "avoid_systems": [
    30000001
  ],
  "connections": [
    {
      "from": 30000001,
      "to": 30000001
    }
  ],
  "preference": "Shorter",
  "security_penalty": 50
}
```

<h3 id="postroute-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|origin_system_id|path|[SolarSystemID](#schemasolarsystemid)|true|Origin system|
|destination_system_id|path|[SolarSystemID](#schemasolarsystemid)|true|Destination system|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|
|body|body|[RouteRequestBody](#schemarouterequestbody)|true|none|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "route": [
    30000001
  ]
}
```

<h3 id="postroute-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Route](#schemaroute)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|
|default|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|default|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|default|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

<h1 id="eve-stable-infrastructure-esi-tranquility-search">Search</h1>

## GetCharactersCharacterIdSearch

<a id="opIdGetCharactersCharacterIdSearch"></a>

`GET /characters/{character_id}/search`

*Search on a string*

Search for entities that match a given sub-string.

<h3 id="getcharacterscharacteridsearch-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|categories|query|array[string]|true|none|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|search|query|string|true|none|
|strict|query|boolean|false|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|categories|agent|
|categories|alliance|
|categories|character|
|categories|constellation|
|categories|corporation|
|categories|faction|
|categories|inventory_type|
|categories|region|
|categories|solar_system|
|categories|station|
|categories|structure|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "agent": [
    0
  ],
  "alliance": [
    0
  ],
  "character": [
    0
  ],
  "constellation": [
    0
  ],
  "corporation": [
    0
  ],
  "faction": [
    0
  ],
  "inventory_type": [
    0
  ],
  "region": [
    0
  ],
  "solar_system": [
    0
  ],
  "station": [
    0
  ],
  "structure": [
    0
  ]
}
```

<h3 id="getcharacterscharacteridsearch-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CharactersCharacterIdSearchGet](#schemacharacterscharacteridsearchget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|Content-Language|string||The language used in the response.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-search.search_structures.v1 )
</aside>

<h1 id="eve-stable-infrastructure-esi-tranquility-skills">Skills</h1>

## GetCharactersCharacterIdAttributes

<a id="opIdGetCharactersCharacterIdAttributes"></a>

`GET /characters/{character_id}/attributes`

*Get character attributes*

Return attributes of a character

<h3 id="getcharacterscharacteridattributes-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "accrued_remap_cooldown_date": "2019-08-24T14:15:22Z",
  "bonus_remaps": 0,
  "charisma": 0,
  "intelligence": 0,
  "last_remap_date": "2019-08-24T14:15:22Z",
  "memory": 0,
  "perception": 0,
  "willpower": 0
}
```

<h3 id="getcharacterscharacteridattributes-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CharactersCharacterIdAttributesGet](#schemacharacterscharacteridattributesget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-skills.read_skills.v1 )
</aside>

## GetCharactersCharacterIdSkillqueue

<a id="opIdGetCharactersCharacterIdSkillqueue"></a>

`GET /characters/{character_id}/skillqueue`

*Get character's skill queue*

List the configured skill queue for the given character

<h3 id="getcharacterscharacteridskillqueue-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "finish_date": "2019-08-24T14:15:22Z",
    "finished_level": 0,
    "level_end_sp": 0,
    "level_start_sp": 0,
    "queue_position": 0,
    "skill_id": 0,
    "start_date": "2019-08-24T14:15:22Z",
    "training_start_sp": 0
  }
]
```

<h3 id="getcharacterscharacteridskillqueue-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CharactersCharacterIdSkillqueueGet](#schemacharacterscharacteridskillqueueget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-skills.read_skillqueue.v1 )
</aside>

## GetCharactersCharacterIdSkills

<a id="opIdGetCharactersCharacterIdSkills"></a>

`GET /characters/{character_id}/skills`

*Get character skills*

List all trained skills for the given character

<h3 id="getcharacterscharacteridskills-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "skills": [
    {
      "active_skill_level": 0,
      "skill_id": 0,
      "skillpoints_in_skill": 0,
      "trained_skill_level": 0
    }
  ],
  "total_sp": 0,
  "unallocated_sp": 0
}
```

<h3 id="getcharacterscharacteridskills-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CharactersCharacterIdSkillsGet](#schemacharacterscharacteridskillsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-skills.read_skills.v1 )
</aside>

<h1 id="eve-stable-infrastructure-esi-tranquility-sovereignty">Sovereignty</h1>

## GetSovereigntyCampaigns

<a id="opIdGetSovereigntyCampaigns"></a>

`GET /sovereignty/campaigns`

*List sovereignty campaigns*

Shows sovereignty data for campaigns.

<h3 id="getsovereigntycampaigns-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "attackers_score": 0.1,
    "campaign_id": 0,
    "constellation_id": 0,
    "defender_id": 0,
    "defender_score": 0.1,
    "event_type": "tcu_defense",
    "participants": [
      {
        "alliance_id": 0,
        "score": 0.1
      }
    ],
    "solar_system_id": 0,
    "start_time": "2019-08-24T14:15:22Z",
    "structure_id": 0
  }
]
```

<h3 id="getsovereigntycampaigns-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[SovereigntyCampaignsGet](#schemasovereigntycampaignsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetSovereigntyMap

<a id="opIdGetSovereigntyMap"></a>

`GET /sovereignty/map`

*List sovereignty of systems*

Shows sovereignty information for solar systems

<h3 id="getsovereigntymap-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "alliance_id": 0,
    "corporation_id": 0,
    "faction_id": 0,
    "system_id": 0
  }
]
```

<h3 id="getsovereigntymap-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[SovereigntyMapGet](#schemasovereigntymapget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetSovereigntyStructures

<a id="opIdGetSovereigntyStructures"></a>

`GET /sovereignty/structures`

*List sovereignty structures*

Shows sovereignty data for structures.

<h3 id="getsovereigntystructures-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "alliance_id": 0,
    "solar_system_id": 0,
    "structure_id": 0,
    "structure_type_id": 0,
    "vulnerability_occupancy_level": 0.1,
    "vulnerable_end_time": "2019-08-24T14:15:22Z",
    "vulnerable_start_time": "2019-08-24T14:15:22Z"
  }
]
```

<h3 id="getsovereigntystructures-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[SovereigntyStructuresGet](#schemasovereigntystructuresget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

<h1 id="eve-stable-infrastructure-esi-tranquility-status">Status</h1>

## GetStatus

<a id="opIdGetStatus"></a>

`GET /status`

*Retrieve the uptime and player counts*

EVE Server status

<h3 id="getstatus-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "players": 0,
  "server_version": "string",
  "start_time": "2019-08-24T14:15:22Z",
  "vip": true
}
```

<h3 id="getstatus-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[StatusGet](#schemastatusget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

<h1 id="eve-stable-infrastructure-esi-tranquility-universe">Universe</h1>

## GetUniverseAncestries

<a id="opIdGetUniverseAncestries"></a>

`GET /universe/ancestries`

*Get ancestries*

Get all character ancestries

This route expires daily at 11:05

<h3 id="getuniverseancestries-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "bloodline_id": 0,
    "description": "string",
    "icon_id": 0,
    "id": 0,
    "name": "string",
    "short_description": "string"
  }
]
```

<h3 id="getuniverseancestries-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[UniverseAncestriesGet](#schemauniverseancestriesget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|Content-Language|string||The language used in the response.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetUniverseAsteroidBeltsAsteroidBeltId

<a id="opIdGetUniverseAsteroidBeltsAsteroidBeltId"></a>

`GET /universe/asteroid_belts/{asteroid_belt_id}`

*Get asteroid belt information*

Get information on an asteroid belt

This route expires daily at 11:05

<h3 id="getuniverseasteroidbeltsasteroidbeltid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|asteroid_belt_id|path|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "name": "string",
  "position": {
    "x": 0.1,
    "y": 0.1,
    "z": 0.1
  },
  "system_id": 0
}
```

<h3 id="getuniverseasteroidbeltsasteroidbeltid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[UniverseAsteroidBeltsAsteroidBeltIdGet](#schemauniverseasteroidbeltsasteroidbeltidget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetUniverseBloodlines

<a id="opIdGetUniverseBloodlines"></a>

`GET /universe/bloodlines`

*Get bloodlines*

Get a list of bloodlines

This route expires daily at 11:05

<h3 id="getuniversebloodlines-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "bloodline_id": 0,
    "charisma": 0,
    "corporation_id": 0,
    "description": "string",
    "intelligence": 0,
    "memory": 0,
    "name": "string",
    "perception": 0,
    "race_id": 0,
    "ship_type_id": 0,
    "willpower": 0
  }
]
```

<h3 id="getuniversebloodlines-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[UniverseBloodlinesGet](#schemauniversebloodlinesget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|Content-Language|string||The language used in the response.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetUniverseCategories

<a id="opIdGetUniverseCategories"></a>

`GET /universe/categories`

*Get item categories*

Get a list of item categories

This route expires daily at 11:05

<h3 id="getuniversecategories-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  0
]
```

<h3 id="getuniversecategories-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[UniverseCategoriesGet](#schemauniversecategoriesget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetUniverseCategoriesCategoryId

<a id="opIdGetUniverseCategoriesCategoryId"></a>

`GET /universe/categories/{category_id}`

*Get item category information*

Get information of an item category

This route expires daily at 11:05

<h3 id="getuniversecategoriescategoryid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|category_id|path|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "category_id": 0,
  "groups": [
    0
  ],
  "name": "string",
  "published": true
}
```

<h3 id="getuniversecategoriescategoryid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[UniverseCategoriesCategoryIdGet](#schemauniversecategoriescategoryidget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|Content-Language|string||The language used in the response.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetUniverseConstellations

<a id="opIdGetUniverseConstellations"></a>

`GET /universe/constellations`

*Get constellations*

Get a list of constellations

This route expires daily at 11:05

<h3 id="getuniverseconstellations-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  0
]
```

<h3 id="getuniverseconstellations-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[UniverseConstellationsGet](#schemauniverseconstellationsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetUniverseConstellationsConstellationId

<a id="opIdGetUniverseConstellationsConstellationId"></a>

`GET /universe/constellations/{constellation_id}`

*Get constellation information*

Get information on a constellation

This route expires daily at 11:05

<h3 id="getuniverseconstellationsconstellationid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|constellation_id|path|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "constellation_id": 0,
  "name": "string",
  "position": {
    "x": 0.1,
    "y": 0.1,
    "z": 0.1
  },
  "region_id": 0,
  "systems": [
    0
  ]
}
```

<h3 id="getuniverseconstellationsconstellationid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[UniverseConstellationsConstellationIdGet](#schemauniverseconstellationsconstellationidget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|Content-Language|string||The language used in the response.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetUniverseFactions

<a id="opIdGetUniverseFactions"></a>

`GET /universe/factions`

*Get factions*

Get a list of factions

This route expires daily at 11:05

<h3 id="getuniversefactions-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "corporation_id": 0,
    "description": "string",
    "faction_id": 0,
    "is_unique": true,
    "militia_corporation_id": 0,
    "name": "string",
    "size_factor": 0.1,
    "solar_system_id": 0,
    "station_count": 0,
    "station_system_count": 0
  }
]
```

<h3 id="getuniversefactions-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[UniverseFactionsGet](#schemauniversefactionsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|Content-Language|string||The language used in the response.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetUniverseGraphics

<a id="opIdGetUniverseGraphics"></a>

`GET /universe/graphics`

*Get graphics*

Get a list of graphics

This route expires daily at 11:05

<h3 id="getuniversegraphics-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  0
]
```

<h3 id="getuniversegraphics-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[UniverseGraphicsGet](#schemauniversegraphicsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetUniverseGraphicsGraphicId

<a id="opIdGetUniverseGraphicsGraphicId"></a>

`GET /universe/graphics/{graphic_id}`

*Get graphic information*

Get information on a graphic

This route expires daily at 11:05

<h3 id="getuniversegraphicsgraphicid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|graphic_id|path|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "collision_file": "string",
  "graphic_file": "string",
  "graphic_id": 0,
  "icon_folder": "string",
  "sof_dna": "string",
  "sof_fation_name": "string",
  "sof_hull_name": "string",
  "sof_race_name": "string"
}
```

<h3 id="getuniversegraphicsgraphicid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[UniverseGraphicsGraphicIdGet](#schemauniversegraphicsgraphicidget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetUniverseGroups

<a id="opIdGetUniverseGroups"></a>

`GET /universe/groups`

*Get item groups*

Get a list of item groups

This route expires daily at 11:05

<h3 id="getuniversegroups-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|page|query|integer(int32)|false|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  0
]
```

<h3 id="getuniversegroups-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[UniverseGroupsGet](#schemauniversegroupsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|
|200|X-Pages|integer|int64|The total number of pages in the result set.|

<aside class="success">
This operation does not require authentication
</aside>

## GetUniverseGroupsGroupId

<a id="opIdGetUniverseGroupsGroupId"></a>

`GET /universe/groups/{group_id}`

*Get item group information*

Get information on an item group

This route expires daily at 11:05

<h3 id="getuniversegroupsgroupid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|group_id|path|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "category_id": 0,
  "group_id": 0,
  "name": "string",
  "published": true,
  "types": [
    0
  ]
}
```

<h3 id="getuniversegroupsgroupid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[UniverseGroupsGroupIdGet](#schemauniversegroupsgroupidget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|Content-Language|string||The language used in the response.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## PostUniverseIds

<a id="opIdPostUniverseIds"></a>

`POST /universe/ids`

*Bulk names to IDs*

Resolve a set of names to IDs in the following categories: agents, alliances, characters, constellations, corporations factions, inventory_types, regions, stations, and systems. Only exact matches will be returned. All names searched for are cached for 12 hours

> Body parameter

```json
[
  "string"
]
```

<h3 id="postuniverseids-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|
|body|body|array[string]|true|none|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "agents": [
    {
      "id": 0,
      "name": "string"
    }
  ],
  "alliances": [
    {
      "id": 0,
      "name": "string"
    }
  ],
  "characters": [
    {
      "id": 0,
      "name": "string"
    }
  ],
  "constellations": [
    {
      "id": 0,
      "name": "string"
    }
  ],
  "corporations": [
    {
      "id": 0,
      "name": "string"
    }
  ],
  "factions": [
    {
      "id": 0,
      "name": "string"
    }
  ],
  "inventory_types": [
    {
      "id": 0,
      "name": "string"
    }
  ],
  "regions": [
    {
      "id": 0,
      "name": "string"
    }
  ],
  "stations": [
    {
      "id": 0,
      "name": "string"
    }
  ],
  "systems": [
    {
      "id": 0,
      "name": "string"
    }
  ]
}
```

<h3 id="postuniverseids-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[UniverseIdsPost](#schemauniverseidspost)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|Content-Language|string||The language used in the response.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetUniverseMoonsMoonId

<a id="opIdGetUniverseMoonsMoonId"></a>

`GET /universe/moons/{moon_id}`

*Get moon information*

Get information on a moon

This route expires daily at 11:05

<h3 id="getuniversemoonsmoonid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|moon_id|path|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "moon_id": 0,
  "name": "string",
  "position": {
    "x": 0.1,
    "y": 0.1,
    "z": 0.1
  },
  "system_id": 0
}
```

<h3 id="getuniversemoonsmoonid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[UniverseMoonsMoonIdGet](#schemauniversemoonsmoonidget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## PostUniverseNames

<a id="opIdPostUniverseNames"></a>

`POST /universe/names`

*Get names and categories for a set of IDs*

Resolve a set of IDs to names and categories. Supported ID's for resolving are: Characters, Corporations, Alliances, Stations, Solar Systems, Constellations, Regions, Types, Factions

> Body parameter

```json
[
  0
]
```

<h3 id="postuniversenames-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|
|body|body|array[integer]|true|none|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "category": "alliance",
    "id": 0,
    "name": "string"
  }
]
```

<h3 id="postuniversenames-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[UniverseNamesPost](#schemauniversenamespost)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetUniversePlanetsPlanetId

<a id="opIdGetUniversePlanetsPlanetId"></a>

`GET /universe/planets/{planet_id}`

*Get planet information*

Get information on a planet

This route expires daily at 11:05

<h3 id="getuniverseplanetsplanetid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|planet_id|path|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "name": "string",
  "planet_id": 0,
  "position": {
    "x": 0.1,
    "y": 0.1,
    "z": 0.1
  },
  "system_id": 0,
  "type_id": 0
}
```

<h3 id="getuniverseplanetsplanetid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[UniversePlanetsPlanetIdGet](#schemauniverseplanetsplanetidget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetUniverseRaces

<a id="opIdGetUniverseRaces"></a>

`GET /universe/races`

*Get character races*

Get a list of character races

This route expires daily at 11:05

<h3 id="getuniverseraces-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "alliance_id": 0,
    "description": "string",
    "name": "string",
    "race_id": 0
  }
]
```

<h3 id="getuniverseraces-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[UniverseRacesGet](#schemauniverseracesget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|Content-Language|string||The language used in the response.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetUniverseRegions

<a id="opIdGetUniverseRegions"></a>

`GET /universe/regions`

*Get regions*

Get a list of regions

This route expires daily at 11:05

<h3 id="getuniverseregions-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  0
]
```

<h3 id="getuniverseregions-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[UniverseRegionsGet](#schemauniverseregionsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetUniverseRegionsRegionId

<a id="opIdGetUniverseRegionsRegionId"></a>

`GET /universe/regions/{region_id}`

*Get region information*

Get information on a region

This route expires daily at 11:05

<h3 id="getuniverseregionsregionid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|region_id|path|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "constellations": [
    0
  ],
  "description": "string",
  "name": "string",
  "region_id": 0
}
```

<h3 id="getuniverseregionsregionid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[UniverseRegionsRegionIdGet](#schemauniverseregionsregionidget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|Content-Language|string||The language used in the response.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetUniverseStargatesStargateId

<a id="opIdGetUniverseStargatesStargateId"></a>

`GET /universe/stargates/{stargate_id}`

*Get stargate information*

Get information on a stargate

This route expires daily at 11:05

<h3 id="getuniversestargatesstargateid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|stargate_id|path|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "destination": {
    "stargate_id": 0,
    "system_id": 0
  },
  "name": "string",
  "position": {
    "x": 0.1,
    "y": 0.1,
    "z": 0.1
  },
  "stargate_id": 0,
  "system_id": 0,
  "type_id": 0
}
```

<h3 id="getuniversestargatesstargateid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[UniverseStargatesStargateIdGet](#schemauniversestargatesstargateidget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetUniverseStarsStarId

<a id="opIdGetUniverseStarsStarId"></a>

`GET /universe/stars/{star_id}`

*Get star information*

Get information on a star

This route expires daily at 11:05

<h3 id="getuniversestarsstarid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|star_id|path|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "age": 0,
  "luminosity": 0.1,
  "name": "string",
  "radius": 0,
  "solar_system_id": 0,
  "spectral_class": "K2 V",
  "temperature": 0,
  "type_id": 0
}
```

<h3 id="getuniversestarsstarid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[UniverseStarsStarIdGet](#schemauniversestarsstaridget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetUniverseStationsStationId

<a id="opIdGetUniverseStationsStationId"></a>

`GET /universe/stations/{station_id}`

*Get station information*

Get information on a station

This route expires daily at 11:05

<h3 id="getuniversestationsstationid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|station_id|path|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "max_dockable_ship_volume": 0.1,
  "name": "string",
  "office_rental_cost": 0.1,
  "owner": 0,
  "position": {
    "x": 0.1,
    "y": 0.1,
    "z": 0.1
  },
  "race_id": 0,
  "reprocessing_efficiency": 0.1,
  "reprocessing_stations_take": 0.1,
  "services": [
    "bounty-missions"
  ],
  "station_id": 0,
  "system_id": 0,
  "type_id": 0
}
```

<h3 id="getuniversestationsstationid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[UniverseStationsStationIdGet](#schemauniversestationsstationidget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetUniverseStructures

<a id="opIdGetUniverseStructures"></a>

`GET /universe/structures`

*List all public structures*

List all public structures

<h3 id="getuniversestructures-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|filter|query|string|false|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|filter|market|
|filter|manufacturing_basic|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  0
]
```

<h3 id="getuniversestructures-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[UniverseStructuresGet](#schemauniversestructuresget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetUniverseStructuresStructureId

<a id="opIdGetUniverseStructuresStructureId"></a>

`GET /universe/structures/{structure_id}`

*Get structure information*

Returns information on requested structure if you are on the ACL. Otherwise, returns "Forbidden" for all inputs.

<h3 id="getuniversestructuresstructureid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|structure_id|path|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "name": "string",
  "owner_id": 0,
  "position": {
    "x": 0.1,
    "y": 0.1,
    "z": 0.1
  },
  "solar_system_id": 0,
  "type_id": 0
}
```

<h3 id="getuniversestructuresstructureid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[UniverseStructuresStructureIdGet](#schemauniversestructuresstructureidget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-universe.read_structures.v1 )
</aside>

## GetUniverseSystemJumps

<a id="opIdGetUniverseSystemJumps"></a>

`GET /universe/system_jumps`

*Get system jumps*

Get the number of jumps in solar systems within the last hour ending at the timestamp of the Last-Modified header, excluding wormhole space. Only systems with jumps will be listed

<h3 id="getuniversesystemjumps-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "ship_jumps": 0,
    "system_id": 0
  }
]
```

<h3 id="getuniversesystemjumps-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[UniverseSystemJumpsGet](#schemauniversesystemjumpsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetUniverseSystemKills

<a id="opIdGetUniverseSystemKills"></a>

`GET /universe/system_kills`

*Get system kills*

Get the number of ship, pod and NPC kills per solar system within the last hour ending at the timestamp of the Last-Modified header, excluding wormhole space. Only systems with kills will be listed

<h3 id="getuniversesystemkills-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "npc_kills": 0,
    "pod_kills": 0,
    "ship_kills": 0,
    "system_id": 0
  }
]
```

<h3 id="getuniversesystemkills-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[UniverseSystemKillsGet](#schemauniversesystemkillsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetUniverseSystems

<a id="opIdGetUniverseSystems"></a>

`GET /universe/systems`

*Get solar systems*

Get a list of solar systems

This route expires daily at 11:05

<h3 id="getuniversesystems-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  0
]
```

<h3 id="getuniversesystems-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[UniverseSystemsGet](#schemauniversesystemsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetUniverseSystemsSystemId

<a id="opIdGetUniverseSystemsSystemId"></a>

`GET /universe/systems/{system_id}`

*Get solar system information*

Get information on a solar system.

This route expires daily at 11:05

<h3 id="getuniversesystemssystemid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|system_id|path|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "constellation_id": 0,
  "name": "string",
  "planets": [
    {
      "asteroid_belts": [
        0
      ],
      "moons": [
        0
      ],
      "planet_id": 0
    }
  ],
  "position": {
    "x": 0.1,
    "y": 0.1,
    "z": 0.1
  },
  "security_class": "string",
  "security_status": 0.1,
  "star_id": 0,
  "stargates": [
    0
  ],
  "stations": [
    0
  ],
  "system_id": 0
}
```

<h3 id="getuniversesystemssystemid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[UniverseSystemsSystemIdGet](#schemauniversesystemssystemidget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|Content-Language|string||The language used in the response.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetUniverseTypes

<a id="opIdGetUniverseTypes"></a>

`GET /universe/types`

*Get types*

Get a list of type ids

This route expires daily at 11:05

<h3 id="getuniversetypes-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|page|query|integer(int32)|false|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  0
]
```

<h3 id="getuniversetypes-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[UniverseTypesGet](#schemauniversetypesget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|
|200|X-Pages|integer|int64|The total number of pages in the result set.|

<aside class="success">
This operation does not require authentication
</aside>

## GetUniverseTypesTypeId

<a id="opIdGetUniverseTypesTypeId"></a>

`GET /universe/types/{type_id}`

*Get type information*

Get information on a type

This route expires daily at 11:05

<h3 id="getuniversetypestypeid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|type_id|path|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "capacity": 0.1,
  "description": "string",
  "dogma_attributes": [
    {
      "attribute_id": 0,
      "value": 0.1
    }
  ],
  "dogma_effects": [
    {
      "effect_id": 0,
      "is_default": true
    }
  ],
  "graphic_id": 0,
  "group_id": 0,
  "icon_id": 0,
  "market_group_id": 0,
  "mass": 0.1,
  "name": "string",
  "packaged_volume": 0.1,
  "portion_size": 0,
  "published": true,
  "radius": 0.1,
  "type_id": 0,
  "volume": 0.1
}
```

<h3 id="getuniversetypestypeid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[UniverseTypesTypeIdGet](#schemauniversetypestypeidget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|Content-Language|string||The language used in the response.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

<h1 id="eve-stable-infrastructure-esi-tranquility-user-interface">User Interface</h1>

## PostUiAutopilotWaypoint

<a id="opIdPostUiAutopilotWaypoint"></a>

`POST /ui/autopilot/waypoint`

*Set Autopilot Waypoint*

Set a solar system as autopilot waypoint

<h3 id="postuiautopilotwaypoint-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|add_to_beginning|query|boolean|true|none|
|clear_other_waypoints|query|boolean|true|none|
|destination_id|query|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> default Response

```json
{
  "details": [
    {
      "location": "string",
      "message": "string",
      "value": null
    }
  ],
  "error": "string"
}
```

<h3 id="postuiautopilotwaypoint-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|204|[No Content](https://tools.ietf.org/html/rfc7231#section-6.3.5)|Open window request received|None|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|204|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|204|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|204|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-ui.write_waypoint.v1 )
</aside>

## PostUiOpenwindowContract

<a id="opIdPostUiOpenwindowContract"></a>

`POST /ui/openwindow/contract`

*Open Contract Window*

Open the contract window inside the client

<h3 id="postuiopenwindowcontract-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|contract_id|query|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> default Response

```json
{
  "details": [
    {
      "location": "string",
      "message": "string",
      "value": null
    }
  ],
  "error": "string"
}
```

<h3 id="postuiopenwindowcontract-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|204|[No Content](https://tools.ietf.org/html/rfc7231#section-6.3.5)|Open window request received|None|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|204|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|204|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|204|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-ui.open_window.v1 )
</aside>

## PostUiOpenwindowInformation

<a id="opIdPostUiOpenwindowInformation"></a>

`POST /ui/openwindow/information`

*Open Information Window*

Open the information window for a character, corporation or alliance inside the client

<h3 id="postuiopenwindowinformation-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|target_id|query|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> default Response

```json
{
  "details": [
    {
      "location": "string",
      "message": "string",
      "value": null
    }
  ],
  "error": "string"
}
```

<h3 id="postuiopenwindowinformation-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|204|[No Content](https://tools.ietf.org/html/rfc7231#section-6.3.5)|Open window request received|None|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|204|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|204|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|204|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-ui.open_window.v1 )
</aside>

## PostUiOpenwindowMarketdetails

<a id="opIdPostUiOpenwindowMarketdetails"></a>

`POST /ui/openwindow/marketdetails`

*Open Market Details*

Open the market details window for a specific typeID inside the client

<h3 id="postuiopenwindowmarketdetails-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|type_id|query|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> default Response

```json
{
  "details": [
    {
      "location": "string",
      "message": "string",
      "value": null
    }
  ],
  "error": "string"
}
```

<h3 id="postuiopenwindowmarketdetails-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|204|[No Content](https://tools.ietf.org/html/rfc7231#section-6.3.5)|Open window request received|None|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|204|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|204|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|204|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-ui.open_window.v1 )
</aside>

## PostUiOpenwindowNewmail

<a id="opIdPostUiOpenwindowNewmail"></a>

`POST /ui/openwindow/newmail`

*Open New Mail Window*

Open the New Mail window, according to settings from the request if applicable

> Body parameter

```json
{
  "body": "string",
  "recipients": [
    0
  ],
  "subject": "string",
  "to_corp_or_alliance_id": 0,
  "to_mailing_list_id": 0
}
```

<h3 id="postuiopenwindownewmail-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|
|body|body|object|true|none|
|» body|body|string|true|none|
|» recipients|body|[integer]|true|none|
|» subject|body|string|true|none|
|» to_corp_or_alliance_id|body|integer(int64)|false|none|
|» to_mailing_list_id|body|integer(int64)|false|Corporations, alliances and mailing lists are all types of mailing groups. You may only send to one mailing group, at a time, so you may fill out either this field or the to_corp_or_alliance_ids field|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> default Response

```json
{
  "details": [
    {
      "location": "string",
      "message": "string",
      "value": null
    }
  ],
  "error": "string"
}
```

<h3 id="postuiopenwindownewmail-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|204|[No Content](https://tools.ietf.org/html/rfc7231#section-6.3.5)|Open window request received|None|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|204|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|204|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|204|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-ui.open_window.v1 )
</aside>

<h1 id="eve-stable-infrastructure-esi-tranquility-wallet">Wallet</h1>

## GetCharactersCharacterIdWallet

<a id="opIdGetCharactersCharacterIdWallet"></a>

`GET /characters/{character_id}/wallet`

*Get a character's wallet balance*

Returns a character's wallet balance

<h3 id="getcharacterscharacteridwallet-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
0.1
```

<h3 id="getcharacterscharacteridwallet-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CharactersCharacterIdWalletGet](#schemacharacterscharacteridwalletget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-wallet.read_character_wallet.v1 )
</aside>

## GetCharactersCharacterIdWalletJournal

<a id="opIdGetCharactersCharacterIdWalletJournal"></a>

`GET /characters/{character_id}/wallet/journal`

*Get character wallet journal*

Retrieve the given character's wallet journal going 30 days back

<h3 id="getcharacterscharacteridwalletjournal-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|page|query|integer(int32)|false|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "amount": 0.1,
    "balance": 0.1,
    "context_id": 0,
    "context_id_type": "structure_id",
    "date": "2019-08-24T14:15:22Z",
    "description": "string",
    "first_party_id": 0,
    "id": 0,
    "reason": "string",
    "ref_type": "acceleration_gate_fee",
    "second_party_id": 0,
    "tax": 0.1,
    "tax_receiver_id": 0
  }
]
```

<h3 id="getcharacterscharacteridwalletjournal-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CharactersCharacterIdWalletJournalGet](#schemacharacterscharacteridwalletjournalget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|
|200|X-Pages|integer|int64|The total number of pages in the result set.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-wallet.read_character_wallet.v1 )
</aside>

## GetCharactersCharacterIdWalletTransactions

<a id="opIdGetCharactersCharacterIdWalletTransactions"></a>

`GET /characters/{character_id}/wallet/transactions`

*Get wallet transactions*

Get wallet transactions of a character

<h3 id="getcharacterscharacteridwallettransactions-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|character_id|path|[CharacterID](#schemacharacterid)|true|The ID of the character|
|from_id|query|integer(int64)|false|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "client_id": 0,
    "date": "2019-08-24T14:15:22Z",
    "is_buy": true,
    "is_personal": true,
    "journal_ref_id": 0,
    "location_id": 0,
    "quantity": 0,
    "transaction_id": 0,
    "type_id": 0,
    "unit_price": 0.1
  }
]
```

<h3 id="getcharacterscharacteridwallettransactions-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CharactersCharacterIdWalletTransactionsGet](#schemacharacterscharacteridwallettransactionsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-wallet.read_character_wallet.v1 )
</aside>

## GetCorporationsCorporationIdWallets

<a id="opIdGetCorporationsCorporationIdWallets"></a>

`GET /corporations/{corporation_id}/wallets`

*Returns a corporation's wallet balance*

Get a corporation's wallets

<h3 id="getcorporationscorporationidwallets-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|corporation_id|path|[CorporationID](#schemacorporationid)|true|The ID of the corporation|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "balance": 0.1,
    "division": 0
  }
]
```

<h3 id="getcorporationscorporationidwallets-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CorporationsCorporationIdWalletsGet](#schemacorporationscorporationidwalletsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-wallet.read_corporation_wallets.v1 )
</aside>

## GetCorporationsCorporationIdWalletsDivisionJournal

<a id="opIdGetCorporationsCorporationIdWalletsDivisionJournal"></a>

`GET /corporations/{corporation_id}/wallets/{division}/journal`

*Get corporation wallet journal*

Retrieve the given corporation's wallet journal for the given division going 30 days back

<h3 id="getcorporationscorporationidwalletsdivisionjournal-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|corporation_id|path|[CorporationID](#schemacorporationid)|true|The ID of the corporation|
|division|path|integer(int64)|true|none|
|page|query|integer(int32)|false|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "amount": 0.1,
    "balance": 0.1,
    "context_id": 0,
    "context_id_type": "structure_id",
    "date": "2019-08-24T14:15:22Z",
    "description": "string",
    "first_party_id": 0,
    "id": 0,
    "reason": "string",
    "ref_type": "acceleration_gate_fee",
    "second_party_id": 0,
    "tax": 0.1,
    "tax_receiver_id": 0
  }
]
```

<h3 id="getcorporationscorporationidwalletsdivisionjournal-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CorporationsCorporationIdWalletsDivisionJournalGet](#schemacorporationscorporationidwalletsdivisionjournalget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|
|200|X-Pages|integer|int64|The total number of pages in the result set.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-wallet.read_corporation_wallets.v1 )
</aside>

## GetCorporationsCorporationIdWalletsDivisionTransactions

<a id="opIdGetCorporationsCorporationIdWalletsDivisionTransactions"></a>

`GET /corporations/{corporation_id}/wallets/{division}/transactions`

*Get corporation wallet transactions*

Get wallet transactions of a corporation

<h3 id="getcorporationscorporationidwalletsdivisiontransactions-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|corporation_id|path|[CorporationID](#schemacorporationid)|true|The ID of the corporation|
|division|path|integer(int64)|true|none|
|from_id|query|integer(int64)|false|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "client_id": 0,
    "date": "2019-08-24T14:15:22Z",
    "is_buy": true,
    "journal_ref_id": 0,
    "location_id": 0,
    "quantity": 0,
    "transaction_id": 0,
    "type_id": 0,
    "unit_price": 0.1
  }
]
```

<h3 id="getcorporationscorporationidwalletsdivisiontransactions-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[CorporationsCorporationIdWalletsDivisionTransactionsGet](#schemacorporationscorporationidwalletsdivisiontransactionsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
OAuth2 ( Scopes: esi-wallet.read_corporation_wallets.v1 )
</aside>

<h1 id="eve-stable-infrastructure-esi-tranquility-wars">Wars</h1>

## GetWars

<a id="opIdGetWars"></a>

`GET /wars`

*List wars*

Return a list of wars

<h3 id="getwars-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|max_war_id|query|integer(int64)|false|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  0
]
```

<h3 id="getwars-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[WarsGet](#schemawarsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetWarsWarId

<a id="opIdGetWarsWarId"></a>

`GET /wars/{war_id}`

*Get war information*

Return details about a war

<h3 id="getwarswarid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|war_id|path|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
{
  "aggressor": {
    "alliance_id": 0,
    "corporation_id": 0,
    "isk_destroyed": 0.1,
    "ships_killed": 0
  },
  "allies": [
    {
      "alliance_id": 0,
      "corporation_id": 0
    }
  ],
  "declared": "2019-08-24T14:15:22Z",
  "defender": {
    "alliance_id": 0,
    "corporation_id": 0,
    "isk_destroyed": 0.1,
    "ships_killed": 0
  },
  "finished": "2019-08-24T14:15:22Z",
  "id": 0,
  "mutual": true,
  "open_for_allies": true,
  "retracted": "2019-08-24T14:15:22Z",
  "started": "2019-08-24T14:15:22Z"
}
```

<h3 id="getwarswarid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[WarsWarIdGet](#schemawarswaridget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|

<aside class="success">
This operation does not require authentication
</aside>

## GetWarsWarIdKillmails

<a id="opIdGetWarsWarIdKillmails"></a>

`GET /wars/{war_id}/killmails`

*List kills for a war*

Return a list of kills related to a war

<h3 id="getwarswaridkillmails-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|page|query|integer(int32)|false|none|
|war_id|path|integer(int64)|true|none|
|Accept-Language|header|string|false|The language to use for the response.|
|If-None-Match|header|string|false|The ETag of the previous request. A 304 will be returned if this matches the current ETag.|
|X-Compatibility-Date|header|string(date)|true|The compatibility date for the request.|
|X-Tenant|header|string|false|The tenant ID for the request.|

#### Enumerated Values

|Parameter|Value|
|---|---|
|Accept-Language|en|
|Accept-Language|de|
|Accept-Language|fr|
|Accept-Language|ja|
|Accept-Language|ru|
|Accept-Language|zh|
|Accept-Language|ko|
|Accept-Language|es|
|X-Compatibility-Date|2025-11-06|

> Example responses

> 200 Response

```json
[
  {
    "killmail_hash": "string",
    "killmail_id": 0
  }
]
```

<h3 id="getwarswaridkillmails-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[WarsWarIdKillmailsGet](#schemawarswaridkillmailsget)|
|default|Default|Error|[Error](#schemaerror)|

### Response Headers

|Status|Header|Type|Format|Description|
|---|---|---|---|---|
|200|Cache-Control|string||Directives for caching mechanisms. It controls how the response can be cached, by whom, and for how long.|
|200|ETag|string||The ETag value of the response body. Use this with If-None-Match to check whether the resource has changed.|
|200|Last-Modified|string||The last modified date of the response. Use this with If-Modified-Since to check whether the resource has changed.|
|200|X-Pages|integer|int64|The total number of pages in the result set.|

<aside class="success">
This operation does not require authentication
</aside>

# Schemas

<h2 id="tocS_AllianceID">AllianceID</h2>
<!-- backwards compatibility -->
<a id="schemaallianceid"></a>
<a id="schema_AllianceID"></a>
<a id="tocSallianceid"></a>
<a id="tocsallianceid"></a>

```json
99000001

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|integer(int64)|false|none|none|

<h2 id="tocS_AlliancesAllianceIdContactsGet">AlliancesAllianceIdContactsGet</h2>
<!-- backwards compatibility -->
<a id="schemaalliancesallianceidcontactsget"></a>
<a id="schema_AlliancesAllianceIdContactsGet"></a>
<a id="tocSalliancesallianceidcontactsget"></a>
<a id="tocsalliancesallianceidcontactsget"></a>

```json
[
  {
    "contact_id": 0,
    "contact_type": "character",
    "label_ids": [
      0
    ],
    "standing": 0.1
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|contact_id|integer(int64)|true|none|none|
|contact_type|string|true|none|none|
|label_ids|[integer]|false|none|none|
|standing|number(double)|true|none|Standing of the contact|

#### Enumerated Values

|Property|Value|
|---|---|
|contact_type|character|
|contact_type|corporation|
|contact_type|alliance|
|contact_type|faction|

<h2 id="tocS_AlliancesAllianceIdContactsLabelsGet">AlliancesAllianceIdContactsLabelsGet</h2>
<!-- backwards compatibility -->
<a id="schemaalliancesallianceidcontactslabelsget"></a>
<a id="schema_AlliancesAllianceIdContactsLabelsGet"></a>
<a id="tocSalliancesallianceidcontactslabelsget"></a>
<a id="tocsalliancesallianceidcontactslabelsget"></a>

```json
[
  {
    "label_id": 0,
    "label_name": "string"
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|label_id|integer(int64)|true|none|none|
|label_name|string|true|none|none|

<h2 id="tocS_AlliancesAllianceIdCorporationsGet">AlliancesAllianceIdCorporationsGet</h2>
<!-- backwards compatibility -->
<a id="schemaalliancesallianceidcorporationsget"></a>
<a id="schema_AlliancesAllianceIdCorporationsGet"></a>
<a id="tocSalliancesallianceidcorporationsget"></a>
<a id="tocsalliancesallianceidcorporationsget"></a>

```json
[
  0
]

```

### Properties

*None*

<h2 id="tocS_AlliancesAllianceIdGet">AlliancesAllianceIdGet</h2>
<!-- backwards compatibility -->
<a id="schemaalliancesallianceidget"></a>
<a id="schema_AlliancesAllianceIdGet"></a>
<a id="tocSalliancesallianceidget"></a>
<a id="tocsalliancesallianceidget"></a>

```json
{
  "creator_corporation_id": 0,
  "creator_id": 0,
  "date_founded": "2019-08-24T14:15:22Z",
  "executor_corporation_id": 0,
  "faction_id": 0,
  "name": "string",
  "ticker": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|creator_corporation_id|integer(int64)|true|none|ID of the corporation that created the alliance|
|creator_id|integer(int64)|true|none|ID of the character that created the alliance|
|date_founded|string(date-time)|true|none|none|
|executor_corporation_id|integer(int64)|false|none|the executor corporation ID, if this alliance is not closed|
|faction_id|integer(int64)|false|none|Faction ID this alliance is fighting for, if this alliance is enlisted in factional warfare|
|name|string|true|none|the full name of the alliance|
|ticker|string|true|none|the short name of the alliance|

<h2 id="tocS_AlliancesAllianceIdIconsGet">AlliancesAllianceIdIconsGet</h2>
<!-- backwards compatibility -->
<a id="schemaalliancesallianceidiconsget"></a>
<a id="schema_AlliancesAllianceIdIconsGet"></a>
<a id="tocSalliancesallianceidiconsget"></a>
<a id="tocsalliancesallianceidiconsget"></a>

```json
{
  "px128x128": "string",
  "px64x64": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|px128x128|string|false|none|none|
|px64x64|string|false|none|none|

<h2 id="tocS_AlliancesGet">AlliancesGet</h2>
<!-- backwards compatibility -->
<a id="schemaalliancesget"></a>
<a id="schema_AlliancesGet"></a>
<a id="tocSalliancesget"></a>
<a id="tocsalliancesget"></a>

```json
[
  0
]

```

### Properties

*None*

<h2 id="tocS_ArchetypeID">ArchetypeID</h2>
<!-- backwards compatibility -->
<a id="schemaarchetypeid"></a>
<a id="schema_ArchetypeID"></a>
<a id="tocSarchetypeid"></a>
<a id="tocsarchetypeid"></a>

```json
33

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|integer(int64)|false|none|none|

<h2 id="tocS_AttributeID">AttributeID</h2>
<!-- backwards compatibility -->
<a id="schemaattributeid"></a>
<a id="schema_AttributeID"></a>
<a id="tocSattributeid"></a>
<a id="tocsattributeid"></a>

```json
209

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|integer(int64)|false|none|none|

<h2 id="tocS_CharacterID">CharacterID</h2>
<!-- backwards compatibility -->
<a id="schemacharacterid"></a>
<a id="schema_CharacterID"></a>
<a id="tocScharacterid"></a>
<a id="tocscharacterid"></a>

```json
90000001

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|integer(int64)|false|none|none|

<h2 id="tocS_CharactersAffiliationPost">CharactersAffiliationPost</h2>
<!-- backwards compatibility -->
<a id="schemacharactersaffiliationpost"></a>
<a id="schema_CharactersAffiliationPost"></a>
<a id="tocScharactersaffiliationpost"></a>
<a id="tocscharactersaffiliationpost"></a>

```json
[
  {
    "alliance_id": 0,
    "character_id": 0,
    "corporation_id": 0,
    "faction_id": 0
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|alliance_id|integer(int64)|false|none|The character's alliance ID, if their corporation is in an alliance|
|character_id|integer(int64)|true|none|The character's ID|
|corporation_id|integer(int64)|true|none|The character's corporation ID|
|faction_id|integer(int64)|false|none|The character's faction ID, if their corporation is in a faction|

<h2 id="tocS_CharactersCharacterIdAgentsResearchGet">CharactersCharacterIdAgentsResearchGet</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridagentsresearchget"></a>
<a id="schema_CharactersCharacterIdAgentsResearchGet"></a>
<a id="tocScharacterscharacteridagentsresearchget"></a>
<a id="tocscharacterscharacteridagentsresearchget"></a>

```json
[
  {
    "agent_id": 0,
    "points_per_day": 0.1,
    "remainder_points": 0.1,
    "skill_type_id": 0,
    "started_at": "2019-08-24T14:15:22Z"
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|agent_id|integer(int64)|true|none|none|
|points_per_day|number(double)|true|none|none|
|remainder_points|number(double)|true|none|none|
|skill_type_id|integer(int64)|true|none|none|
|started_at|string(date-time)|true|none|none|

<h2 id="tocS_CharactersCharacterIdAssetsGet">CharactersCharacterIdAssetsGet</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridassetsget"></a>
<a id="schema_CharactersCharacterIdAssetsGet"></a>
<a id="tocScharacterscharacteridassetsget"></a>
<a id="tocscharacterscharacteridassetsget"></a>

```json
[
  {
    "is_blueprint_copy": true,
    "is_singleton": true,
    "item_id": 0,
    "location_flag": "AssetSafety",
    "location_id": 0,
    "location_type": "station",
    "quantity": 0,
    "type_id": 0
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|is_blueprint_copy|boolean|false|none|none|
|is_singleton|boolean|true|none|none|
|item_id|integer(int64)|true|none|none|
|location_flag|string|true|none|none|
|location_id|integer(int64)|true|none|none|
|location_type|string|true|none|none|
|quantity|integer(int64)|true|none|none|
|type_id|integer(int64)|true|none|none|

#### Enumerated Values

|Property|Value|
|---|---|
|location_flag|AssetSafety|
|location_flag|AutoFit|
|location_flag|BoosterBay|
|location_flag|CapsuleerDeliveries|
|location_flag|Cargo|
|location_flag|CorporationGoalDeliveries|
|location_flag|CorpseBay|
|location_flag|Deliveries|
|location_flag|DroneBay|
|location_flag|ExpeditionHold|
|location_flag|FighterBay|
|location_flag|FighterTube0|
|location_flag|FighterTube1|
|location_flag|FighterTube2|
|location_flag|FighterTube3|
|location_flag|FighterTube4|
|location_flag|FleetHangar|
|location_flag|FrigateEscapeBay|
|location_flag|Hangar|
|location_flag|HangarAll|
|location_flag|HiSlot0|
|location_flag|HiSlot1|
|location_flag|HiSlot2|
|location_flag|HiSlot3|
|location_flag|HiSlot4|
|location_flag|HiSlot5|
|location_flag|HiSlot6|
|location_flag|HiSlot7|
|location_flag|HiddenModifiers|
|location_flag|Implant|
|location_flag|InfrastructureHangar|
|location_flag|LoSlot0|
|location_flag|LoSlot1|
|location_flag|LoSlot2|
|location_flag|LoSlot3|
|location_flag|LoSlot4|
|location_flag|LoSlot5|
|location_flag|LoSlot6|
|location_flag|LoSlot7|
|location_flag|Locked|
|location_flag|MedSlot0|
|location_flag|MedSlot1|
|location_flag|MedSlot2|
|location_flag|MedSlot3|
|location_flag|MedSlot4|
|location_flag|MedSlot5|
|location_flag|MedSlot6|
|location_flag|MedSlot7|
|location_flag|MobileDepotHold|
|location_flag|MoonMaterialBay|
|location_flag|QuafeBay|
|location_flag|RigSlot0|
|location_flag|RigSlot1|
|location_flag|RigSlot2|
|location_flag|RigSlot3|
|location_flag|RigSlot4|
|location_flag|RigSlot5|
|location_flag|RigSlot6|
|location_flag|RigSlot7|
|location_flag|ShipHangar|
|location_flag|Skill|
|location_flag|SpecializedAmmoHold|
|location_flag|SpecializedAsteroidHold|
|location_flag|SpecializedCommandCenterHold|
|location_flag|SpecializedFuelBay|
|location_flag|SpecializedGasHold|
|location_flag|SpecializedIceHold|
|location_flag|SpecializedIndustrialShipHold|
|location_flag|SpecializedLargeShipHold|
|location_flag|SpecializedMaterialBay|
|location_flag|SpecializedMediumShipHold|
|location_flag|SpecializedMineralHold|
|location_flag|SpecializedOreHold|
|location_flag|SpecializedPlanetaryCommoditiesHold|
|location_flag|SpecializedSalvageHold|
|location_flag|SpecializedShipHold|
|location_flag|SpecializedSmallShipHold|
|location_flag|StructureDeedBay|
|location_flag|SubSystemBay|
|location_flag|SubSystemSlot0|
|location_flag|SubSystemSlot1|
|location_flag|SubSystemSlot2|
|location_flag|SubSystemSlot3|
|location_flag|SubSystemSlot4|
|location_flag|SubSystemSlot5|
|location_flag|SubSystemSlot6|
|location_flag|SubSystemSlot7|
|location_flag|Unlocked|
|location_flag|Wardrobe|
|location_type|station|
|location_type|solar_system|
|location_type|item|
|location_type|other|

<h2 id="tocS_CharactersCharacterIdAssetsLocationsPost">CharactersCharacterIdAssetsLocationsPost</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridassetslocationspost"></a>
<a id="schema_CharactersCharacterIdAssetsLocationsPost"></a>
<a id="tocScharacterscharacteridassetslocationspost"></a>
<a id="tocscharacterscharacteridassetslocationspost"></a>

```json
[
  {
    "item_id": 0,
    "position": {
      "x": 0.1,
      "y": 0.1,
      "z": 0.1
    }
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|item_id|integer(int64)|true|none|none|
|position|object|true|none|none|
|» x|number(double)|true|none|none|
|» y|number(double)|true|none|none|
|» z|number(double)|true|none|none|

<h2 id="tocS_CharactersCharacterIdAssetsNamesPost">CharactersCharacterIdAssetsNamesPost</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridassetsnamespost"></a>
<a id="schema_CharactersCharacterIdAssetsNamesPost"></a>
<a id="tocScharacterscharacteridassetsnamespost"></a>
<a id="tocscharacterscharacteridassetsnamespost"></a>

```json
[
  {
    "item_id": 0,
    "name": "string"
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|item_id|integer(int64)|true|none|none|
|name|string|true|none|none|

<h2 id="tocS_CharactersCharacterIdAttributesGet">CharactersCharacterIdAttributesGet</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridattributesget"></a>
<a id="schema_CharactersCharacterIdAttributesGet"></a>
<a id="tocScharacterscharacteridattributesget"></a>
<a id="tocscharacterscharacteridattributesget"></a>

```json
{
  "accrued_remap_cooldown_date": "2019-08-24T14:15:22Z",
  "bonus_remaps": 0,
  "charisma": 0,
  "intelligence": 0,
  "last_remap_date": "2019-08-24T14:15:22Z",
  "memory": 0,
  "perception": 0,
  "willpower": 0
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|accrued_remap_cooldown_date|string(date-time)|false|none|Neural remapping cooldown after a character uses remap accrued over time|
|bonus_remaps|integer(int64)|false|none|Number of available bonus character neural remaps|
|charisma|integer(int64)|true|none|none|
|intelligence|integer(int64)|true|none|none|
|last_remap_date|string(date-time)|false|none|Datetime of last neural remap, including usage of bonus remaps|
|memory|integer(int64)|true|none|none|
|perception|integer(int64)|true|none|none|
|willpower|integer(int64)|true|none|none|

<h2 id="tocS_CharactersCharacterIdBlueprintsGet">CharactersCharacterIdBlueprintsGet</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridblueprintsget"></a>
<a id="schema_CharactersCharacterIdBlueprintsGet"></a>
<a id="tocScharacterscharacteridblueprintsget"></a>
<a id="tocscharacterscharacteridblueprintsget"></a>

```json
[
  {
    "item_id": 0,
    "location_flag": "AutoFit",
    "location_id": 0,
    "material_efficiency": 0,
    "quantity": 0,
    "runs": 0,
    "time_efficiency": 0,
    "type_id": 0
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|item_id|integer(int64)|true|none|Unique ID for this item.|
|location_flag|string|true|none|Type of the location_id|
|location_id|integer(int64)|true|none|References a station, a ship or an item_id if this blueprint is located within a container. If the return value is an item_id, then the Character AssetList API must be queried to find the container using the given item_id to determine the correct location of the Blueprint.|
|material_efficiency|integer(int64)|true|none|Material Efficiency Level of the blueprint.|
|quantity|integer(int64)|true|none|A range of numbers with a minimum of -2 and no maximum value where -1 is an original and -2 is a copy. It can be a positive integer if it is a stack of blueprint originals fresh from the market (e.g. no activities performed on them yet).|
|runs|integer(int64)|true|none|Number of runs remaining if the blueprint is a copy, -1 if it is an original.|
|time_efficiency|integer(int64)|true|none|Time Efficiency Level of the blueprint.|
|type_id|integer(int64)|true|none|none|

#### Enumerated Values

|Property|Value|
|---|---|
|location_flag|AutoFit|
|location_flag|Cargo|
|location_flag|CorpseBay|
|location_flag|DroneBay|
|location_flag|FleetHangar|
|location_flag|Deliveries|
|location_flag|HiddenModifiers|
|location_flag|Hangar|
|location_flag|HangarAll|
|location_flag|LoSlot0|
|location_flag|LoSlot1|
|location_flag|LoSlot2|
|location_flag|LoSlot3|
|location_flag|LoSlot4|
|location_flag|LoSlot5|
|location_flag|LoSlot6|
|location_flag|LoSlot7|
|location_flag|MedSlot0|
|location_flag|MedSlot1|
|location_flag|MedSlot2|
|location_flag|MedSlot3|
|location_flag|MedSlot4|
|location_flag|MedSlot5|
|location_flag|MedSlot6|
|location_flag|MedSlot7|
|location_flag|HiSlot0|
|location_flag|HiSlot1|
|location_flag|HiSlot2|
|location_flag|HiSlot3|
|location_flag|HiSlot4|
|location_flag|HiSlot5|
|location_flag|HiSlot6|
|location_flag|HiSlot7|
|location_flag|AssetSafety|
|location_flag|Locked|
|location_flag|Unlocked|
|location_flag|Implant|
|location_flag|QuafeBay|
|location_flag|RigSlot0|
|location_flag|RigSlot1|
|location_flag|RigSlot2|
|location_flag|RigSlot3|
|location_flag|RigSlot4|
|location_flag|RigSlot5|
|location_flag|RigSlot6|
|location_flag|RigSlot7|
|location_flag|ShipHangar|
|location_flag|SpecializedFuelBay|
|location_flag|SpecializedOreHold|
|location_flag|SpecializedGasHold|
|location_flag|SpecializedMineralHold|
|location_flag|SpecializedSalvageHold|
|location_flag|SpecializedShipHold|
|location_flag|SpecializedSmallShipHold|
|location_flag|SpecializedMediumShipHold|
|location_flag|SpecializedLargeShipHold|
|location_flag|SpecializedIndustrialShipHold|
|location_flag|SpecializedAmmoHold|
|location_flag|SpecializedCommandCenterHold|
|location_flag|SpecializedPlanetaryCommoditiesHold|
|location_flag|SpecializedMaterialBay|
|location_flag|SubSystemSlot0|
|location_flag|SubSystemSlot1|
|location_flag|SubSystemSlot2|
|location_flag|SubSystemSlot3|
|location_flag|SubSystemSlot4|
|location_flag|SubSystemSlot5|
|location_flag|SubSystemSlot6|
|location_flag|SubSystemSlot7|
|location_flag|FighterBay|
|location_flag|FighterTube0|
|location_flag|FighterTube1|
|location_flag|FighterTube2|
|location_flag|FighterTube3|
|location_flag|FighterTube4|
|location_flag|Module|

<h2 id="tocS_CharactersCharacterIdCalendarEventIdAttendeesGet">CharactersCharacterIdCalendarEventIdAttendeesGet</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridcalendareventidattendeesget"></a>
<a id="schema_CharactersCharacterIdCalendarEventIdAttendeesGet"></a>
<a id="tocScharacterscharacteridcalendareventidattendeesget"></a>
<a id="tocscharacterscharacteridcalendareventidattendeesget"></a>

```json
[
  {
    "character_id": 0,
    "event_response": "declined"
  }
]

```

List of attendees for a given event

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|character_id|integer(int64)|false|none|none|
|event_response|string|false|none|none|

#### Enumerated Values

|Property|Value|
|---|---|
|event_response|declined|
|event_response|not_responded|
|event_response|accepted|
|event_response|tentative|

<h2 id="tocS_CharactersCharacterIdCalendarEventIdGet">CharactersCharacterIdCalendarEventIdGet</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridcalendareventidget"></a>
<a id="schema_CharactersCharacterIdCalendarEventIdGet"></a>
<a id="tocScharacterscharacteridcalendareventidget"></a>
<a id="tocscharacterscharacteridcalendareventidget"></a>

```json
{
  "date": "2019-08-24T14:15:22Z",
  "duration": 0,
  "event_id": 0,
  "importance": 0,
  "owner_id": 0,
  "owner_name": "string",
  "owner_type": "eve_server",
  "response": "string",
  "text": "string",
  "title": "string"
}

```

Full details of a specific event

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|date|string(date-time)|true|none|none|
|duration|integer(int64)|true|none|Length in minutes|
|event_id|integer(int64)|true|none|none|
|importance|integer(int64)|true|none|none|
|owner_id|integer(int64)|true|none|none|
|owner_name|string|true|none|none|
|owner_type|string|true|none|none|
|response|string|true|none|none|
|text|string|true|none|none|
|title|string|true|none|none|

#### Enumerated Values

|Property|Value|
|---|---|
|owner_type|eve_server|
|owner_type|corporation|
|owner_type|faction|
|owner_type|character|
|owner_type|alliance|

<h2 id="tocS_CharactersCharacterIdCalendarGet">CharactersCharacterIdCalendarGet</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridcalendarget"></a>
<a id="schema_CharactersCharacterIdCalendarGet"></a>
<a id="tocScharacterscharacteridcalendarget"></a>
<a id="tocscharacterscharacteridcalendarget"></a>

```json
[
  {
    "event_date": "2019-08-24T14:15:22Z",
    "event_id": 0,
    "event_response": "declined",
    "importance": 0,
    "title": "string"
  }
]

```

Up to 50 events from now or the event you requested

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|event_date|string(date-time)|false|none|none|
|event_id|integer(int64)|false|none|none|
|event_response|string|false|none|none|
|importance|integer(int64)|false|none|none|
|title|string|false|none|none|

#### Enumerated Values

|Property|Value|
|---|---|
|event_response|declined|
|event_response|not_responded|
|event_response|accepted|
|event_response|tentative|

<h2 id="tocS_CharactersCharacterIdClonesGet">CharactersCharacterIdClonesGet</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridclonesget"></a>
<a id="schema_CharactersCharacterIdClonesGet"></a>
<a id="tocScharacterscharacteridclonesget"></a>
<a id="tocscharacterscharacteridclonesget"></a>

```json
{
  "home_location": {
    "location_id": 0,
    "location_type": "station"
  },
  "jump_clones": [
    {
      "implants": [
        0
      ],
      "jump_clone_id": 0,
      "location_id": 0,
      "location_type": "station",
      "name": "string"
    }
  ],
  "last_clone_jump_date": "2019-08-24T14:15:22Z",
  "last_station_change_date": "2019-08-24T14:15:22Z"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|home_location|object|false|none|none|
|» location_id|integer(int64)|false|none|none|
|» location_type|string|false|none|none|
|jump_clones|[object]|true|none|none|
|» implants|[integer]|true|none|none|
|» jump_clone_id|integer(int64)|true|none|none|
|» location_id|integer(int64)|true|none|none|
|» location_type|string|true|none|none|
|» name|string|false|none|none|
|last_clone_jump_date|string(date-time)|false|none|none|
|last_station_change_date|string(date-time)|false|none|none|

#### Enumerated Values

|Property|Value|
|---|---|
|location_type|station|
|location_type|structure|
|location_type|station|
|location_type|structure|

<h2 id="tocS_CharactersCharacterIdContactsGet">CharactersCharacterIdContactsGet</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridcontactsget"></a>
<a id="schema_CharactersCharacterIdContactsGet"></a>
<a id="tocScharacterscharacteridcontactsget"></a>
<a id="tocscharacterscharacteridcontactsget"></a>

```json
[
  {
    "contact_id": 0,
    "contact_type": "character",
    "is_blocked": true,
    "is_watched": true,
    "label_ids": [
      0
    ],
    "standing": 0.1
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|contact_id|integer(int64)|true|none|none|
|contact_type|string|true|none|none|
|is_blocked|boolean|false|none|Whether this contact is in the blocked list. Note a missing value denotes unknown, not true or false|
|is_watched|boolean|false|none|Whether this contact is being watched|
|label_ids|[integer]|false|none|none|
|standing|number(double)|true|none|Standing of the contact|

#### Enumerated Values

|Property|Value|
|---|---|
|contact_type|character|
|contact_type|corporation|
|contact_type|alliance|
|contact_type|faction|

<h2 id="tocS_CharactersCharacterIdContactsLabelsGet">CharactersCharacterIdContactsLabelsGet</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridcontactslabelsget"></a>
<a id="schema_CharactersCharacterIdContactsLabelsGet"></a>
<a id="tocScharacterscharacteridcontactslabelsget"></a>
<a id="tocscharacterscharacteridcontactslabelsget"></a>

```json
[
  {
    "label_id": 0,
    "label_name": "string"
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|label_id|integer(int64)|true|none|none|
|label_name|string|true|none|none|

<h2 id="tocS_CharactersCharacterIdContactsPost">CharactersCharacterIdContactsPost</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridcontactspost"></a>
<a id="schema_CharactersCharacterIdContactsPost"></a>
<a id="tocScharacterscharacteridcontactspost"></a>
<a id="tocscharacterscharacteridcontactspost"></a>

```json
[
  0
]

```

201 created array

### Properties

*None*

<h2 id="tocS_CharactersCharacterIdContractsContractIdBidsGet">CharactersCharacterIdContractsContractIdBidsGet</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridcontractscontractidbidsget"></a>
<a id="schema_CharactersCharacterIdContractsContractIdBidsGet"></a>
<a id="tocScharacterscharacteridcontractscontractidbidsget"></a>
<a id="tocscharacterscharacteridcontractscontractidbidsget"></a>

```json
[
  {
    "amount": 0.1,
    "bid_id": 0,
    "bidder_id": 0,
    "date_bid": "2019-08-24T14:15:22Z"
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|amount|number(double)|true|none|The amount bid, in ISK|
|bid_id|integer(int64)|true|none|Unique ID for the bid|
|bidder_id|integer(int64)|true|none|Character ID of the bidder|
|date_bid|string(date-time)|true|none|Datetime when the bid was placed|

<h2 id="tocS_CharactersCharacterIdContractsContractIdItemsGet">CharactersCharacterIdContractsContractIdItemsGet</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridcontractscontractiditemsget"></a>
<a id="schema_CharactersCharacterIdContractsContractIdItemsGet"></a>
<a id="tocScharacterscharacteridcontractscontractiditemsget"></a>
<a id="tocscharacterscharacteridcontractscontractiditemsget"></a>

```json
[
  {
    "is_included": true,
    "is_singleton": true,
    "quantity": 0,
    "raw_quantity": 0,
    "record_id": 0,
    "type_id": 0
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|is_included|boolean|true|none|true if the contract issuer has submitted this item with the contract, false if the isser is asking for this item in the contract|
|is_singleton|boolean|true|none|none|
|quantity|integer(int64)|true|none|Number of items in the stack|
|raw_quantity|integer(int64)|false|none|-1 indicates that the item is a singleton (non-stackable). If the item happens to be a Blueprint, -1 is an Original and -2 is a Blueprint Copy|
|record_id|integer(int64)|true|none|Unique ID for the item|
|type_id|integer(int64)|true|none|Type ID for item|

<h2 id="tocS_CharactersCharacterIdContractsGet">CharactersCharacterIdContractsGet</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridcontractsget"></a>
<a id="schema_CharactersCharacterIdContractsGet"></a>
<a id="tocScharacterscharacteridcontractsget"></a>
<a id="tocscharacterscharacteridcontractsget"></a>

```json
[
  {
    "acceptor_id": 0,
    "assignee_id": 0,
    "availability": "public",
    "buyout": 0.1,
    "collateral": 0.1,
    "contract_id": 0,
    "date_accepted": "2019-08-24T14:15:22Z",
    "date_completed": "2019-08-24T14:15:22Z",
    "date_expired": "2019-08-24T14:15:22Z",
    "date_issued": "2019-08-24T14:15:22Z",
    "days_to_complete": 0,
    "end_location_id": 0,
    "for_corporation": true,
    "issuer_corporation_id": 0,
    "issuer_id": 0,
    "price": 0.1,
    "reward": 0.1,
    "start_location_id": 0,
    "status": "outstanding",
    "title": "string",
    "type": "unknown",
    "volume": 0.1
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|acceptor_id|integer(int64)|true|none|Who will accept the contract|
|assignee_id|integer(int64)|true|none|ID to whom the contract is assigned, can be alliance, corporation or character ID|
|availability|string|true|none|To whom the contract is available|
|buyout|number(double)|false|none|Buyout price (for Auctions only)|
|collateral|number(double)|false|none|Collateral price (for Couriers only)|
|contract_id|integer(int64)|true|none|none|
|date_accepted|string(date-time)|false|none|Date of confirmation of contract|
|date_completed|string(date-time)|false|none|Date of completed of contract|
|date_expired|string(date-time)|true|none|Expiration date of the contract|
|date_issued|string(date-time)|true|none|Сreation date of the contract|
|days_to_complete|integer(int64)|false|none|Number of days to perform the contract|
|end_location_id|integer(int64)|false|none|End location ID (for Couriers contract)|
|for_corporation|boolean|true|none|true if the contract was issued on behalf of the issuer's corporation|
|issuer_corporation_id|integer(int64)|true|none|Character's corporation ID for the issuer|
|issuer_id|integer(int64)|true|none|Character ID for the issuer|
|price|number(double)|false|none|Price of contract (for ItemsExchange and Auctions)|
|reward|number(double)|false|none|Remuneration for contract (for Couriers only)|
|start_location_id|integer(int64)|false|none|Start location ID (for Couriers contract)|
|status|string|true|none|Status of the the contract|
|title|string|false|none|Title of the contract|
|type|string|true|none|Type of the contract|
|volume|number(double)|false|none|Volume of items in the contract|

#### Enumerated Values

|Property|Value|
|---|---|
|availability|public|
|availability|personal|
|availability|corporation|
|availability|alliance|
|status|outstanding|
|status|in_progress|
|status|finished_issuer|
|status|finished_contractor|
|status|finished|
|status|cancelled|
|status|rejected|
|status|failed|
|status|deleted|
|status|reversed|
|type|unknown|
|type|item_exchange|
|type|auction|
|type|courier|
|type|loan|

<h2 id="tocS_CharactersCharacterIdCorporationhistoryGet">CharactersCharacterIdCorporationhistoryGet</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridcorporationhistoryget"></a>
<a id="schema_CharactersCharacterIdCorporationhistoryGet"></a>
<a id="tocScharacterscharacteridcorporationhistoryget"></a>
<a id="tocscharacterscharacteridcorporationhistoryget"></a>

```json
[
  {
    "corporation_id": 0,
    "is_deleted": true,
    "record_id": 0,
    "start_date": "2019-08-24T14:15:22Z"
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|corporation_id|integer(int64)|true|none|none|
|is_deleted|boolean|false|none|True if the corporation has been deleted|
|record_id|integer(int64)|true|none|An incrementing ID that can be used to canonically establish order of records in cases where dates may be ambiguous|
|start_date|string(date-time)|true|none|none|

<h2 id="tocS_CharactersCharacterIdCspaPost">CharactersCharacterIdCspaPost</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridcspapost"></a>
<a id="schema_CharactersCharacterIdCspaPost"></a>
<a id="tocScharacterscharacteridcspapost"></a>
<a id="tocscharacterscharacteridcspapost"></a>

```json
0.1

```

201 created number

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|number(double)|false|none|201 created number|

<h2 id="tocS_CharactersCharacterIdFatigueGet">CharactersCharacterIdFatigueGet</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridfatigueget"></a>
<a id="schema_CharactersCharacterIdFatigueGet"></a>
<a id="tocScharacterscharacteridfatigueget"></a>
<a id="tocscharacterscharacteridfatigueget"></a>

```json
{
  "jump_fatigue_expire_date": "2019-08-24T14:15:22Z",
  "last_jump_date": "2019-08-24T14:15:22Z",
  "last_update_date": "2019-08-24T14:15:22Z"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|jump_fatigue_expire_date|string(date-time)|false|none|Character's jump fatigue expiry|
|last_jump_date|string(date-time)|false|none|Character's last jump activation|
|last_update_date|string(date-time)|false|none|Character's last jump update|

<h2 id="tocS_CharactersCharacterIdFittingsGet">CharactersCharacterIdFittingsGet</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridfittingsget"></a>
<a id="schema_CharactersCharacterIdFittingsGet"></a>
<a id="tocScharacterscharacteridfittingsget"></a>
<a id="tocscharacterscharacteridfittingsget"></a>

```json
[
  {
    "description": "string",
    "fitting_id": 0,
    "items": [
      {
        "flag": "Cargo",
        "quantity": 0,
        "type_id": 0
      }
    ],
    "name": "string",
    "ship_type_id": 0
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|description|string|true|none|none|
|fitting_id|integer(int64)|true|none|none|
|items|[object]|true|none|none|
|» flag|string|true|none|none|
|» quantity|integer(int64)|true|none|none|
|» type_id|integer(int64)|true|none|none|
|name|string|true|none|none|
|ship_type_id|integer(int64)|true|none|none|

#### Enumerated Values

|Property|Value|
|---|---|
|flag|Cargo|
|flag|DroneBay|
|flag|FighterBay|
|flag|HiSlot0|
|flag|HiSlot1|
|flag|HiSlot2|
|flag|HiSlot3|
|flag|HiSlot4|
|flag|HiSlot5|
|flag|HiSlot6|
|flag|HiSlot7|
|flag|Invalid|
|flag|LoSlot0|
|flag|LoSlot1|
|flag|LoSlot2|
|flag|LoSlot3|
|flag|LoSlot4|
|flag|LoSlot5|
|flag|LoSlot6|
|flag|LoSlot7|
|flag|MedSlot0|
|flag|MedSlot1|
|flag|MedSlot2|
|flag|MedSlot3|
|flag|MedSlot4|
|flag|MedSlot5|
|flag|MedSlot6|
|flag|MedSlot7|
|flag|RigSlot0|
|flag|RigSlot1|
|flag|RigSlot2|
|flag|ServiceSlot0|
|flag|ServiceSlot1|
|flag|ServiceSlot2|
|flag|ServiceSlot3|
|flag|ServiceSlot4|
|flag|ServiceSlot5|
|flag|ServiceSlot6|
|flag|ServiceSlot7|
|flag|SubSystemSlot0|
|flag|SubSystemSlot1|
|flag|SubSystemSlot2|
|flag|SubSystemSlot3|

<h2 id="tocS_CharactersCharacterIdFittingsPost">CharactersCharacterIdFittingsPost</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridfittingspost"></a>
<a id="schema_CharactersCharacterIdFittingsPost"></a>
<a id="tocScharacterscharacteridfittingspost"></a>
<a id="tocscharacterscharacteridfittingspost"></a>

```json
{
  "fitting_id": 0
}

```

201 created object

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|fitting_id|integer(int64)|true|none|none|

<h2 id="tocS_CharactersCharacterIdFleetGet">CharactersCharacterIdFleetGet</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridfleetget"></a>
<a id="schema_CharactersCharacterIdFleetGet"></a>
<a id="tocScharacterscharacteridfleetget"></a>
<a id="tocscharacterscharacteridfleetget"></a>

```json
{
  "fleet_boss_id": 0,
  "fleet_id": 0,
  "role": "fleet_commander",
  "squad_id": 0,
  "wing_id": 0
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|fleet_boss_id|integer(int64)|true|none|Character ID of the current fleet boss|
|fleet_id|integer(int64)|true|none|The character's current fleet ID|
|role|string|true|none|Member’s role in fleet|
|squad_id|integer(int64)|true|none|ID of the squad the member is in. If not applicable, will be set to -1|
|wing_id|integer(int64)|true|none|ID of the wing the member is in. If not applicable, will be set to -1|

#### Enumerated Values

|Property|Value|
|---|---|
|role|fleet_commander|
|role|squad_commander|
|role|squad_member|
|role|wing_commander|

<h2 id="tocS_CharactersCharacterIdFwStatsGet">CharactersCharacterIdFwStatsGet</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridfwstatsget"></a>
<a id="schema_CharactersCharacterIdFwStatsGet"></a>
<a id="tocScharacterscharacteridfwstatsget"></a>
<a id="tocscharacterscharacteridfwstatsget"></a>

```json
{
  "current_rank": 0,
  "enlisted_on": "2019-08-24T14:15:22Z",
  "faction_id": 0,
  "highest_rank": 0,
  "kills": {
    "last_week": 0,
    "total": 0,
    "yesterday": 0
  },
  "victory_points": {
    "last_week": 0,
    "total": 0,
    "yesterday": 0
  }
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|current_rank|integer(int64)|false|none|The given character's current faction rank|
|enlisted_on|string(date-time)|false|none|The enlistment date of the given character into faction warfare. Will not be included if character is not enlisted in faction warfare|
|faction_id|integer(int64)|false|none|The faction the given character is enlisted to fight for. Will not be included if character is not enlisted in faction warfare|
|highest_rank|integer(int64)|false|none|The given character's highest faction rank achieved|
|kills|object|true|none|Summary of kills done by the given character against enemy factions|
|» last_week|integer(int64)|true|none|Last week's total number of kills by a given character against enemy factions|
|» total|integer(int64)|true|none|Total number of kills by a given character against enemy factions since the character enlisted|
|» yesterday|integer(int64)|true|none|Yesterday's total number of kills by a given character against enemy factions|
|victory_points|object|true|none|Summary of victory points gained by the given character for the enlisted faction|
|» last_week|integer(int64)|true|none|Last week's victory points gained by the given character|
|» total|integer(int64)|true|none|Total victory points gained since the given character enlisted|
|» yesterday|integer(int64)|true|none|Yesterday's victory points gained by the given character|

<h2 id="tocS_CharactersCharacterIdGet">CharactersCharacterIdGet</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridget"></a>
<a id="schema_CharactersCharacterIdGet"></a>
<a id="tocScharacterscharacteridget"></a>
<a id="tocscharacterscharacteridget"></a>

```json
{
  "alliance_id": 0,
  "birthday": "2019-08-24T14:15:22Z",
  "bloodline_id": 0,
  "corporation_id": 0,
  "description": "string",
  "faction_id": 0,
  "gender": "female",
  "name": "string",
  "race_id": 0,
  "security_status": 0.1,
  "title": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|alliance_id|integer(int64)|false|none|The character's alliance ID|
|birthday|string(date-time)|true|none|Creation date of the character|
|bloodline_id|integer(int64)|true|none|none|
|corporation_id|integer(int64)|true|none|The character's corporation ID|
|description|string|false|none|none|
|faction_id|integer(int64)|false|none|ID of the faction the character is fighting for, if the character is enlisted in Factional Warfare|
|gender|string|true|none|none|
|name|string|true|none|none|
|race_id|integer(int64)|true|none|none|
|security_status|number(double)|false|none|none|
|title|string|false|none|The individual title of the character|

#### Enumerated Values

|Property|Value|
|---|---|
|gender|female|
|gender|male|

<h2 id="tocS_CharactersCharacterIdImplantsGet">CharactersCharacterIdImplantsGet</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridimplantsget"></a>
<a id="schema_CharactersCharacterIdImplantsGet"></a>
<a id="tocScharacterscharacteridimplantsget"></a>
<a id="tocscharacterscharacteridimplantsget"></a>

```json
[
  0
]

```

### Properties

*None*

<h2 id="tocS_CharactersCharacterIdIndustryJobsGet">CharactersCharacterIdIndustryJobsGet</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridindustryjobsget"></a>
<a id="schema_CharactersCharacterIdIndustryJobsGet"></a>
<a id="tocScharacterscharacteridindustryjobsget"></a>
<a id="tocscharacterscharacteridindustryjobsget"></a>

```json
[
  {
    "activity_id": 0,
    "blueprint_id": 0,
    "blueprint_location_id": 0,
    "blueprint_type_id": 0,
    "completed_character_id": 0,
    "completed_date": "2019-08-24T14:15:22Z",
    "cost": 0.1,
    "duration": 0,
    "end_date": "2019-08-24T14:15:22Z",
    "facility_id": 0,
    "installer_id": 0,
    "job_id": 0,
    "licensed_runs": 0,
    "output_location_id": 0,
    "pause_date": "2019-08-24T14:15:22Z",
    "probability": 0.1,
    "product_type_id": 0,
    "runs": 0,
    "start_date": "2019-08-24T14:15:22Z",
    "station_id": 0,
    "status": "active",
    "successful_runs": 0
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|activity_id|integer(int64)|true|none|Job activity ID|
|blueprint_id|integer(int64)|true|none|none|
|blueprint_location_id|integer(int64)|true|none|Location ID of the location from which the blueprint was installed. Normally a station ID, but can also be an asset (e.g. container) or corporation facility|
|blueprint_type_id|integer(int64)|true|none|none|
|completed_character_id|integer(int64)|false|none|ID of the character which completed this job|
|completed_date|string(date-time)|false|none|Date and time when this job was completed|
|cost|number(double)|false|none|The sume of job installation fee and industry facility tax|
|duration|integer(int64)|true|none|Job duration in seconds|
|end_date|string(date-time)|true|none|Date and time when this job finished|
|facility_id|integer(int64)|true|none|ID of the facility where this job is running|
|installer_id|integer(int64)|true|none|ID of the character which installed this job|
|job_id|integer(int64)|true|none|Unique job ID|
|licensed_runs|integer(int64)|false|none|Number of runs blueprint is licensed for|
|output_location_id|integer(int64)|true|none|Location ID of the location to which the output of the job will be delivered. Normally a station ID, but can also be a corporation facility|
|pause_date|string(date-time)|false|none|Date and time when this job was paused (i.e. time when the facility where this job was installed went offline)|
|probability|number(double)|false|none|Chance of success for invention|
|product_type_id|integer(int64)|false|none|Type ID of product (manufactured, copied or invented)|
|runs|integer(int64)|true|none|Number of runs for a manufacturing job, or number of copies to make for a blueprint copy|
|start_date|string(date-time)|true|none|Date and time when this job started|
|station_id|integer(int64)|true|none|ID of the station where industry facility is located|
|status|string|true|none|none|
|successful_runs|integer(int64)|false|none|Number of successful runs for this job. Equal to runs unless this is an invention job|

#### Enumerated Values

|Property|Value|
|---|---|
|status|active|
|status|cancelled|
|status|delivered|
|status|paused|
|status|ready|
|status|reverted|

<h2 id="tocS_CharactersCharacterIdKillmailsRecentGet">CharactersCharacterIdKillmailsRecentGet</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridkillmailsrecentget"></a>
<a id="schema_CharactersCharacterIdKillmailsRecentGet"></a>
<a id="tocScharacterscharacteridkillmailsrecentget"></a>
<a id="tocscharacterscharacteridkillmailsrecentget"></a>

```json
[
  {
    "killmail_hash": "string",
    "killmail_id": 0
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|killmail_hash|string|true|none|A hash of this killmail|
|killmail_id|integer(int64)|true|none|ID of this killmail|

<h2 id="tocS_CharactersCharacterIdLocationGet">CharactersCharacterIdLocationGet</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridlocationget"></a>
<a id="schema_CharactersCharacterIdLocationGet"></a>
<a id="tocScharacterscharacteridlocationget"></a>
<a id="tocscharacterscharacteridlocationget"></a>

```json
{
  "solar_system_id": 0,
  "station_id": 0,
  "structure_id": 0
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|solar_system_id|integer(int64)|true|none|none|
|station_id|integer(int64)|false|none|none|
|structure_id|integer(int64)|false|none|none|

<h2 id="tocS_CharactersCharacterIdLoyaltyPointsGet">CharactersCharacterIdLoyaltyPointsGet</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridloyaltypointsget"></a>
<a id="schema_CharactersCharacterIdLoyaltyPointsGet"></a>
<a id="tocScharacterscharacteridloyaltypointsget"></a>
<a id="tocscharacterscharacteridloyaltypointsget"></a>

```json
[
  {
    "corporation_id": 0,
    "loyalty_points": 0
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|corporation_id|integer(int64)|true|none|none|
|loyalty_points|integer(int64)|true|none|none|

<h2 id="tocS_CharactersCharacterIdMailGet">CharactersCharacterIdMailGet</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridmailget"></a>
<a id="schema_CharactersCharacterIdMailGet"></a>
<a id="tocScharacterscharacteridmailget"></a>
<a id="tocscharacterscharacteridmailget"></a>

```json
[
  {
    "from": 0,
    "is_read": true,
    "labels": [
      0
    ],
    "mail_id": 0,
    "recipients": [
      {
        "recipient_id": 0,
        "recipient_type": "alliance"
      }
    ],
    "subject": "string",
    "timestamp": "2019-08-24T14:15:22Z"
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|from|integer(int64)|false|none|From whom the mail was sent|
|is_read|boolean|false|none|none|
|labels|[integer]|false|none|none|
|mail_id|integer(int64)|false|none|none|
|recipients|[object]|false|none|Recipients of the mail|
|» recipient_id|integer(int64)|true|none|none|
|» recipient_type|string|true|none|none|
|subject|string|false|none|Mail subject|
|timestamp|string(date-time)|false|none|When the mail was sent|

#### Enumerated Values

|Property|Value|
|---|---|
|recipient_type|alliance|
|recipient_type|character|
|recipient_type|corporation|
|recipient_type|mailing_list|

<h2 id="tocS_CharactersCharacterIdMailLabelsGet">CharactersCharacterIdMailLabelsGet</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridmaillabelsget"></a>
<a id="schema_CharactersCharacterIdMailLabelsGet"></a>
<a id="tocScharacterscharacteridmaillabelsget"></a>
<a id="tocscharacterscharacteridmaillabelsget"></a>

```json
{
  "labels": [
    {
      "color": "#0000fe",
      "label_id": 0,
      "name": "string",
      "unread_count": 0
    }
  ],
  "total_unread_count": 0
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|labels|[object]|false|none|none|
|» color|string|false|none|none|
|» label_id|integer(int64)|false|none|none|
|» name|string|false|none|none|
|» unread_count|integer(int64)|false|none|none|
|total_unread_count|integer(int64)|false|none|none|

#### Enumerated Values

|Property|Value|
|---|---|
|color|#0000fe|
|color|#006634|
|color|#0099ff|
|color|#00ff33|
|color|#01ffff|
|color|#349800|
|color|#660066|
|color|#666666|
|color|#999999|
|color|#99ffff|
|color|#9a0000|
|color|#ccff9a|
|color|#e6e6e6|
|color|#fe0000|
|color|#ff6600|
|color|#ffff01|
|color|#ffffcd|
|color|#ffffff|

<h2 id="tocS_CharactersCharacterIdMailLabelsPost">CharactersCharacterIdMailLabelsPost</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridmaillabelspost"></a>
<a id="schema_CharactersCharacterIdMailLabelsPost"></a>
<a id="tocScharacterscharacteridmaillabelspost"></a>
<a id="tocscharacterscharacteridmaillabelspost"></a>

```json
0

```

Label ID

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|integer(int64)|false|none|Label ID|

<h2 id="tocS_CharactersCharacterIdMailListsGet">CharactersCharacterIdMailListsGet</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridmaillistsget"></a>
<a id="schema_CharactersCharacterIdMailListsGet"></a>
<a id="tocScharacterscharacteridmaillistsget"></a>
<a id="tocscharacterscharacteridmaillistsget"></a>

```json
[
  {
    "mailing_list_id": 0,
    "name": "string"
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|mailing_list_id|integer(int64)|true|none|Mailing list ID|
|name|string|true|none|none|

<h2 id="tocS_CharactersCharacterIdMailMailIdGet">CharactersCharacterIdMailMailIdGet</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridmailmailidget"></a>
<a id="schema_CharactersCharacterIdMailMailIdGet"></a>
<a id="tocScharacterscharacteridmailmailidget"></a>
<a id="tocscharacterscharacteridmailmailidget"></a>

```json
{
  "body": "string",
  "from": 0,
  "labels": [
    0
  ],
  "read": true,
  "recipients": [
    {
      "recipient_id": 0,
      "recipient_type": "alliance"
    }
  ],
  "subject": "string",
  "timestamp": "2019-08-24T14:15:22Z"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|body|string|false|none|Mail's body|
|from|integer(int64)|false|none|From whom the mail was sent|
|labels|[integer]|false|none|Labels attached to the mail|
|read|boolean|false|none|Whether the mail is flagged as read|
|recipients|[object]|false|none|Recipients of the mail|
|» recipient_id|integer(int64)|true|none|none|
|» recipient_type|string|true|none|none|
|subject|string|false|none|Mail subject|
|timestamp|string(date-time)|false|none|When the mail was sent|

#### Enumerated Values

|Property|Value|
|---|---|
|recipient_type|alliance|
|recipient_type|character|
|recipient_type|corporation|
|recipient_type|mailing_list|

<h2 id="tocS_CharactersCharacterIdMailPost">CharactersCharacterIdMailPost</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridmailpost"></a>
<a id="schema_CharactersCharacterIdMailPost"></a>
<a id="tocScharacterscharacteridmailpost"></a>
<a id="tocscharacterscharacteridmailpost"></a>

```json
0

```

Mail ID

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|integer(int64)|false|none|Mail ID|

<h2 id="tocS_CharactersCharacterIdMedalsGet">CharactersCharacterIdMedalsGet</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridmedalsget"></a>
<a id="schema_CharactersCharacterIdMedalsGet"></a>
<a id="tocScharacterscharacteridmedalsget"></a>
<a id="tocscharacterscharacteridmedalsget"></a>

```json
[
  {
    "corporation_id": 0,
    "date": "2019-08-24T14:15:22Z",
    "description": "string",
    "graphics": [
      {
        "color": 0,
        "graphic": "string",
        "layer": 0,
        "part": 0
      }
    ],
    "issuer_id": 0,
    "medal_id": 0,
    "reason": "string",
    "status": "public",
    "title": "string"
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|corporation_id|integer(int64)|true|none|none|
|date|string(date-time)|true|none|none|
|description|string|true|none|none|
|graphics|[object]|true|none|none|
|» color|integer(int64)|false|none|none|
|» graphic|string|true|none|none|
|» layer|integer(int64)|true|none|none|
|» part|integer(int64)|true|none|none|
|issuer_id|integer(int64)|true|none|none|
|medal_id|integer(int64)|true|none|none|
|reason|string|true|none|none|
|status|string|true|none|none|
|title|string|true|none|none|

#### Enumerated Values

|Property|Value|
|---|---|
|status|public|
|status|private|

<h2 id="tocS_CharactersCharacterIdMiningGet">CharactersCharacterIdMiningGet</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridminingget"></a>
<a id="schema_CharactersCharacterIdMiningGet"></a>
<a id="tocScharacterscharacteridminingget"></a>
<a id="tocscharacterscharacteridminingget"></a>

```json
[
  {
    "date": "2019-08-24",
    "quantity": 0,
    "solar_system_id": 0,
    "type_id": 0
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|date|string(date)|true|none|none|
|quantity|integer(int64)|true|none|none|
|solar_system_id|integer(int64)|true|none|none|
|type_id|integer(int64)|true|none|none|

<h2 id="tocS_CharactersCharacterIdNotificationsContactsGet">CharactersCharacterIdNotificationsContactsGet</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridnotificationscontactsget"></a>
<a id="schema_CharactersCharacterIdNotificationsContactsGet"></a>
<a id="tocScharacterscharacteridnotificationscontactsget"></a>
<a id="tocscharacterscharacteridnotificationscontactsget"></a>

```json
[
  {
    "message": "string",
    "notification_id": 0,
    "send_date": "2019-08-24T14:15:22Z",
    "sender_character_id": 0,
    "standing_level": 0.1
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|message|string|true|none|none|
|notification_id|integer(int64)|true|none|none|
|send_date|string(date-time)|true|none|none|
|sender_character_id|integer(int64)|true|none|none|
|standing_level|number(double)|true|none|A number representing the standing level the receiver has been added at by the sender. The standing levels are as follows: -10 -> Terrible | -5 -> Bad |  0 -> Neutral |  5 -> Good |  10 -> Excellent|

<h2 id="tocS_CharactersCharacterIdNotificationsGet">CharactersCharacterIdNotificationsGet</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridnotificationsget"></a>
<a id="schema_CharactersCharacterIdNotificationsGet"></a>
<a id="tocScharacterscharacteridnotificationsget"></a>
<a id="tocscharacterscharacteridnotificationsget"></a>

```json
[
  {
    "is_read": true,
    "notification_id": 0,
    "sender_id": 0,
    "sender_type": "character",
    "text": "string",
    "timestamp": "2019-08-24T14:15:22Z",
    "type": "AcceptedAlly"
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|is_read|boolean|false|none|none|
|notification_id|integer(int64)|true|none|none|
|sender_id|integer(int64)|true|none|none|
|sender_type|string|true|none|none|
|text|string|false|none|none|
|timestamp|string(date-time)|true|none|none|
|type|string|true|none|none|

#### Enumerated Values

|Property|Value|
|---|---|
|sender_type|character|
|sender_type|corporation|
|sender_type|alliance|
|sender_type|faction|
|sender_type|other|
|type|AcceptedAlly|
|type|AcceptedSurrender|
|type|AgentRetiredTrigravian|
|type|AllAnchoringMsg|
|type|AllMaintenanceBillMsg|
|type|AllStrucInvulnerableMsg|
|type|AllStructVulnerableMsg|
|type|AllWarCorpJoinedAllianceMsg|
|type|AllWarDeclaredMsg|
|type|AllWarInvalidatedMsg|
|type|AllWarRetractedMsg|
|type|AllWarSurrenderMsg|
|type|AllianceCapitalChanged|
|type|AllianceWarDeclaredV2|
|type|AllyContractCancelled|
|type|AllyJoinedWarAggressorMsg|
|type|AllyJoinedWarAllyMsg|
|type|AllyJoinedWarDefenderMsg|
|type|BattlePunishFriendlyFire|
|type|BillOutOfMoneyMsg|
|type|BillPaidCorpAllMsg|
|type|BountyClaimMsg|
|type|BountyESSShared|
|type|BountyESSTaken|
|type|BountyPlacedAlliance|
|type|BountyPlacedChar|
|type|BountyPlacedCorp|
|type|BountyYourBountyClaimed|
|type|BuddyConnectContactAdd|
|type|CharAppAcceptMsg|
|type|CharAppRejectMsg|
|type|CharAppWithdrawMsg|
|type|CharLeftCorpMsg|
|type|CharMedalMsg|
|type|CharTerminationMsg|
|type|CloneActivationMsg|
|type|CloneActivationMsg2|
|type|CloneMovedMsg|
|type|CloneRevokedMsg1|
|type|CloneRevokedMsg2|
|type|CombatOperationFinished|
|type|ContactAdd|
|type|ContactEdit|
|type|ContainerPasswordMsg|
|type|ContractRegionChangedToPochven|
|type|CorpAllBillMsg|
|type|CorpAppAcceptMsg|
|type|CorpAppInvitedMsg|
|type|CorpAppNewMsg|
|type|CorpAppRejectCustomMsg|
|type|CorpAppRejectMsg|
|type|CorpBecameWarEligible|
|type|CorpDividendMsg|
|type|CorpFriendlyFireDisableTimerCompleted|
|type|CorpFriendlyFireDisableTimerStarted|
|type|CorpFriendlyFireEnableTimerCompleted|
|type|CorpFriendlyFireEnableTimerStarted|
|type|CorpKicked|
|type|CorpLiquidationMsg|
|type|CorpNewCEOMsg|
|type|CorpNewsMsg|
|type|CorpNoLongerWarEligible|
|type|CorpOfficeExpirationMsg|
|type|CorpStructLostMsg|
|type|CorpTaxChangeMsg|
|type|CorpVoteCEORevokedMsg|
|type|CorpVoteMsg|
|type|CorpWarDeclaredMsg|
|type|CorpWarDeclaredV2|
|type|CorpWarFightingLegalMsg|
|type|CorpWarInvalidatedMsg|
|type|CorpWarRetractedMsg|
|type|CorpWarSurrenderMsg|
|type|CorporationGoalClosed|
|type|CorporationGoalCompleted|
|type|CorporationGoalCreated|
|type|CorporationGoalExpired|
|type|CorporationGoalLimitReached|
|type|CorporationGoalNameChange|
|type|CorporationLeft|
|type|CustomsMsg|
|type|DailyItemRewardAutoClaimed|
|type|DeclareWar|
|type|DistrictAttacked|
|type|DustAppAcceptedMsg|
|type|ESSMainBankLink|
|type|EntosisCaptureStarted|
|type|ExpertSystemExpired|
|type|ExpertSystemExpiryImminent|
|type|FWAllianceKickMsg|
|type|FWAllianceWarningMsg|
|type|FWCharKickMsg|
|type|FWCharRankGainMsg|
|type|FWCharRankLossMsg|
|type|FWCharWarningMsg|
|type|FWCorpJoinMsg|
|type|FWCorpKickMsg|
|type|FWCorpLeaveMsg|
|type|FWCorpWarningMsg|
|type|FacWarCorpJoinRequestMsg|
|type|FacWarCorpJoinWithdrawMsg|
|type|FacWarCorpLeaveRequestMsg|
|type|FacWarCorpLeaveWithdrawMsg|
|type|FacWarDirectEnlistmentRevoked|
|type|FacWarLPDisqualifiedEvent|
|type|FacWarLPDisqualifiedKill|
|type|FacWarLPPayoutEvent|
|type|FacWarLPPayoutKill|
|type|FreelanceProjectClosed|
|type|FreelanceProjectCompleted|
|type|FreelanceProjectCreated|
|type|FreelanceProjectExpired|
|type|FreelanceProjectLimitReached|
|type|FreelanceProjectParticipantKicked|
|type|GameTimeAdded|
|type|GameTimeReceived|
|type|GameTimeSent|
|type|GiftReceived|
|type|IHubDestroyedByBillFailure|
|type|IncursionCompletedMsg|
|type|IndustryOperationFinished|
|type|IndustryTeamAuctionLost|
|type|IndustryTeamAuctionWon|
|type|InfrastructureHubBillAboutToExpire|
|type|InsuranceExpirationMsg|
|type|InsuranceFirstShipMsg|
|type|InsuranceInvalidatedMsg|
|type|InsuranceIssuedMsg|
|type|InsurancePayoutMsg|
|type|InvasionCompletedMsg|
|type|InvasionSystemLogin|
|type|InvasionSystemStart|
|type|JumpCloneDeletedMsg1|
|type|JumpCloneDeletedMsg2|
|type|KillReportFinalBlow|
|type|KillReportVictim|
|type|KillRightAvailable|
|type|KillRightAvailableOpen|
|type|KillRightEarned|
|type|KillRightUnavailable|
|type|KillRightUnavailableOpen|
|type|KillRightUsed|
|type|LPAutoRedeemed|
|type|LocateCharMsg|
|type|MadeWarMutual|
|type|MercOfferRetractedMsg|
|type|MercOfferedNegotiationMsg|
|type|MercenaryDenAttacked|
|type|MercenaryDenNewMTO|
|type|MercenaryDenReinforced|
|type|MissionCanceledTriglavian|
|type|MissionOfferExpirationMsg|
|type|MissionTimeoutMsg|
|type|MoonminingAutomaticFracture|
|type|MoonminingExtractionCancelled|
|type|MoonminingExtractionFinished|
|type|MoonminingExtractionStarted|
|type|MoonminingLaserFired|
|type|MutualWarExpired|
|type|MutualWarInviteAccepted|
|type|MutualWarInviteRejected|
|type|MutualWarInviteSent|
|type|NPCStandingsGained|
|type|NPCStandingsLost|
|type|OfferToAllyRetracted|
|type|OfferedSurrender|
|type|OfferedToAlly|
|type|OfficeLeaseCanceledInsufficientStandings|
|type|OldLscMessages|
|type|OperationFinished|
|type|OrbitalAttacked|
|type|OrbitalReinforced|
|type|OwnershipTransferred|
|type|RaffleCreated|
|type|RaffleExpired|
|type|RaffleFinished|
|type|ReimbursementMsg|
|type|ResearchMissionAvailableMsg|
|type|RetractsWar|
|type|SPAutoRedeemed|
|type|SeasonalChallengeCompleted|
|type|SkinSequencingCompleted|
|type|SkyhookDeployed|
|type|SkyhookDestroyed|
|type|SkyhookLostShields|
|type|SkyhookOnline|
|type|SkyhookUnderAttack|
|type|SovAllClaimAquiredMsg|
|type|SovAllClaimLostMsg|
|type|SovCommandNodeEventStarted|
|type|SovCorpBillLateMsg|
|type|SovCorpClaimFailMsg|
|type|SovDisruptorMsg|
|type|SovStationEnteredFreeport|
|type|SovStructureDestroyed|
|type|SovStructureReinforced|
|type|SovStructureSelfDestructCancel|
|type|SovStructureSelfDestructFinished|
|type|SovStructureSelfDestructRequested|
|type|SovereigntyIHDamageMsg|
|type|SovereigntySBUDamageMsg|
|type|SovereigntyTCUDamageMsg|
|type|StationAggressionMsg1|
|type|StationAggressionMsg2|
|type|StationConquerMsg|
|type|StationServiceDisabled|
|type|StationServiceEnabled|
|type|StationStateChangeMsg|
|type|StoryLineMissionAvailableMsg|
|type|StructureAnchoring|
|type|StructureCourierContractChanged|
|type|StructureDestroyed|
|type|StructureFuelAlert|
|type|StructureImpendingAbandonmentAssetsAtRisk|
|type|StructureItemsDelivered|
|type|StructureItemsMovedToSafety|
|type|StructureLostArmor|
|type|StructureLostShields|
|type|StructureLowReagentsAlert|
|type|StructureNoReagentsAlert|
|type|StructureOnline|
|type|StructurePaintPurchased|
|type|StructureServicesOffline|
|type|StructureUnanchoring|
|type|StructureUnderAttack|
|type|StructureWentHighPower|
|type|StructureWentLowPower|
|type|StructuresJobsCancelled|
|type|StructuresJobsPaused|
|type|StructuresReinforcementChanged|
|type|TowerAlertMsg|
|type|TowerResourceAlertMsg|
|type|TransactionReversalMsg|
|type|TutorialMsg|
|type|WarAdopted |
|type|WarAllyInherited|
|type|WarAllyOfferDeclinedMsg|
|type|WarConcordInvalidates|
|type|WarDeclared|
|type|WarEndedHqSecurityDrop|
|type|WarHQRemovedFromSpace|
|type|WarInherited|
|type|WarInvalid|
|type|WarRetracted|
|type|WarRetractedByConcord|
|type|WarSurrenderDeclinedMsg|
|type|WarSurrenderOfferMsg|

<h2 id="tocS_CharactersCharacterIdOnlineGet">CharactersCharacterIdOnlineGet</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridonlineget"></a>
<a id="schema_CharactersCharacterIdOnlineGet"></a>
<a id="tocScharacterscharacteridonlineget"></a>
<a id="tocscharacterscharacteridonlineget"></a>

```json
{
  "last_login": "2019-08-24T14:15:22Z",
  "last_logout": "2019-08-24T14:15:22Z",
  "logins": 0,
  "online": true
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|last_login|string(date-time)|false|none|Timestamp of the last login|
|last_logout|string(date-time)|false|none|Timestamp of the last logout|
|logins|integer(int64)|false|none|Total number of times the character has logged in|
|online|boolean|true|none|If the character is online|

<h2 id="tocS_CharactersCharacterIdOrdersGet">CharactersCharacterIdOrdersGet</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridordersget"></a>
<a id="schema_CharactersCharacterIdOrdersGet"></a>
<a id="tocScharacterscharacteridordersget"></a>
<a id="tocscharacterscharacteridordersget"></a>

```json
[
  {
    "duration": 0,
    "escrow": 0.1,
    "is_buy_order": true,
    "is_corporation": true,
    "issued": "2019-08-24T14:15:22Z",
    "location_id": 0,
    "min_volume": 0,
    "order_id": 0,
    "price": 0.1,
    "range": "1",
    "region_id": 0,
    "type_id": 0,
    "volume_remain": 0,
    "volume_total": 0
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|duration|integer(int64)|true|none|Number of days for which order is valid (starting from the issued date). An order expires at time issued + duration|
|escrow|number(double)|false|none|For buy orders, the amount of ISK in escrow|
|is_buy_order|boolean|false|none|True if the order is a bid (buy) order|
|is_corporation|boolean|true|none|Signifies whether the buy/sell order was placed on behalf of a corporation.|
|issued|string(date-time)|true|none|Date and time when this order was issued|
|location_id|integer(int64)|true|none|ID of the location where order was placed|
|min_volume|integer(int64)|false|none|For buy orders, the minimum quantity that will be accepted in a matching sell order|
|order_id|integer(int64)|true|none|Unique order ID|
|price|number(double)|true|none|Cost per unit for this order|
|range|string|true|none|Valid order range, numbers are ranges in jumps|
|region_id|integer(int64)|true|none|ID of the region where order was placed|
|type_id|integer(int64)|true|none|The type ID of the item transacted in this order|
|volume_remain|integer(int64)|true|none|Quantity of items still required or offered|
|volume_total|integer(int64)|true|none|Quantity of items required or offered at time order was placed|

#### Enumerated Values

|Property|Value|
|---|---|
|range|1|
|range|10|
|range|2|
|range|20|
|range|3|
|range|30|
|range|4|
|range|40|
|range|5|
|range|region|
|range|solarsystem|
|range|station|

<h2 id="tocS_CharactersCharacterIdOrdersHistoryGet">CharactersCharacterIdOrdersHistoryGet</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridordershistoryget"></a>
<a id="schema_CharactersCharacterIdOrdersHistoryGet"></a>
<a id="tocScharacterscharacteridordershistoryget"></a>
<a id="tocscharacterscharacteridordershistoryget"></a>

```json
[
  {
    "duration": 0,
    "escrow": 0.1,
    "is_buy_order": true,
    "is_corporation": true,
    "issued": "2019-08-24T14:15:22Z",
    "location_id": 0,
    "min_volume": 0,
    "order_id": 0,
    "price": 0.1,
    "range": "1",
    "region_id": 0,
    "state": "cancelled",
    "type_id": 0,
    "volume_remain": 0,
    "volume_total": 0
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|duration|integer(int64)|true|none|Number of days the order was valid for (starting from the issued date). An order expires at time issued + duration|
|escrow|number(double)|false|none|For buy orders, the amount of ISK in escrow|
|is_buy_order|boolean|false|none|True if the order is a bid (buy) order|
|is_corporation|boolean|true|none|Signifies whether the buy/sell order was placed on behalf of a corporation.|
|issued|string(date-time)|true|none|Date and time when this order was issued|
|location_id|integer(int64)|true|none|ID of the location where order was placed|
|min_volume|integer(int64)|false|none|For buy orders, the minimum quantity that will be accepted in a matching sell order|
|order_id|integer(int64)|true|none|Unique order ID|
|price|number(double)|true|none|Cost per unit for this order|
|range|string|true|none|Valid order range, numbers are ranges in jumps|
|region_id|integer(int64)|true|none|ID of the region where order was placed|
|state|string|true|none|Current order state|
|type_id|integer(int64)|true|none|The type ID of the item transacted in this order|
|volume_remain|integer(int64)|true|none|Quantity of items still required or offered|
|volume_total|integer(int64)|true|none|Quantity of items required or offered at time order was placed|

#### Enumerated Values

|Property|Value|
|---|---|
|range|1|
|range|10|
|range|2|
|range|20|
|range|3|
|range|30|
|range|4|
|range|40|
|range|5|
|range|region|
|range|solarsystem|
|range|station|
|state|cancelled|
|state|expired|

<h2 id="tocS_CharactersCharacterIdPlanetsGet">CharactersCharacterIdPlanetsGet</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridplanetsget"></a>
<a id="schema_CharactersCharacterIdPlanetsGet"></a>
<a id="tocScharacterscharacteridplanetsget"></a>
<a id="tocscharacterscharacteridplanetsget"></a>

```json
[
  {
    "last_update": "2019-08-24T14:15:22Z",
    "num_pins": 0,
    "owner_id": 0,
    "planet_id": 0,
    "planet_type": "temperate",
    "solar_system_id": 0,
    "upgrade_level": 0
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|last_update|string(date-time)|true|none|none|
|num_pins|integer(int64)|true|none|none|
|owner_id|integer(int64)|true|none|none|
|planet_id|integer(int64)|true|none|none|
|planet_type|string|true|none|none|
|solar_system_id|integer(int64)|true|none|none|
|upgrade_level|integer(int64)|true|none|none|

#### Enumerated Values

|Property|Value|
|---|---|
|planet_type|temperate|
|planet_type|barren|
|planet_type|oceanic|
|planet_type|ice|
|planet_type|gas|
|planet_type|lava|
|planet_type|storm|
|planet_type|plasma|

<h2 id="tocS_CharactersCharacterIdPlanetsPlanetIdGet">CharactersCharacterIdPlanetsPlanetIdGet</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridplanetsplanetidget"></a>
<a id="schema_CharactersCharacterIdPlanetsPlanetIdGet"></a>
<a id="tocScharacterscharacteridplanetsplanetidget"></a>
<a id="tocscharacterscharacteridplanetsplanetidget"></a>

```json
{
  "links": [
    {
      "destination_pin_id": 0,
      "link_level": 0,
      "source_pin_id": 0
    }
  ],
  "pins": [
    {
      "contents": [
        {
          "amount": 0,
          "type_id": 0
        }
      ],
      "expiry_time": "2019-08-24T14:15:22Z",
      "extractor_details": {
        "cycle_time": 0,
        "head_radius": 0.1,
        "heads": [
          {
            "head_id": 0,
            "latitude": 0.1,
            "longitude": 0.1
          }
        ],
        "product_type_id": 0,
        "qty_per_cycle": 0
      },
      "factory_details": {
        "schematic_id": 0
      },
      "install_time": "2019-08-24T14:15:22Z",
      "last_cycle_start": "2019-08-24T14:15:22Z",
      "latitude": 0.1,
      "longitude": 0.1,
      "pin_id": 0,
      "schematic_id": 0,
      "type_id": 0
    }
  ],
  "routes": [
    {
      "content_type_id": 0,
      "destination_pin_id": 0,
      "quantity": 0.1,
      "route_id": 0,
      "source_pin_id": 0,
      "waypoints": [
        0
      ]
    }
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|links|[object]|true|none|none|
|» destination_pin_id|integer(int64)|true|none|none|
|» link_level|integer(int64)|true|none|none|
|» source_pin_id|integer(int64)|true|none|none|
|pins|[object]|true|none|none|
|» contents|[object]|false|none|none|
|»» amount|integer(int64)|true|none|none|
|»» type_id|integer(int64)|true|none|none|
|» expiry_time|string(date-time)|false|none|none|
|» extractor_details|object|false|none|none|
|»» cycle_time|integer(int64)|false|none|in seconds|
|»» head_radius|number(double)|false|none|none|
|»» heads|[object]|true|none|none|
|»»» head_id|integer(int64)|true|none|none|
|»»» latitude|number(double)|true|none|none|
|»»» longitude|number(double)|true|none|none|
|»» product_type_id|integer(int64)|false|none|none|
|»» qty_per_cycle|integer(int64)|false|none|none|
|» factory_details|object|false|none|none|
|»» schematic_id|integer(int64)|true|none|none|
|» install_time|string(date-time)|false|none|none|
|» last_cycle_start|string(date-time)|false|none|none|
|» latitude|number(double)|true|none|none|
|» longitude|number(double)|true|none|none|
|» pin_id|integer(int64)|true|none|none|
|» schematic_id|integer(int64)|false|none|none|
|» type_id|integer(int64)|true|none|none|
|routes|[object]|true|none|none|
|» content_type_id|integer(int64)|true|none|none|
|» destination_pin_id|integer(int64)|true|none|none|
|» quantity|number(double)|true|none|none|
|» route_id|integer(int64)|true|none|none|
|» source_pin_id|integer(int64)|true|none|none|
|» waypoints|[integer]|false|none|list of pin ID waypoints|

<h2 id="tocS_CharactersCharacterIdPortraitGet">CharactersCharacterIdPortraitGet</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridportraitget"></a>
<a id="schema_CharactersCharacterIdPortraitGet"></a>
<a id="tocScharacterscharacteridportraitget"></a>
<a id="tocscharacterscharacteridportraitget"></a>

```json
{
  "px128x128": "string",
  "px256x256": "string",
  "px512x512": "string",
  "px64x64": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|px128x128|string|false|none|none|
|px256x256|string|false|none|none|
|px512x512|string|false|none|none|
|px64x64|string|false|none|none|

<h2 id="tocS_CharactersCharacterIdRolesGet">CharactersCharacterIdRolesGet</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridrolesget"></a>
<a id="schema_CharactersCharacterIdRolesGet"></a>
<a id="tocScharacterscharacteridrolesget"></a>
<a id="tocscharacterscharacteridrolesget"></a>

```json
{
  "roles": [
    "Account_Take_1"
  ],
  "roles_at_base": [
    "Account_Take_1"
  ],
  "roles_at_hq": [
    "Account_Take_1"
  ],
  "roles_at_other": [
    "Account_Take_1"
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|roles|[string]|false|none|none|
|roles_at_base|[string]|false|none|none|
|roles_at_hq|[string]|false|none|none|
|roles_at_other|[string]|false|none|none|

<h2 id="tocS_CharactersCharacterIdSearchGet">CharactersCharacterIdSearchGet</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridsearchget"></a>
<a id="schema_CharactersCharacterIdSearchGet"></a>
<a id="tocScharacterscharacteridsearchget"></a>
<a id="tocscharacterscharacteridsearchget"></a>

```json
{
  "agent": [
    0
  ],
  "alliance": [
    0
  ],
  "character": [
    0
  ],
  "constellation": [
    0
  ],
  "corporation": [
    0
  ],
  "faction": [
    0
  ],
  "inventory_type": [
    0
  ],
  "region": [
    0
  ],
  "solar_system": [
    0
  ],
  "station": [
    0
  ],
  "structure": [
    0
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|agent|[integer]|false|none|none|
|alliance|[integer]|false|none|none|
|character|[integer]|false|none|none|
|constellation|[integer]|false|none|none|
|corporation|[integer]|false|none|none|
|faction|[integer]|false|none|none|
|inventory_type|[integer]|false|none|none|
|region|[integer]|false|none|none|
|solar_system|[integer]|false|none|none|
|station|[integer]|false|none|none|
|structure|[integer]|false|none|none|

<h2 id="tocS_CharactersCharacterIdShipGet">CharactersCharacterIdShipGet</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridshipget"></a>
<a id="schema_CharactersCharacterIdShipGet"></a>
<a id="tocScharacterscharacteridshipget"></a>
<a id="tocscharacterscharacteridshipget"></a>

```json
{
  "ship_item_id": 0,
  "ship_name": "string",
  "ship_type_id": 0
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|ship_item_id|integer(int64)|true|none|Item id's are unique to a ship and persist until it is repackaged. This value can be used to track repeated uses of a ship, or detect when a pilot changes into a different instance of the same ship type.|
|ship_name|string|true|none|none|
|ship_type_id|integer(int64)|true|none|none|

<h2 id="tocS_CharactersCharacterIdSkillqueueGet">CharactersCharacterIdSkillqueueGet</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridskillqueueget"></a>
<a id="schema_CharactersCharacterIdSkillqueueGet"></a>
<a id="tocScharacterscharacteridskillqueueget"></a>
<a id="tocscharacterscharacteridskillqueueget"></a>

```json
[
  {
    "finish_date": "2019-08-24T14:15:22Z",
    "finished_level": 0,
    "level_end_sp": 0,
    "level_start_sp": 0,
    "queue_position": 0,
    "skill_id": 0,
    "start_date": "2019-08-24T14:15:22Z",
    "training_start_sp": 0
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|finish_date|string(date-time)|false|none|Date on which training of the skill will complete. Omitted if the skill queue is paused.|
|finished_level|integer(int64)|true|none|none|
|level_end_sp|integer(int64)|false|none|none|
|level_start_sp|integer(int64)|false|none|Amount of SP that was in the skill when it started training it's current level. Used to calculate % of current level complete.|
|queue_position|integer(int64)|true|none|none|
|skill_id|integer(int64)|true|none|none|
|start_date|string(date-time)|false|none|none|
|training_start_sp|integer(int64)|false|none|none|

<h2 id="tocS_CharactersCharacterIdSkillsGet">CharactersCharacterIdSkillsGet</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridskillsget"></a>
<a id="schema_CharactersCharacterIdSkillsGet"></a>
<a id="tocScharacterscharacteridskillsget"></a>
<a id="tocscharacterscharacteridskillsget"></a>

```json
{
  "skills": [
    {
      "active_skill_level": 0,
      "skill_id": 0,
      "skillpoints_in_skill": 0,
      "trained_skill_level": 0
    }
  ],
  "total_sp": 0,
  "unallocated_sp": 0
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|skills|[object]|true|none|none|
|» active_skill_level|integer(int64)|true|none|none|
|» skill_id|integer(int64)|true|none|none|
|» skillpoints_in_skill|integer(int64)|true|none|none|
|» trained_skill_level|integer(int64)|true|none|none|
|total_sp|integer(int64)|true|none|none|
|unallocated_sp|integer(int64)|false|none|Skill points available to be assigned|

<h2 id="tocS_CharactersCharacterIdStandingsGet">CharactersCharacterIdStandingsGet</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridstandingsget"></a>
<a id="schema_CharactersCharacterIdStandingsGet"></a>
<a id="tocScharacterscharacteridstandingsget"></a>
<a id="tocscharacterscharacteridstandingsget"></a>

```json
[
  {
    "from_id": 0,
    "from_type": "agent",
    "standing": 0.1
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|from_id|integer(int64)|true|none|none|
|from_type|string|true|none|none|
|standing|number(double)|true|none|none|

#### Enumerated Values

|Property|Value|
|---|---|
|from_type|agent|
|from_type|npc_corp|
|from_type|faction|

<h2 id="tocS_CharactersCharacterIdTitlesGet">CharactersCharacterIdTitlesGet</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridtitlesget"></a>
<a id="schema_CharactersCharacterIdTitlesGet"></a>
<a id="tocScharacterscharacteridtitlesget"></a>
<a id="tocscharacterscharacteridtitlesget"></a>

```json
[
  {
    "name": "string",
    "title_id": 0
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|name|string|false|none|none|
|title_id|integer(int64)|false|none|none|

<h2 id="tocS_CharactersCharacterIdWalletGet">CharactersCharacterIdWalletGet</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridwalletget"></a>
<a id="schema_CharactersCharacterIdWalletGet"></a>
<a id="tocScharacterscharacteridwalletget"></a>
<a id="tocscharacterscharacteridwalletget"></a>

```json
0.1

```

Wallet balance

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|number(double)|false|none|Wallet balance|

<h2 id="tocS_CharactersCharacterIdWalletJournalGet">CharactersCharacterIdWalletJournalGet</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridwalletjournalget"></a>
<a id="schema_CharactersCharacterIdWalletJournalGet"></a>
<a id="tocScharacterscharacteridwalletjournalget"></a>
<a id="tocscharacterscharacteridwalletjournalget"></a>

```json
[
  {
    "amount": 0.1,
    "balance": 0.1,
    "context_id": 0,
    "context_id_type": "structure_id",
    "date": "2019-08-24T14:15:22Z",
    "description": "string",
    "first_party_id": 0,
    "id": 0,
    "reason": "string",
    "ref_type": "acceleration_gate_fee",
    "second_party_id": 0,
    "tax": 0.1,
    "tax_receiver_id": 0
  }
]

```

Wallet journal entries

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|amount|number(double)|false|none|The amount of ISK given or taken from the wallet as a result of the given transaction. Positive when ISK is deposited into the wallet and negative when ISK is withdrawn|
|balance|number(double)|false|none|Wallet balance after transaction occurred|
|context_id|integer(int64)|false|none|An ID that gives extra context to the particular transaction. Because of legacy reasons the context is completely different per ref_type and means different things. It is also possible to not have a context_id|
|context_id_type|string|false|none|The type of the given context_id if present|
|date|string(date-time)|true|none|Date and time of transaction|
|description|string|true|none|The reason for the transaction, mirrors what is seen in the client|
|first_party_id|integer(int64)|false|none|The id of the first party involved in the transaction. This attribute has no consistency and is different or non existant for particular ref_types. The description attribute will help make sense of what this attribute means. For more info about the given ID it can be dropped into the /universe/names/ ESI route to determine its type and name|
|id|integer(int64)|true|none|Unique journal reference ID|
|reason|string|false|none|The user stated reason for the transaction. Only applies to some ref_types|
|ref_type|string|true|none|"The transaction type for the given. transaction. Different transaction types will populate different attributes."|
|second_party_id|integer(int64)|false|none|The id of the second party involved in the transaction. This attribute has no consistency and is different or non existant for particular ref_types. The description attribute will help make sense of what this attribute means. For more info about the given ID it can be dropped into the /universe/names/ ESI route to determine its type and name|
|tax|number(double)|false|none|Tax amount received. Only applies to tax related transactions|
|tax_receiver_id|integer(int64)|false|none|The corporation ID receiving any tax paid. Only applies to tax related transactions|

#### Enumerated Values

|Property|Value|
|---|---|
|context_id_type|structure_id|
|context_id_type|station_id|
|context_id_type|market_transaction_id|
|context_id_type|character_id|
|context_id_type|corporation_id|
|context_id_type|alliance_id|
|context_id_type|eve_system|
|context_id_type|industry_job_id|
|context_id_type|contract_id|
|context_id_type|planet_id|
|context_id_type|system_id|
|context_id_type|type_id|
|ref_type|acceleration_gate_fee|
|ref_type|advertisement_listing_fee|
|ref_type|agent_donation|
|ref_type|agent_location_services|
|ref_type|agent_miscellaneous|
|ref_type|agent_mission_collateral_paid|
|ref_type|agent_mission_collateral_refunded|
|ref_type|agent_mission_reward|
|ref_type|agent_mission_reward_corporation_tax|
|ref_type|agent_mission_time_bonus_reward|
|ref_type|agent_mission_time_bonus_reward_corporation_tax|
|ref_type|agent_security_services|
|ref_type|agent_services_rendered|
|ref_type|agents_preward|
|ref_type|air_career_program_reward|
|ref_type|alliance_maintainance_fee|
|ref_type|alliance_registration_fee|
|ref_type|allignment_based_gate_toll|
|ref_type|asset_safety_recovery_tax|
|ref_type|bounty|
|ref_type|bounty_prize|
|ref_type|bounty_prize_corporation_tax|
|ref_type|bounty_prizes|
|ref_type|bounty_reimbursement|
|ref_type|bounty_surcharge|
|ref_type|brokers_fee|
|ref_type|clone_activation|
|ref_type|clone_transfer|
|ref_type|contraband_fine|
|ref_type|contract_auction_bid|
|ref_type|contract_auction_bid_corp|
|ref_type|contract_auction_bid_refund|
|ref_type|contract_auction_sold|
|ref_type|contract_brokers_fee|
|ref_type|contract_brokers_fee_corp|
|ref_type|contract_collateral|
|ref_type|contract_collateral_deposited_corp|
|ref_type|contract_collateral_payout|
|ref_type|contract_collateral_refund|
|ref_type|contract_deposit|
|ref_type|contract_deposit_corp|
|ref_type|contract_deposit_refund|
|ref_type|contract_deposit_sales_tax|
|ref_type|contract_price|
|ref_type|contract_price_payment_corp|
|ref_type|contract_reversal|
|ref_type|contract_reward|
|ref_type|contract_reward_deposited|
|ref_type|contract_reward_deposited_corp|
|ref_type|contract_reward_refund|
|ref_type|contract_sales_tax|
|ref_type|copying|
|ref_type|corporate_reward_payout|
|ref_type|corporate_reward_tax|
|ref_type|corporation_account_withdrawal|
|ref_type|corporation_bulk_payment|
|ref_type|corporation_dividend_payment|
|ref_type|corporation_liquidation|
|ref_type|corporation_logo_change_cost|
|ref_type|corporation_payment|
|ref_type|corporation_registration_fee|
|ref_type|cosmetic_market_component_item_purchase|
|ref_type|cosmetic_market_skin_purchase|
|ref_type|cosmetic_market_skin_sale|
|ref_type|cosmetic_market_skin_sale_broker_fee|
|ref_type|cosmetic_market_skin_sale_tax|
|ref_type|cosmetic_market_skin_transaction|
|ref_type|courier_mission_escrow|
|ref_type|cspa|
|ref_type|cspaofflinerefund|
|ref_type|daily_challenge_reward|
|ref_type|daily_goal_payouts|
|ref_type|daily_goal_payouts_tax|
|ref_type|datacore_fee|
|ref_type|dna_modification_fee|
|ref_type|docking_fee|
|ref_type|duel_wager_escrow|
|ref_type|duel_wager_payment|
|ref_type|duel_wager_refund|
|ref_type|ess_escrow_transfer|
|ref_type|external_trade_delivery|
|ref_type|external_trade_freeze|
|ref_type|external_trade_thaw|
|ref_type|factory_slot_rental_fee|
|ref_type|flux_payout|
|ref_type|flux_tax|
|ref_type|flux_ticket_repayment|
|ref_type|flux_ticket_sale|
|ref_type|freelance_jobs_broadcasting_fee|
|ref_type|freelance_jobs_duration_fee|
|ref_type|freelance_jobs_escrow_refund|
|ref_type|freelance_jobs_reward|
|ref_type|freelance_jobs_reward_corporation_tax|
|ref_type|freelance_jobs_reward_escrow|
|ref_type|gm_cash_transfer|
|ref_type|gm_plex_fee_refund|
|ref_type|industry_job_tax|
|ref_type|infrastructure_hub_maintenance|
|ref_type|inheritance|
|ref_type|insurance|
|ref_type|insurgency_corruption_contribution_reward|
|ref_type|insurgency_suppression_contribution_reward|
|ref_type|item_trader_payment|
|ref_type|jump_clone_activation_fee|
|ref_type|jump_clone_installation_fee|
|ref_type|kill_right_fee|
|ref_type|lp_store|
|ref_type|manufacturing|
|ref_type|market_escrow|
|ref_type|market_fine_paid|
|ref_type|market_provider_tax|
|ref_type|market_transaction|
|ref_type|medal_creation|
|ref_type|medal_issued|
|ref_type|milestone_reward_payment|
|ref_type|mission_completion|
|ref_type|mission_cost|
|ref_type|mission_expiration|
|ref_type|mission_reward|
|ref_type|office_rental_fee|
|ref_type|operation_bonus|
|ref_type|opportunity_reward|
|ref_type|planetary_construction|
|ref_type|planetary_export_tax|
|ref_type|planetary_import_tax|
|ref_type|player_donation|
|ref_type|player_trading|
|ref_type|project_discovery_reward|
|ref_type|project_discovery_tax|
|ref_type|project_payouts|
|ref_type|reaction|
|ref_type|redeemed_isk_token|
|ref_type|release_of_impounded_property|
|ref_type|repair_bill|
|ref_type|reprocessing_tax|
|ref_type|researching_material_productivity|
|ref_type|researching_technology|
|ref_type|researching_time_productivity|
|ref_type|resource_wars_reward|
|ref_type|reverse_engineering|
|ref_type|season_challenge_reward|
|ref_type|security_processing_fee|
|ref_type|shares|
|ref_type|skill_purchase|
|ref_type|skyhook_claim_fee|
|ref_type|sovereignity_bill|
|ref_type|store_purchase|
|ref_type|store_purchase_refund|
|ref_type|structure_gate_jump|
|ref_type|transaction_tax|
|ref_type|under_construction|
|ref_type|upkeep_adjustment_fee|
|ref_type|war_ally_contract|
|ref_type|war_fee|
|ref_type|war_fee_surrender|

<h2 id="tocS_CharactersCharacterIdWalletTransactionsGet">CharactersCharacterIdWalletTransactionsGet</h2>
<!-- backwards compatibility -->
<a id="schemacharacterscharacteridwallettransactionsget"></a>
<a id="schema_CharactersCharacterIdWalletTransactionsGet"></a>
<a id="tocScharacterscharacteridwallettransactionsget"></a>
<a id="tocscharacterscharacteridwallettransactionsget"></a>

```json
[
  {
    "client_id": 0,
    "date": "2019-08-24T14:15:22Z",
    "is_buy": true,
    "is_personal": true,
    "journal_ref_id": 0,
    "location_id": 0,
    "quantity": 0,
    "transaction_id": 0,
    "type_id": 0,
    "unit_price": 0.1
  }
]

```

Wallet transactions

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|client_id|integer(int64)|true|none|none|
|date|string(date-time)|true|none|Date and time of transaction|
|is_buy|boolean|true|none|none|
|is_personal|boolean|true|none|none|
|journal_ref_id|integer(int64)|true|none|none|
|location_id|integer(int64)|true|none|none|
|quantity|integer(int64)|true|none|none|
|transaction_id|integer(int64)|true|none|Unique transaction ID|
|type_id|integer(int64)|true|none|none|
|unit_price|number(double)|true|none|Amount paid per unit|

<h2 id="tocS_CompatibilityDate">CompatibilityDate</h2>
<!-- backwards compatibility -->
<a id="schemacompatibilitydate"></a>
<a id="schema_CompatibilityDate"></a>
<a id="tocScompatibilitydate"></a>
<a id="tocscompatibilitydate"></a>

```json
"2025-08-26"

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|string(date)|false|none|none|

<h2 id="tocS_ConstellationID">ConstellationID</h2>
<!-- backwards compatibility -->
<a id="schemaconstellationid"></a>
<a id="schema_ConstellationID"></a>
<a id="tocSconstellationid"></a>
<a id="tocsconstellationid"></a>

```json
20000001

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|integer(int64)|false|none|none|

<h2 id="tocS_ContractsPublicBidsContractIdGet">ContractsPublicBidsContractIdGet</h2>
<!-- backwards compatibility -->
<a id="schemacontractspublicbidscontractidget"></a>
<a id="schema_ContractsPublicBidsContractIdGet"></a>
<a id="tocScontractspublicbidscontractidget"></a>
<a id="tocscontractspublicbidscontractidget"></a>

```json
[
  {
    "amount": 0.1,
    "bid_id": 0,
    "date_bid": "2019-08-24T14:15:22Z"
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|amount|number(double)|true|none|The amount bid, in ISK|
|bid_id|integer(int64)|true|none|Unique ID for the bid|
|date_bid|string(date-time)|true|none|Datetime when the bid was placed|

<h2 id="tocS_ContractsPublicItemsContractIdGet">ContractsPublicItemsContractIdGet</h2>
<!-- backwards compatibility -->
<a id="schemacontractspublicitemscontractidget"></a>
<a id="schema_ContractsPublicItemsContractIdGet"></a>
<a id="tocScontractspublicitemscontractidget"></a>
<a id="tocscontractspublicitemscontractidget"></a>

```json
[
  {
    "is_blueprint_copy": true,
    "is_included": true,
    "item_id": 0,
    "material_efficiency": 0,
    "quantity": 0,
    "record_id": 0,
    "runs": 0,
    "time_efficiency": 0,
    "type_id": 0
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|is_blueprint_copy|boolean|false|none|none|
|is_included|boolean|true|none|true if the contract issuer has submitted this item with the contract, false if the isser is asking for this item in the contract|
|item_id|integer(int64)|false|none|Unique ID for the item being sold. Not present if item is being requested by contract rather than sold with contract|
|material_efficiency|integer(int64)|false|none|Material Efficiency Level of the blueprint|
|quantity|integer(int64)|true|none|Number of items in the stack|
|record_id|integer(int64)|true|none|Unique ID for the item, used by the contract system|
|runs|integer(int64)|false|none|Number of runs remaining if the blueprint is a copy, -1 if it is an original|
|time_efficiency|integer(int64)|false|none|Time Efficiency Level of the blueprint|
|type_id|integer(int64)|true|none|Type ID for item|

<h2 id="tocS_ContractsPublicRegionIdGet">ContractsPublicRegionIdGet</h2>
<!-- backwards compatibility -->
<a id="schemacontractspublicregionidget"></a>
<a id="schema_ContractsPublicRegionIdGet"></a>
<a id="tocScontractspublicregionidget"></a>
<a id="tocscontractspublicregionidget"></a>

```json
[
  {
    "buyout": 0.1,
    "collateral": 0.1,
    "contract_id": 0,
    "date_expired": "2019-08-24T14:15:22Z",
    "date_issued": "2019-08-24T14:15:22Z",
    "days_to_complete": 0,
    "end_location_id": 0,
    "for_corporation": true,
    "issuer_corporation_id": 0,
    "issuer_id": 0,
    "price": 0.1,
    "reward": 0.1,
    "start_location_id": 0,
    "title": "string",
    "type": "unknown",
    "volume": 0.1
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|buyout|number(double)|false|none|Buyout price (for Auctions only)|
|collateral|number(double)|false|none|Collateral price (for Couriers only)|
|contract_id|integer(int64)|true|none|none|
|date_expired|string(date-time)|true|none|Expiration date of the contract|
|date_issued|string(date-time)|true|none|Сreation date of the contract|
|days_to_complete|integer(int64)|false|none|Number of days to perform the contract|
|end_location_id|integer(int64)|false|none|End location ID (for Couriers contract)|
|for_corporation|boolean|false|none|true if the contract was issued on behalf of the issuer's corporation|
|issuer_corporation_id|integer(int64)|true|none|Character's corporation ID for the issuer|
|issuer_id|integer(int64)|true|none|Character ID for the issuer|
|price|number(double)|false|none|Price of contract (for ItemsExchange and Auctions)|
|reward|number(double)|false|none|Remuneration for contract (for Couriers only)|
|start_location_id|integer(int64)|false|none|Start location ID (for Couriers contract)|
|title|string|false|none|Title of the contract|
|type|string|true|none|Type of the contract|
|volume|number(double)|false|none|Volume of items in the contract|

#### Enumerated Values

|Property|Value|
|---|---|
|type|unknown|
|type|item_exchange|
|type|auction|
|type|courier|
|type|loan|

<h2 id="tocS_CorporationCorporationIdMiningExtractionsGet">CorporationCorporationIdMiningExtractionsGet</h2>
<!-- backwards compatibility -->
<a id="schemacorporationcorporationidminingextractionsget"></a>
<a id="schema_CorporationCorporationIdMiningExtractionsGet"></a>
<a id="tocScorporationcorporationidminingextractionsget"></a>
<a id="tocscorporationcorporationidminingextractionsget"></a>

```json
[
  {
    "chunk_arrival_time": "2019-08-24T14:15:22Z",
    "extraction_start_time": "2019-08-24T14:15:22Z",
    "moon_id": 0,
    "natural_decay_time": "2019-08-24T14:15:22Z",
    "structure_id": 0
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|chunk_arrival_time|string(date-time)|true|none|The time at which the chunk being extracted will arrive and can be fractured by the moon mining drill.|
|extraction_start_time|string(date-time)|true|none|The time at which the current extraction was initiated.|
|moon_id|integer(int64)|true|none|none|
|natural_decay_time|string(date-time)|true|none|The time at which the chunk being extracted will naturally fracture if it is not first fractured by the moon mining drill.|
|structure_id|integer(int64)|true|none|none|

<h2 id="tocS_CorporationCorporationIdMiningObserversGet">CorporationCorporationIdMiningObserversGet</h2>
<!-- backwards compatibility -->
<a id="schemacorporationcorporationidminingobserversget"></a>
<a id="schema_CorporationCorporationIdMiningObserversGet"></a>
<a id="tocScorporationcorporationidminingobserversget"></a>
<a id="tocscorporationcorporationidminingobserversget"></a>

```json
[
  {
    "last_updated": "2019-08-24",
    "observer_id": 0,
    "observer_type": "structure"
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|last_updated|string(date)|true|none|none|
|observer_id|integer(int64)|true|none|The entity that was observing the asteroid field when it was mined.|
|observer_type|string|true|none|The category of the observing entity|

#### Enumerated Values

|Property|Value|
|---|---|
|observer_type|structure|

<h2 id="tocS_CorporationCorporationIdMiningObserversObserverIdGet">CorporationCorporationIdMiningObserversObserverIdGet</h2>
<!-- backwards compatibility -->
<a id="schemacorporationcorporationidminingobserversobserveridget"></a>
<a id="schema_CorporationCorporationIdMiningObserversObserverIdGet"></a>
<a id="tocScorporationcorporationidminingobserversobserveridget"></a>
<a id="tocscorporationcorporationidminingobserversobserveridget"></a>

```json
[
  {
    "character_id": 0,
    "last_updated": "2019-08-24",
    "quantity": 0,
    "recorded_corporation_id": 0,
    "type_id": 0
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|character_id|integer(int64)|true|none|The character that did the mining|
|last_updated|string(date)|true|none|none|
|quantity|integer(int64)|true|none|none|
|recorded_corporation_id|integer(int64)|true|none|The corporation id of the character at the time data was recorded.|
|type_id|integer(int64)|true|none|none|

<h2 id="tocS_CorporationID">CorporationID</h2>
<!-- backwards compatibility -->
<a id="schemacorporationid"></a>
<a id="schema_CorporationID"></a>
<a id="tocScorporationid"></a>
<a id="tocscorporationid"></a>

```json
98777771

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|integer(int64)|false|none|none|

<h2 id="tocS_CorporationsCorporationIdAlliancehistoryGet">CorporationsCorporationIdAlliancehistoryGet</h2>
<!-- backwards compatibility -->
<a id="schemacorporationscorporationidalliancehistoryget"></a>
<a id="schema_CorporationsCorporationIdAlliancehistoryGet"></a>
<a id="tocScorporationscorporationidalliancehistoryget"></a>
<a id="tocscorporationscorporationidalliancehistoryget"></a>

```json
[
  {
    "alliance_id": 0,
    "is_deleted": true,
    "record_id": 0,
    "start_date": "2019-08-24T14:15:22Z"
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|alliance_id|integer(int64)|false|none|none|
|is_deleted|boolean|false|none|True if the alliance has been closed|
|record_id|integer(int64)|true|none|An incrementing ID that can be used to canonically establish order of records in cases where dates may be ambiguous|
|start_date|string(date-time)|true|none|none|

<h2 id="tocS_CorporationsCorporationIdAssetsGet">CorporationsCorporationIdAssetsGet</h2>
<!-- backwards compatibility -->
<a id="schemacorporationscorporationidassetsget"></a>
<a id="schema_CorporationsCorporationIdAssetsGet"></a>
<a id="tocScorporationscorporationidassetsget"></a>
<a id="tocscorporationscorporationidassetsget"></a>

```json
[
  {
    "is_blueprint_copy": true,
    "is_singleton": true,
    "item_id": 0,
    "location_flag": "AssetSafety",
    "location_id": 0,
    "location_type": "station",
    "quantity": 0,
    "type_id": 0
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|is_blueprint_copy|boolean|false|none|none|
|is_singleton|boolean|true|none|none|
|item_id|integer(int64)|true|none|none|
|location_flag|string|true|none|none|
|location_id|integer(int64)|true|none|none|
|location_type|string|true|none|none|
|quantity|integer(int64)|true|none|none|
|type_id|integer(int64)|true|none|none|

#### Enumerated Values

|Property|Value|
|---|---|
|location_flag|AssetSafety|
|location_flag|AutoFit|
|location_flag|Bonus|
|location_flag|Booster|
|location_flag|BoosterBay|
|location_flag|Capsule|
|location_flag|CapsuleerDeliveries|
|location_flag|Cargo|
|location_flag|CorpDeliveries|
|location_flag|CorpSAG1|
|location_flag|CorpSAG2|
|location_flag|CorpSAG3|
|location_flag|CorpSAG4|
|location_flag|CorpSAG5|
|location_flag|CorpSAG6|
|location_flag|CorpSAG7|
|location_flag|CorporationGoalDeliveries|
|location_flag|CrateLoot|
|location_flag|Deliveries|
|location_flag|DroneBay|
|location_flag|DustBattle|
|location_flag|DustDatabank|
|location_flag|ExpeditionHold|
|location_flag|FighterBay|
|location_flag|FighterTube0|
|location_flag|FighterTube1|
|location_flag|FighterTube2|
|location_flag|FighterTube3|
|location_flag|FighterTube4|
|location_flag|FleetHangar|
|location_flag|FrigateEscapeBay|
|location_flag|Hangar|
|location_flag|HangarAll|
|location_flag|HiSlot0|
|location_flag|HiSlot1|
|location_flag|HiSlot2|
|location_flag|HiSlot3|
|location_flag|HiSlot4|
|location_flag|HiSlot5|
|location_flag|HiSlot6|
|location_flag|HiSlot7|
|location_flag|HiddenModifiers|
|location_flag|Implant|
|location_flag|Impounded|
|location_flag|InfrastructureHangar|
|location_flag|JunkyardReprocessed|
|location_flag|JunkyardTrashed|
|location_flag|LoSlot0|
|location_flag|LoSlot1|
|location_flag|LoSlot2|
|location_flag|LoSlot3|
|location_flag|LoSlot4|
|location_flag|LoSlot5|
|location_flag|LoSlot6|
|location_flag|LoSlot7|
|location_flag|Locked|
|location_flag|MedSlot0|
|location_flag|MedSlot1|
|location_flag|MedSlot2|
|location_flag|MedSlot3|
|location_flag|MedSlot4|
|location_flag|MedSlot5|
|location_flag|MedSlot6|
|location_flag|MedSlot7|
|location_flag|MobileDepotHold|
|location_flag|MoonMaterialBay|
|location_flag|OfficeFolder|
|location_flag|Pilot|
|location_flag|PlanetSurface|
|location_flag|QuafeBay|
|location_flag|QuantumCoreRoom|
|location_flag|Reward|
|location_flag|RigSlot0|
|location_flag|RigSlot1|
|location_flag|RigSlot2|
|location_flag|RigSlot3|
|location_flag|RigSlot4|
|location_flag|RigSlot5|
|location_flag|RigSlot6|
|location_flag|RigSlot7|
|location_flag|SecondaryStorage|
|location_flag|ServiceSlot0|
|location_flag|ServiceSlot1|
|location_flag|ServiceSlot2|
|location_flag|ServiceSlot3|
|location_flag|ServiceSlot4|
|location_flag|ServiceSlot5|
|location_flag|ServiceSlot6|
|location_flag|ServiceSlot7|
|location_flag|ShipHangar|
|location_flag|ShipOffline|
|location_flag|Skill|
|location_flag|SkillInTraining|
|location_flag|SpecializedAmmoHold|
|location_flag|SpecializedAsteroidHold|
|location_flag|SpecializedCommandCenterHold|
|location_flag|SpecializedFuelBay|
|location_flag|SpecializedGasHold|
|location_flag|SpecializedIceHold|
|location_flag|SpecializedIndustrialShipHold|
|location_flag|SpecializedLargeShipHold|
|location_flag|SpecializedMaterialBay|
|location_flag|SpecializedMediumShipHold|
|location_flag|SpecializedMineralHold|
|location_flag|SpecializedOreHold|
|location_flag|SpecializedPlanetaryCommoditiesHold|
|location_flag|SpecializedSalvageHold|
|location_flag|SpecializedShipHold|
|location_flag|SpecializedSmallShipHold|
|location_flag|StructureActive|
|location_flag|StructureFuel|
|location_flag|StructureInactive|
|location_flag|StructureOffline|
|location_flag|SubSystemBay|
|location_flag|SubSystemSlot0|
|location_flag|SubSystemSlot1|
|location_flag|SubSystemSlot2|
|location_flag|SubSystemSlot3|
|location_flag|SubSystemSlot4|
|location_flag|SubSystemSlot5|
|location_flag|SubSystemSlot6|
|location_flag|SubSystemSlot7|
|location_flag|Unlocked|
|location_flag|Wallet|
|location_flag|Wardrobe|
|location_type|station|
|location_type|solar_system|
|location_type|item|
|location_type|other|

<h2 id="tocS_CorporationsCorporationIdAssetsLocationsPost">CorporationsCorporationIdAssetsLocationsPost</h2>
<!-- backwards compatibility -->
<a id="schemacorporationscorporationidassetslocationspost"></a>
<a id="schema_CorporationsCorporationIdAssetsLocationsPost"></a>
<a id="tocScorporationscorporationidassetslocationspost"></a>
<a id="tocscorporationscorporationidassetslocationspost"></a>

```json
[
  {
    "item_id": 0,
    "position": {
      "x": 0.1,
      "y": 0.1,
      "z": 0.1
    }
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|item_id|integer(int64)|true|none|none|
|position|object|true|none|none|
|» x|number(double)|true|none|none|
|» y|number(double)|true|none|none|
|» z|number(double)|true|none|none|

<h2 id="tocS_CorporationsCorporationIdAssetsNamesPost">CorporationsCorporationIdAssetsNamesPost</h2>
<!-- backwards compatibility -->
<a id="schemacorporationscorporationidassetsnamespost"></a>
<a id="schema_CorporationsCorporationIdAssetsNamesPost"></a>
<a id="tocScorporationscorporationidassetsnamespost"></a>
<a id="tocscorporationscorporationidassetsnamespost"></a>

```json
[
  {
    "item_id": 0,
    "name": "string"
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|item_id|integer(int64)|true|none|none|
|name|string|true|none|none|

<h2 id="tocS_CorporationsCorporationIdBlueprintsGet">CorporationsCorporationIdBlueprintsGet</h2>
<!-- backwards compatibility -->
<a id="schemacorporationscorporationidblueprintsget"></a>
<a id="schema_CorporationsCorporationIdBlueprintsGet"></a>
<a id="tocScorporationscorporationidblueprintsget"></a>
<a id="tocscorporationscorporationidblueprintsget"></a>

```json
[
  {
    "item_id": 0,
    "location_flag": "AssetSafety",
    "location_id": 0,
    "material_efficiency": 0,
    "quantity": 0,
    "runs": 0,
    "time_efficiency": 0,
    "type_id": 0
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|item_id|integer(int64)|true|none|Unique ID for this item.|
|location_flag|string|true|none|Type of the location_id|
|location_id|integer(int64)|true|none|References a station, a ship or an item_id if this blueprint is located within a container.|
|material_efficiency|integer(int64)|true|none|Material Efficiency Level of the blueprint.|
|quantity|integer(int64)|true|none|A range of numbers with a minimum of -2 and no maximum value where -1 is an original and -2 is a copy. It can be a positive integer if it is a stack of blueprint originals fresh from the market (e.g. no activities performed on them yet).|
|runs|integer(int64)|true|none|Number of runs remaining if the blueprint is a copy, -1 if it is an original.|
|time_efficiency|integer(int64)|true|none|Time Efficiency Level of the blueprint.|
|type_id|integer(int64)|true|none|none|

#### Enumerated Values

|Property|Value|
|---|---|
|location_flag|AssetSafety|
|location_flag|AutoFit|
|location_flag|Bonus|
|location_flag|Booster|
|location_flag|BoosterBay|
|location_flag|Capsule|
|location_flag|CapsuleerDeliveries|
|location_flag|Cargo|
|location_flag|CorpDeliveries|
|location_flag|CorpSAG1|
|location_flag|CorpSAG2|
|location_flag|CorpSAG3|
|location_flag|CorpSAG4|
|location_flag|CorpSAG5|
|location_flag|CorpSAG6|
|location_flag|CorpSAG7|
|location_flag|CorporationGoalDeliveries|
|location_flag|CrateLoot|
|location_flag|Deliveries|
|location_flag|DroneBay|
|location_flag|DustBattle|
|location_flag|DustDatabank|
|location_flag|ExpeditionHold|
|location_flag|FighterBay|
|location_flag|FighterTube0|
|location_flag|FighterTube1|
|location_flag|FighterTube2|
|location_flag|FighterTube3|
|location_flag|FighterTube4|
|location_flag|FleetHangar|
|location_flag|FrigateEscapeBay|
|location_flag|Hangar|
|location_flag|HangarAll|
|location_flag|HiSlot0|
|location_flag|HiSlot1|
|location_flag|HiSlot2|
|location_flag|HiSlot3|
|location_flag|HiSlot4|
|location_flag|HiSlot5|
|location_flag|HiSlot6|
|location_flag|HiSlot7|
|location_flag|HiddenModifiers|
|location_flag|Implant|
|location_flag|Impounded|
|location_flag|InfrastructureHangar|
|location_flag|JunkyardReprocessed|
|location_flag|JunkyardTrashed|
|location_flag|LoSlot0|
|location_flag|LoSlot1|
|location_flag|LoSlot2|
|location_flag|LoSlot3|
|location_flag|LoSlot4|
|location_flag|LoSlot5|
|location_flag|LoSlot6|
|location_flag|LoSlot7|
|location_flag|Locked|
|location_flag|MedSlot0|
|location_flag|MedSlot1|
|location_flag|MedSlot2|
|location_flag|MedSlot3|
|location_flag|MedSlot4|
|location_flag|MedSlot5|
|location_flag|MedSlot6|
|location_flag|MedSlot7|
|location_flag|MobileDepotHold|
|location_flag|MoonMaterialBay|
|location_flag|OfficeFolder|
|location_flag|Pilot|
|location_flag|PlanetSurface|
|location_flag|QuafeBay|
|location_flag|QuantumCoreRoom|
|location_flag|Reward|
|location_flag|RigSlot0|
|location_flag|RigSlot1|
|location_flag|RigSlot2|
|location_flag|RigSlot3|
|location_flag|RigSlot4|
|location_flag|RigSlot5|
|location_flag|RigSlot6|
|location_flag|RigSlot7|
|location_flag|SecondaryStorage|
|location_flag|ServiceSlot0|
|location_flag|ServiceSlot1|
|location_flag|ServiceSlot2|
|location_flag|ServiceSlot3|
|location_flag|ServiceSlot4|
|location_flag|ServiceSlot5|
|location_flag|ServiceSlot6|
|location_flag|ServiceSlot7|
|location_flag|ShipHangar|
|location_flag|ShipOffline|
|location_flag|Skill|
|location_flag|SkillInTraining|
|location_flag|SpecializedAmmoHold|
|location_flag|SpecializedAsteroidHold|
|location_flag|SpecializedCommandCenterHold|
|location_flag|SpecializedFuelBay|
|location_flag|SpecializedGasHold|
|location_flag|SpecializedIceHold|
|location_flag|SpecializedIndustrialShipHold|
|location_flag|SpecializedLargeShipHold|
|location_flag|SpecializedMaterialBay|
|location_flag|SpecializedMediumShipHold|
|location_flag|SpecializedMineralHold|
|location_flag|SpecializedOreHold|
|location_flag|SpecializedPlanetaryCommoditiesHold|
|location_flag|SpecializedSalvageHold|
|location_flag|SpecializedShipHold|
|location_flag|SpecializedSmallShipHold|
|location_flag|StructureActive|
|location_flag|StructureFuel|
|location_flag|StructureInactive|
|location_flag|StructureOffline|
|location_flag|SubSystemBay|
|location_flag|SubSystemSlot0|
|location_flag|SubSystemSlot1|
|location_flag|SubSystemSlot2|
|location_flag|SubSystemSlot3|
|location_flag|SubSystemSlot4|
|location_flag|SubSystemSlot5|
|location_flag|SubSystemSlot6|
|location_flag|SubSystemSlot7|
|location_flag|Unlocked|
|location_flag|Wallet|
|location_flag|Wardrobe|

<h2 id="tocS_CorporationsCorporationIdContactsGet">CorporationsCorporationIdContactsGet</h2>
<!-- backwards compatibility -->
<a id="schemacorporationscorporationidcontactsget"></a>
<a id="schema_CorporationsCorporationIdContactsGet"></a>
<a id="tocScorporationscorporationidcontactsget"></a>
<a id="tocscorporationscorporationidcontactsget"></a>

```json
[
  {
    "contact_id": 0,
    "contact_type": "character",
    "is_watched": true,
    "label_ids": [
      0
    ],
    "standing": 0.1
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|contact_id|integer(int64)|true|none|none|
|contact_type|string|true|none|none|
|is_watched|boolean|false|none|Whether this contact is being watched|
|label_ids|[integer]|false|none|none|
|standing|number(double)|true|none|Standing of the contact|

#### Enumerated Values

|Property|Value|
|---|---|
|contact_type|character|
|contact_type|corporation|
|contact_type|alliance|
|contact_type|faction|

<h2 id="tocS_CorporationsCorporationIdContactsLabelsGet">CorporationsCorporationIdContactsLabelsGet</h2>
<!-- backwards compatibility -->
<a id="schemacorporationscorporationidcontactslabelsget"></a>
<a id="schema_CorporationsCorporationIdContactsLabelsGet"></a>
<a id="tocScorporationscorporationidcontactslabelsget"></a>
<a id="tocscorporationscorporationidcontactslabelsget"></a>

```json
[
  {
    "label_id": 0,
    "label_name": "string"
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|label_id|integer(int64)|true|none|none|
|label_name|string|true|none|none|

<h2 id="tocS_CorporationsCorporationIdContainersLogsGet">CorporationsCorporationIdContainersLogsGet</h2>
<!-- backwards compatibility -->
<a id="schemacorporationscorporationidcontainerslogsget"></a>
<a id="schema_CorporationsCorporationIdContainersLogsGet"></a>
<a id="tocScorporationscorporationidcontainerslogsget"></a>
<a id="tocscorporationscorporationidcontainerslogsget"></a>

```json
[
  {
    "action": "add",
    "character_id": 0,
    "container_id": 0,
    "container_type_id": 0,
    "location_flag": "AssetSafety",
    "location_id": 0,
    "logged_at": "2019-08-24T14:15:22Z",
    "new_config_bitmask": 0,
    "old_config_bitmask": 0,
    "password_type": "config",
    "quantity": 0,
    "type_id": 0
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|action|string|true|none|none|
|character_id|integer(int64)|true|none|ID of the character who performed the action.|
|container_id|integer(int64)|true|none|ID of the container|
|container_type_id|integer(int64)|true|none|Type ID of the container|
|location_flag|string|true|none|none|
|location_id|integer(int64)|true|none|none|
|logged_at|string(date-time)|true|none|Timestamp when this log was created|
|new_config_bitmask|integer(int64)|false|none|none|
|old_config_bitmask|integer(int64)|false|none|none|
|password_type|string|false|none|Type of password set if action is of type SetPassword or EnterPassword|
|quantity|integer(int64)|false|none|Quantity of the item being acted upon|
|type_id|integer(int64)|false|none|Type ID of the item being acted upon|

#### Enumerated Values

|Property|Value|
|---|---|
|action|add|
|action|assemble|
|action|configure|
|action|enter_password|
|action|lock|
|action|move|
|action|repackage|
|action|set_name|
|action|set_password|
|action|unlock|
|location_flag|AssetSafety|
|location_flag|AutoFit|
|location_flag|Bonus|
|location_flag|Booster|
|location_flag|BoosterBay|
|location_flag|Capsule|
|location_flag|CapsuleerDeliveries|
|location_flag|Cargo|
|location_flag|CorpDeliveries|
|location_flag|CorpSAG1|
|location_flag|CorpSAG2|
|location_flag|CorpSAG3|
|location_flag|CorpSAG4|
|location_flag|CorpSAG5|
|location_flag|CorpSAG6|
|location_flag|CorpSAG7|
|location_flag|CorporationGoalDeliveries|
|location_flag|CrateLoot|
|location_flag|Deliveries|
|location_flag|DroneBay|
|location_flag|DustBattle|
|location_flag|DustDatabank|
|location_flag|ExpeditionHold|
|location_flag|FighterBay|
|location_flag|FighterTube0|
|location_flag|FighterTube1|
|location_flag|FighterTube2|
|location_flag|FighterTube3|
|location_flag|FighterTube4|
|location_flag|FleetHangar|
|location_flag|FrigateEscapeBay|
|location_flag|Hangar|
|location_flag|HangarAll|
|location_flag|HiSlot0|
|location_flag|HiSlot1|
|location_flag|HiSlot2|
|location_flag|HiSlot3|
|location_flag|HiSlot4|
|location_flag|HiSlot5|
|location_flag|HiSlot6|
|location_flag|HiSlot7|
|location_flag|HiddenModifiers|
|location_flag|Implant|
|location_flag|Impounded|
|location_flag|InfrastructureHangar|
|location_flag|JunkyardReprocessed|
|location_flag|JunkyardTrashed|
|location_flag|LoSlot0|
|location_flag|LoSlot1|
|location_flag|LoSlot2|
|location_flag|LoSlot3|
|location_flag|LoSlot4|
|location_flag|LoSlot5|
|location_flag|LoSlot6|
|location_flag|LoSlot7|
|location_flag|Locked|
|location_flag|MedSlot0|
|location_flag|MedSlot1|
|location_flag|MedSlot2|
|location_flag|MedSlot3|
|location_flag|MedSlot4|
|location_flag|MedSlot5|
|location_flag|MedSlot6|
|location_flag|MedSlot7|
|location_flag|MobileDepotHold|
|location_flag|MoonMaterialBay|
|location_flag|OfficeFolder|
|location_flag|Pilot|
|location_flag|PlanetSurface|
|location_flag|QuafeBay|
|location_flag|QuantumCoreRoom|
|location_flag|Reward|
|location_flag|RigSlot0|
|location_flag|RigSlot1|
|location_flag|RigSlot2|
|location_flag|RigSlot3|
|location_flag|RigSlot4|
|location_flag|RigSlot5|
|location_flag|RigSlot6|
|location_flag|RigSlot7|
|location_flag|SecondaryStorage|
|location_flag|ServiceSlot0|
|location_flag|ServiceSlot1|
|location_flag|ServiceSlot2|
|location_flag|ServiceSlot3|
|location_flag|ServiceSlot4|
|location_flag|ServiceSlot5|
|location_flag|ServiceSlot6|
|location_flag|ServiceSlot7|
|location_flag|ShipHangar|
|location_flag|ShipOffline|
|location_flag|Skill|
|location_flag|SkillInTraining|
|location_flag|SpecializedAmmoHold|
|location_flag|SpecializedAsteroidHold|
|location_flag|SpecializedCommandCenterHold|
|location_flag|SpecializedFuelBay|
|location_flag|SpecializedGasHold|
|location_flag|SpecializedIceHold|
|location_flag|SpecializedIndustrialShipHold|
|location_flag|SpecializedLargeShipHold|
|location_flag|SpecializedMaterialBay|
|location_flag|SpecializedMediumShipHold|
|location_flag|SpecializedMineralHold|
|location_flag|SpecializedOreHold|
|location_flag|SpecializedPlanetaryCommoditiesHold|
|location_flag|SpecializedSalvageHold|
|location_flag|SpecializedShipHold|
|location_flag|SpecializedSmallShipHold|
|location_flag|StructureActive|
|location_flag|StructureFuel|
|location_flag|StructureInactive|
|location_flag|StructureOffline|
|location_flag|SubSystemBay|
|location_flag|SubSystemSlot0|
|location_flag|SubSystemSlot1|
|location_flag|SubSystemSlot2|
|location_flag|SubSystemSlot3|
|location_flag|SubSystemSlot4|
|location_flag|SubSystemSlot5|
|location_flag|SubSystemSlot6|
|location_flag|SubSystemSlot7|
|location_flag|Unlocked|
|location_flag|Wallet|
|location_flag|Wardrobe|
|password_type|config|
|password_type|general|

<h2 id="tocS_CorporationsCorporationIdContractsContractIdBidsGet">CorporationsCorporationIdContractsContractIdBidsGet</h2>
<!-- backwards compatibility -->
<a id="schemacorporationscorporationidcontractscontractidbidsget"></a>
<a id="schema_CorporationsCorporationIdContractsContractIdBidsGet"></a>
<a id="tocScorporationscorporationidcontractscontractidbidsget"></a>
<a id="tocscorporationscorporationidcontractscontractidbidsget"></a>

```json
[
  {
    "amount": 0.1,
    "bid_id": 0,
    "bidder_id": 0,
    "date_bid": "2019-08-24T14:15:22Z"
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|amount|number(double)|true|none|The amount bid, in ISK|
|bid_id|integer(int64)|true|none|Unique ID for the bid|
|bidder_id|integer(int64)|true|none|Character ID of the bidder|
|date_bid|string(date-time)|true|none|Datetime when the bid was placed|

<h2 id="tocS_CorporationsCorporationIdContractsContractIdItemsGet">CorporationsCorporationIdContractsContractIdItemsGet</h2>
<!-- backwards compatibility -->
<a id="schemacorporationscorporationidcontractscontractiditemsget"></a>
<a id="schema_CorporationsCorporationIdContractsContractIdItemsGet"></a>
<a id="tocScorporationscorporationidcontractscontractiditemsget"></a>
<a id="tocscorporationscorporationidcontractscontractiditemsget"></a>

```json
[
  {
    "is_included": true,
    "is_singleton": true,
    "quantity": 0,
    "raw_quantity": 0,
    "record_id": 0,
    "type_id": 0
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|is_included|boolean|true|none|true if the contract issuer has submitted this item with the contract, false if the isser is asking for this item in the contract|
|is_singleton|boolean|true|none|none|
|quantity|integer(int64)|true|none|Number of items in the stack|
|raw_quantity|integer(int64)|false|none|-1 indicates that the item is a singleton (non-stackable). If the item happens to be a Blueprint, -1 is an Original and -2 is a Blueprint Copy|
|record_id|integer(int64)|true|none|Unique ID for the item|
|type_id|integer(int64)|true|none|Type ID for item|

<h2 id="tocS_CorporationsCorporationIdContractsGet">CorporationsCorporationIdContractsGet</h2>
<!-- backwards compatibility -->
<a id="schemacorporationscorporationidcontractsget"></a>
<a id="schema_CorporationsCorporationIdContractsGet"></a>
<a id="tocScorporationscorporationidcontractsget"></a>
<a id="tocscorporationscorporationidcontractsget"></a>

```json
[
  {
    "acceptor_id": 0,
    "assignee_id": 0,
    "availability": "public",
    "buyout": 0.1,
    "collateral": 0.1,
    "contract_id": 0,
    "date_accepted": "2019-08-24T14:15:22Z",
    "date_completed": "2019-08-24T14:15:22Z",
    "date_expired": "2019-08-24T14:15:22Z",
    "date_issued": "2019-08-24T14:15:22Z",
    "days_to_complete": 0,
    "end_location_id": 0,
    "for_corporation": true,
    "issuer_corporation_id": 0,
    "issuer_id": 0,
    "price": 0.1,
    "reward": 0.1,
    "start_location_id": 0,
    "status": "outstanding",
    "title": "string",
    "type": "unknown",
    "volume": 0.1
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|acceptor_id|integer(int64)|true|none|Who will accept the contract|
|assignee_id|integer(int64)|true|none|ID to whom the contract is assigned, can be corporation or character ID|
|availability|string|true|none|To whom the contract is available|
|buyout|number(double)|false|none|Buyout price (for Auctions only)|
|collateral|number(double)|false|none|Collateral price (for Couriers only)|
|contract_id|integer(int64)|true|none|none|
|date_accepted|string(date-time)|false|none|Date of confirmation of contract|
|date_completed|string(date-time)|false|none|Date of completed of contract|
|date_expired|string(date-time)|true|none|Expiration date of the contract|
|date_issued|string(date-time)|true|none|Сreation date of the contract|
|days_to_complete|integer(int64)|false|none|Number of days to perform the contract|
|end_location_id|integer(int64)|false|none|End location ID (for Couriers contract)|
|for_corporation|boolean|true|none|true if the contract was issued on behalf of the issuer's corporation|
|issuer_corporation_id|integer(int64)|true|none|Character's corporation ID for the issuer|
|issuer_id|integer(int64)|true|none|Character ID for the issuer|
|price|number(double)|false|none|Price of contract (for ItemsExchange and Auctions)|
|reward|number(double)|false|none|Remuneration for contract (for Couriers only)|
|start_location_id|integer(int64)|false|none|Start location ID (for Couriers contract)|
|status|string|true|none|Status of the the contract|
|title|string|false|none|Title of the contract|
|type|string|true|none|Type of the contract|
|volume|number(double)|false|none|Volume of items in the contract|

#### Enumerated Values

|Property|Value|
|---|---|
|availability|public|
|availability|personal|
|availability|corporation|
|availability|alliance|
|status|outstanding|
|status|in_progress|
|status|finished_issuer|
|status|finished_contractor|
|status|finished|
|status|cancelled|
|status|rejected|
|status|failed|
|status|deleted|
|status|reversed|
|type|unknown|
|type|item_exchange|
|type|auction|
|type|courier|
|type|loan|

<h2 id="tocS_CorporationsCorporationIdCustomsOfficesGet">CorporationsCorporationIdCustomsOfficesGet</h2>
<!-- backwards compatibility -->
<a id="schemacorporationscorporationidcustomsofficesget"></a>
<a id="schema_CorporationsCorporationIdCustomsOfficesGet"></a>
<a id="tocScorporationscorporationidcustomsofficesget"></a>
<a id="tocscorporationscorporationidcustomsofficesget"></a>

```json
[
  {
    "alliance_tax_rate": 0.1,
    "allow_access_with_standings": true,
    "allow_alliance_access": true,
    "bad_standing_tax_rate": 0.1,
    "corporation_tax_rate": 0.1,
    "excellent_standing_tax_rate": 0.1,
    "good_standing_tax_rate": 0.1,
    "neutral_standing_tax_rate": 0.1,
    "office_id": 0,
    "reinforce_exit_end": 0,
    "reinforce_exit_start": 0,
    "standing_level": "bad",
    "system_id": 0,
    "terrible_standing_tax_rate": 0.1
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|alliance_tax_rate|number(double)|false|none|Only present if alliance access is allowed|
|allow_access_with_standings|boolean|true|none|standing_level and any standing related tax rate only present when this is true|
|allow_alliance_access|boolean|true|none|none|
|bad_standing_tax_rate|number(double)|false|none|none|
|corporation_tax_rate|number(double)|false|none|none|
|excellent_standing_tax_rate|number(double)|false|none|Tax rate for entities with excellent level of standing, only present if this level is allowed, same for all other standing related tax rates|
|good_standing_tax_rate|number(double)|false|none|none|
|neutral_standing_tax_rate|number(double)|false|none|none|
|office_id|integer(int64)|true|none|unique ID of this customs office|
|reinforce_exit_end|integer(int64)|true|none|none|
|reinforce_exit_start|integer(int64)|true|none|Together with reinforce_exit_end, marks a 2-hour period where this customs office could exit reinforcement mode during the day after initial attack|
|standing_level|string|false|none|Access is allowed only for entities with this level of standing or better|
|system_id|integer(int64)|true|none|ID of the solar system this customs office is located in|
|terrible_standing_tax_rate|number(double)|false|none|none|

#### Enumerated Values

|Property|Value|
|---|---|
|standing_level|bad|
|standing_level|excellent|
|standing_level|good|
|standing_level|neutral|
|standing_level|terrible|

<h2 id="tocS_CorporationsCorporationIdDivisionsGet">CorporationsCorporationIdDivisionsGet</h2>
<!-- backwards compatibility -->
<a id="schemacorporationscorporationiddivisionsget"></a>
<a id="schema_CorporationsCorporationIdDivisionsGet"></a>
<a id="tocScorporationscorporationiddivisionsget"></a>
<a id="tocscorporationscorporationiddivisionsget"></a>

```json
{
  "hangar": [
    {
      "division": 0,
      "name": "string"
    }
  ],
  "wallet": [
    {
      "division": 0,
      "name": "string"
    }
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|hangar|[object]|false|none|none|
|» division|integer(int64)|false|none|none|
|» name|string|false|none|none|
|wallet|[object]|false|none|none|
|» division|integer(int64)|false|none|none|
|» name|string|false|none|none|

<h2 id="tocS_CorporationsCorporationIdFacilitiesGet">CorporationsCorporationIdFacilitiesGet</h2>
<!-- backwards compatibility -->
<a id="schemacorporationscorporationidfacilitiesget"></a>
<a id="schema_CorporationsCorporationIdFacilitiesGet"></a>
<a id="tocScorporationscorporationidfacilitiesget"></a>
<a id="tocscorporationscorporationidfacilitiesget"></a>

```json
[
  {
    "facility_id": 0,
    "system_id": 0,
    "type_id": 0
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|facility_id|integer(int64)|true|none|none|
|system_id|integer(int64)|true|none|none|
|type_id|integer(int64)|true|none|none|

<h2 id="tocS_CorporationsCorporationIdFwStatsGet">CorporationsCorporationIdFwStatsGet</h2>
<!-- backwards compatibility -->
<a id="schemacorporationscorporationidfwstatsget"></a>
<a id="schema_CorporationsCorporationIdFwStatsGet"></a>
<a id="tocScorporationscorporationidfwstatsget"></a>
<a id="tocscorporationscorporationidfwstatsget"></a>

```json
{
  "enlisted_on": "2019-08-24T14:15:22Z",
  "faction_id": 0,
  "kills": {
    "last_week": 0,
    "total": 0,
    "yesterday": 0
  },
  "pilots": 0,
  "victory_points": {
    "last_week": 0,
    "total": 0,
    "yesterday": 0
  }
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|enlisted_on|string(date-time)|false|none|The enlistment date of the given corporation into faction warfare. Will not be included if corporation is not enlisted in faction warfare|
|faction_id|integer(int64)|false|none|The faction the given corporation is enlisted to fight for. Will not be included if corporation is not enlisted in faction warfare|
|kills|object|true|none|Summary of kills done by the given corporation against enemy factions|
|» last_week|integer(int64)|true|none|Last week's total number of kills by members of the given corporation against enemy factions|
|» total|integer(int64)|true|none|Total number of kills by members of the given corporation against enemy factions since the corporation enlisted|
|» yesterday|integer(int64)|true|none|Yesterday's total number of kills by members of the given corporation against enemy factions|
|pilots|integer(int64)|false|none|How many pilots the enlisted corporation has. Will not be included if corporation is not enlisted in faction warfare|
|victory_points|object|true|none|Summary of victory points gained by the given corporation for the enlisted faction|
|» last_week|integer(int64)|true|none|Last week's victory points gained by members of the given corporation|
|» total|integer(int64)|true|none|Total victory points gained since the given corporation enlisted|
|» yesterday|integer(int64)|true|none|Yesterday's victory points gained by members of the given corporation|

<h2 id="tocS_CorporationsCorporationIdGet">CorporationsCorporationIdGet</h2>
<!-- backwards compatibility -->
<a id="schemacorporationscorporationidget"></a>
<a id="schema_CorporationsCorporationIdGet"></a>
<a id="tocScorporationscorporationidget"></a>
<a id="tocscorporationscorporationidget"></a>

```json
{
  "alliance_id": 0,
  "ceo_id": 0,
  "creator_id": 0,
  "date_founded": "2019-08-24T14:15:22Z",
  "description": "string",
  "faction_id": 0,
  "home_station_id": 0,
  "member_count": 0,
  "name": "string",
  "shares": 0,
  "tax_rate": 0.1,
  "ticker": "string",
  "url": "string",
  "war_eligible": true
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|alliance_id|integer(int64)|false|none|ID of the alliance that corporation is a member of, if any|
|ceo_id|integer(int64)|true|none|none|
|creator_id|integer(int64)|true|none|none|
|date_founded|string(date-time)|false|none|none|
|description|string|false|none|none|
|faction_id|integer(int64)|false|none|none|
|home_station_id|integer(int64)|false|none|none|
|member_count|integer(int64)|true|none|none|
|name|string|true|none|the full name of the corporation|
|shares|integer(int64)|false|none|none|
|tax_rate|number(double)|true|none|none|
|ticker|string|true|none|the short name of the corporation|
|url|string|false|none|none|
|war_eligible|boolean|false|none|none|

<h2 id="tocS_CorporationsCorporationIdIconsGet">CorporationsCorporationIdIconsGet</h2>
<!-- backwards compatibility -->
<a id="schemacorporationscorporationidiconsget"></a>
<a id="schema_CorporationsCorporationIdIconsGet"></a>
<a id="tocScorporationscorporationidiconsget"></a>
<a id="tocscorporationscorporationidiconsget"></a>

```json
{
  "px128x128": "string",
  "px256x256": "string",
  "px64x64": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|px128x128|string|false|none|none|
|px256x256|string|false|none|none|
|px64x64|string|false|none|none|

<h2 id="tocS_CorporationsCorporationIdIndustryJobsGet">CorporationsCorporationIdIndustryJobsGet</h2>
<!-- backwards compatibility -->
<a id="schemacorporationscorporationidindustryjobsget"></a>
<a id="schema_CorporationsCorporationIdIndustryJobsGet"></a>
<a id="tocScorporationscorporationidindustryjobsget"></a>
<a id="tocscorporationscorporationidindustryjobsget"></a>

```json
[
  {
    "activity_id": 0,
    "blueprint_id": 0,
    "blueprint_location_id": 0,
    "blueprint_type_id": 0,
    "completed_character_id": 0,
    "completed_date": "2019-08-24T14:15:22Z",
    "cost": 0.1,
    "duration": 0,
    "end_date": "2019-08-24T14:15:22Z",
    "facility_id": 0,
    "installer_id": 0,
    "job_id": 0,
    "licensed_runs": 0,
    "location_id": 0,
    "output_location_id": 0,
    "pause_date": "2019-08-24T14:15:22Z",
    "probability": 0.1,
    "product_type_id": 0,
    "runs": 0,
    "start_date": "2019-08-24T14:15:22Z",
    "status": "active",
    "successful_runs": 0
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|activity_id|integer(int64)|true|none|Job activity ID|
|blueprint_id|integer(int64)|true|none|none|
|blueprint_location_id|integer(int64)|true|none|Location ID of the location from which the blueprint was installed. Normally a station ID, but can also be an asset (e.g. container) or corporation facility|
|blueprint_type_id|integer(int64)|true|none|none|
|completed_character_id|integer(int64)|false|none|ID of the character which completed this job|
|completed_date|string(date-time)|false|none|Date and time when this job was completed|
|cost|number(double)|false|none|The sume of job installation fee and industry facility tax|
|duration|integer(int64)|true|none|Job duration in seconds|
|end_date|string(date-time)|true|none|Date and time when this job finished|
|facility_id|integer(int64)|true|none|ID of the facility where this job is running|
|installer_id|integer(int64)|true|none|ID of the character which installed this job|
|job_id|integer(int64)|true|none|Unique job ID|
|licensed_runs|integer(int64)|false|none|Number of runs blueprint is licensed for|
|location_id|integer(int64)|true|none|ID of the location for the industry facility|
|output_location_id|integer(int64)|true|none|Location ID of the location to which the output of the job will be delivered. Normally a station ID, but can also be a corporation facility|
|pause_date|string(date-time)|false|none|Date and time when this job was paused (i.e. time when the facility where this job was installed went offline)|
|probability|number(double)|false|none|Chance of success for invention|
|product_type_id|integer(int64)|false|none|Type ID of product (manufactured, copied or invented)|
|runs|integer(int64)|true|none|Number of runs for a manufacturing job, or number of copies to make for a blueprint copy|
|start_date|string(date-time)|true|none|Date and time when this job started|
|status|string|true|none|none|
|successful_runs|integer(int64)|false|none|Number of successful runs for this job. Equal to runs unless this is an invention job|

#### Enumerated Values

|Property|Value|
|---|---|
|status|active|
|status|cancelled|
|status|delivered|
|status|paused|
|status|ready|
|status|reverted|

<h2 id="tocS_CorporationsCorporationIdKillmailsRecentGet">CorporationsCorporationIdKillmailsRecentGet</h2>
<!-- backwards compatibility -->
<a id="schemacorporationscorporationidkillmailsrecentget"></a>
<a id="schema_CorporationsCorporationIdKillmailsRecentGet"></a>
<a id="tocScorporationscorporationidkillmailsrecentget"></a>
<a id="tocscorporationscorporationidkillmailsrecentget"></a>

```json
[
  {
    "killmail_hash": "string",
    "killmail_id": 0
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|killmail_hash|string|true|none|A hash of this killmail|
|killmail_id|integer(int64)|true|none|ID of this killmail|

<h2 id="tocS_CorporationsCorporationIdMedalsGet">CorporationsCorporationIdMedalsGet</h2>
<!-- backwards compatibility -->
<a id="schemacorporationscorporationidmedalsget"></a>
<a id="schema_CorporationsCorporationIdMedalsGet"></a>
<a id="tocScorporationscorporationidmedalsget"></a>
<a id="tocscorporationscorporationidmedalsget"></a>

```json
[
  {
    "created_at": "2019-08-24T14:15:22Z",
    "creator_id": 0,
    "description": "string",
    "medal_id": 0,
    "title": "string"
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|created_at|string(date-time)|true|none|none|
|creator_id|integer(int64)|true|none|ID of the character who created this medal|
|description|string|true|none|none|
|medal_id|integer(int64)|true|none|none|
|title|string|true|none|none|

<h2 id="tocS_CorporationsCorporationIdMedalsIssuedGet">CorporationsCorporationIdMedalsIssuedGet</h2>
<!-- backwards compatibility -->
<a id="schemacorporationscorporationidmedalsissuedget"></a>
<a id="schema_CorporationsCorporationIdMedalsIssuedGet"></a>
<a id="tocScorporationscorporationidmedalsissuedget"></a>
<a id="tocscorporationscorporationidmedalsissuedget"></a>

```json
[
  {
    "character_id": 0,
    "issued_at": "2019-08-24T14:15:22Z",
    "issuer_id": 0,
    "medal_id": 0,
    "reason": "string",
    "status": "private"
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|character_id|integer(int64)|true|none|ID of the character who was rewarded this medal|
|issued_at|string(date-time)|true|none|none|
|issuer_id|integer(int64)|true|none|ID of the character who issued the medal|
|medal_id|integer(int64)|true|none|none|
|reason|string|true|none|none|
|status|string|true|none|none|

#### Enumerated Values

|Property|Value|
|---|---|
|status|private|
|status|public|

<h2 id="tocS_CorporationsCorporationIdMembersGet">CorporationsCorporationIdMembersGet</h2>
<!-- backwards compatibility -->
<a id="schemacorporationscorporationidmembersget"></a>
<a id="schema_CorporationsCorporationIdMembersGet"></a>
<a id="tocScorporationscorporationidmembersget"></a>
<a id="tocscorporationscorporationidmembersget"></a>

```json
[
  0
]

```

A list of character IDs

### Properties

*None*

<h2 id="tocS_CorporationsCorporationIdMembersLimitGet">CorporationsCorporationIdMembersLimitGet</h2>
<!-- backwards compatibility -->
<a id="schemacorporationscorporationidmemberslimitget"></a>
<a id="schema_CorporationsCorporationIdMembersLimitGet"></a>
<a id="tocScorporationscorporationidmemberslimitget"></a>
<a id="tocscorporationscorporationidmemberslimitget"></a>

```json
0

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|integer(int64)|false|none|none|

<h2 id="tocS_CorporationsCorporationIdMembersTitlesGet">CorporationsCorporationIdMembersTitlesGet</h2>
<!-- backwards compatibility -->
<a id="schemacorporationscorporationidmemberstitlesget"></a>
<a id="schema_CorporationsCorporationIdMembersTitlesGet"></a>
<a id="tocScorporationscorporationidmemberstitlesget"></a>
<a id="tocscorporationscorporationidmemberstitlesget"></a>

```json
[
  {
    "character_id": 0,
    "titles": [
      0
    ]
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|character_id|integer(int64)|true|none|none|
|titles|[integer]|true|none|A list of title_id|

<h2 id="tocS_CorporationsCorporationIdMembertrackingGet">CorporationsCorporationIdMembertrackingGet</h2>
<!-- backwards compatibility -->
<a id="schemacorporationscorporationidmembertrackingget"></a>
<a id="schema_CorporationsCorporationIdMembertrackingGet"></a>
<a id="tocScorporationscorporationidmembertrackingget"></a>
<a id="tocscorporationscorporationidmembertrackingget"></a>

```json
[
  {
    "base_id": 0,
    "character_id": 0,
    "location_id": 0,
    "logoff_date": "2019-08-24T14:15:22Z",
    "logon_date": "2019-08-24T14:15:22Z",
    "ship_type_id": 0,
    "start_date": "2019-08-24T14:15:22Z"
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|base_id|integer(int64)|false|none|none|
|character_id|integer(int64)|true|none|none|
|location_id|integer(int64)|false|none|none|
|logoff_date|string(date-time)|false|none|none|
|logon_date|string(date-time)|false|none|none|
|ship_type_id|integer(int64)|false|none|none|
|start_date|string(date-time)|false|none|none|

<h2 id="tocS_CorporationsCorporationIdOrdersGet">CorporationsCorporationIdOrdersGet</h2>
<!-- backwards compatibility -->
<a id="schemacorporationscorporationidordersget"></a>
<a id="schema_CorporationsCorporationIdOrdersGet"></a>
<a id="tocScorporationscorporationidordersget"></a>
<a id="tocscorporationscorporationidordersget"></a>

```json
[
  {
    "duration": 0,
    "escrow": 0.1,
    "is_buy_order": true,
    "issued": "2019-08-24T14:15:22Z",
    "issued_by": 0,
    "location_id": 0,
    "min_volume": 0,
    "order_id": 0,
    "price": 0.1,
    "range": "1",
    "region_id": 0,
    "type_id": 0,
    "volume_remain": 0,
    "volume_total": 0,
    "wallet_division": 0
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|duration|integer(int64)|true|none|Number of days for which order is valid (starting from the issued date). An order expires at time issued + duration|
|escrow|number(double)|false|none|For buy orders, the amount of ISK in escrow|
|is_buy_order|boolean|false|none|True if the order is a bid (buy) order|
|issued|string(date-time)|true|none|Date and time when this order was issued|
|issued_by|integer(int64)|true|none|The character who issued this order|
|location_id|integer(int64)|true|none|ID of the location where order was placed|
|min_volume|integer(int64)|false|none|For buy orders, the minimum quantity that will be accepted in a matching sell order|
|order_id|integer(int64)|true|none|Unique order ID|
|price|number(double)|true|none|Cost per unit for this order|
|range|string|true|none|Valid order range, numbers are ranges in jumps|
|region_id|integer(int64)|true|none|ID of the region where order was placed|
|type_id|integer(int64)|true|none|The type ID of the item transacted in this order|
|volume_remain|integer(int64)|true|none|Quantity of items still required or offered|
|volume_total|integer(int64)|true|none|Quantity of items required or offered at time order was placed|
|wallet_division|integer(int64)|true|none|The corporation wallet division used for this order.|

#### Enumerated Values

|Property|Value|
|---|---|
|range|1|
|range|10|
|range|2|
|range|20|
|range|3|
|range|30|
|range|4|
|range|40|
|range|5|
|range|region|
|range|solarsystem|
|range|station|

<h2 id="tocS_CorporationsCorporationIdOrdersHistoryGet">CorporationsCorporationIdOrdersHistoryGet</h2>
<!-- backwards compatibility -->
<a id="schemacorporationscorporationidordershistoryget"></a>
<a id="schema_CorporationsCorporationIdOrdersHistoryGet"></a>
<a id="tocScorporationscorporationidordershistoryget"></a>
<a id="tocscorporationscorporationidordershistoryget"></a>

```json
[
  {
    "duration": 0,
    "escrow": 0.1,
    "is_buy_order": true,
    "issued": "2019-08-24T14:15:22Z",
    "issued_by": 0,
    "location_id": 0,
    "min_volume": 0,
    "order_id": 0,
    "price": 0.1,
    "range": "1",
    "region_id": 0,
    "state": "cancelled",
    "type_id": 0,
    "volume_remain": 0,
    "volume_total": 0,
    "wallet_division": 0
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|duration|integer(int64)|true|none|Number of days the order was valid for (starting from the issued date). An order expires at time issued + duration|
|escrow|number(double)|false|none|For buy orders, the amount of ISK in escrow|
|is_buy_order|boolean|false|none|True if the order is a bid (buy) order|
|issued|string(date-time)|true|none|Date and time when this order was issued|
|issued_by|integer(int64)|false|none|The character who issued this order|
|location_id|integer(int64)|true|none|ID of the location where order was placed|
|min_volume|integer(int64)|false|none|For buy orders, the minimum quantity that will be accepted in a matching sell order|
|order_id|integer(int64)|true|none|Unique order ID|
|price|number(double)|true|none|Cost per unit for this order|
|range|string|true|none|Valid order range, numbers are ranges in jumps|
|region_id|integer(int64)|true|none|ID of the region where order was placed|
|state|string|true|none|Current order state|
|type_id|integer(int64)|true|none|The type ID of the item transacted in this order|
|volume_remain|integer(int64)|true|none|Quantity of items still required or offered|
|volume_total|integer(int64)|true|none|Quantity of items required or offered at time order was placed|
|wallet_division|integer(int64)|true|none|The corporation wallet division used for this order|

#### Enumerated Values

|Property|Value|
|---|---|
|range|1|
|range|10|
|range|2|
|range|20|
|range|3|
|range|30|
|range|4|
|range|40|
|range|5|
|range|region|
|range|solarsystem|
|range|station|
|state|cancelled|
|state|expired|

<h2 id="tocS_CorporationsCorporationIdRolesGet">CorporationsCorporationIdRolesGet</h2>
<!-- backwards compatibility -->
<a id="schemacorporationscorporationidrolesget"></a>
<a id="schema_CorporationsCorporationIdRolesGet"></a>
<a id="tocScorporationscorporationidrolesget"></a>
<a id="tocscorporationscorporationidrolesget"></a>

```json
[
  {
    "character_id": 0,
    "grantable_roles": [
      "Account_Take_1"
    ],
    "grantable_roles_at_base": [
      "Account_Take_1"
    ],
    "grantable_roles_at_hq": [
      "Account_Take_1"
    ],
    "grantable_roles_at_other": [
      "Account_Take_1"
    ],
    "roles": [
      "Account_Take_1"
    ],
    "roles_at_base": [
      "Account_Take_1"
    ],
    "roles_at_hq": [
      "Account_Take_1"
    ],
    "roles_at_other": [
      "Account_Take_1"
    ]
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|character_id|integer(int64)|true|none|none|
|grantable_roles|[string]|false|none|none|
|grantable_roles_at_base|[string]|false|none|none|
|grantable_roles_at_hq|[string]|false|none|none|
|grantable_roles_at_other|[string]|false|none|none|
|roles|[string]|false|none|none|
|roles_at_base|[string]|false|none|none|
|roles_at_hq|[string]|false|none|none|
|roles_at_other|[string]|false|none|none|

<h2 id="tocS_CorporationsCorporationIdRolesHistoryGet">CorporationsCorporationIdRolesHistoryGet</h2>
<!-- backwards compatibility -->
<a id="schemacorporationscorporationidroleshistoryget"></a>
<a id="schema_CorporationsCorporationIdRolesHistoryGet"></a>
<a id="tocScorporationscorporationidroleshistoryget"></a>
<a id="tocscorporationscorporationidroleshistoryget"></a>

```json
[
  {
    "changed_at": "2019-08-24T14:15:22Z",
    "character_id": 0,
    "issuer_id": 0,
    "new_roles": [
      "Account_Take_1"
    ],
    "old_roles": [
      "Account_Take_1"
    ],
    "role_type": "grantable_roles"
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|changed_at|string(date-time)|true|none|none|
|character_id|integer(int64)|true|none|The character whose roles are changed|
|issuer_id|integer(int64)|true|none|ID of the character who issued this change|
|new_roles|[string]|true|none|none|
|old_roles|[string]|true|none|none|
|role_type|string|true|none|none|

#### Enumerated Values

|Property|Value|
|---|---|
|role_type|grantable_roles|
|role_type|grantable_roles_at_base|
|role_type|grantable_roles_at_hq|
|role_type|grantable_roles_at_other|
|role_type|roles|
|role_type|roles_at_base|
|role_type|roles_at_hq|
|role_type|roles_at_other|

<h2 id="tocS_CorporationsCorporationIdShareholdersGet">CorporationsCorporationIdShareholdersGet</h2>
<!-- backwards compatibility -->
<a id="schemacorporationscorporationidshareholdersget"></a>
<a id="schema_CorporationsCorporationIdShareholdersGet"></a>
<a id="tocScorporationscorporationidshareholdersget"></a>
<a id="tocscorporationscorporationidshareholdersget"></a>

```json
[
  {
    "share_count": 0,
    "shareholder_id": 0,
    "shareholder_type": "character"
  }
]

```

List of shareholders

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|share_count|integer(int64)|true|none|none|
|shareholder_id|integer(int64)|true|none|none|
|shareholder_type|string|true|none|none|

#### Enumerated Values

|Property|Value|
|---|---|
|shareholder_type|character|
|shareholder_type|corporation|

<h2 id="tocS_CorporationsCorporationIdStandingsGet">CorporationsCorporationIdStandingsGet</h2>
<!-- backwards compatibility -->
<a id="schemacorporationscorporationidstandingsget"></a>
<a id="schema_CorporationsCorporationIdStandingsGet"></a>
<a id="tocScorporationscorporationidstandingsget"></a>
<a id="tocscorporationscorporationidstandingsget"></a>

```json
[
  {
    "from_id": 0,
    "from_type": "agent",
    "standing": 0.1
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|from_id|integer(int64)|true|none|none|
|from_type|string|true|none|none|
|standing|number(double)|true|none|none|

#### Enumerated Values

|Property|Value|
|---|---|
|from_type|agent|
|from_type|npc_corp|
|from_type|faction|

<h2 id="tocS_CorporationsCorporationIdStarbasesGet">CorporationsCorporationIdStarbasesGet</h2>
<!-- backwards compatibility -->
<a id="schemacorporationscorporationidstarbasesget"></a>
<a id="schema_CorporationsCorporationIdStarbasesGet"></a>
<a id="tocScorporationscorporationidstarbasesget"></a>
<a id="tocscorporationscorporationidstarbasesget"></a>

```json
[
  {
    "moon_id": 0,
    "onlined_since": "2019-08-24T14:15:22Z",
    "reinforced_until": "2019-08-24T14:15:22Z",
    "starbase_id": 0,
    "state": "offline",
    "system_id": 0,
    "type_id": 0,
    "unanchor_at": "2019-08-24T14:15:22Z"
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|moon_id|integer(int64)|false|none|The moon this starbase (POS) is anchored on, unanchored POSes do not have this information|
|onlined_since|string(date-time)|false|none|When the POS onlined, for starbases (POSes) in online state|
|reinforced_until|string(date-time)|false|none|When the POS will be out of reinforcement, for starbases (POSes) in reinforced state|
|starbase_id|integer(int64)|true|none|Unique ID for this starbase (POS)|
|state|string|false|none|none|
|system_id|integer(int64)|true|none|The solar system this starbase (POS) is in, unanchored POSes have this information|
|type_id|integer(int64)|true|none|Starbase (POS) type|
|unanchor_at|string(date-time)|false|none|When the POS started unanchoring, for starbases (POSes) in unanchoring state|

#### Enumerated Values

|Property|Value|
|---|---|
|state|offline|
|state|online|
|state|onlining|
|state|reinforced|
|state|unanchoring|

<h2 id="tocS_CorporationsCorporationIdStarbasesStarbaseIdGet">CorporationsCorporationIdStarbasesStarbaseIdGet</h2>
<!-- backwards compatibility -->
<a id="schemacorporationscorporationidstarbasesstarbaseidget"></a>
<a id="schema_CorporationsCorporationIdStarbasesStarbaseIdGet"></a>
<a id="tocScorporationscorporationidstarbasesstarbaseidget"></a>
<a id="tocscorporationscorporationidstarbasesstarbaseidget"></a>

```json
{
  "allow_alliance_members": true,
  "allow_corporation_members": true,
  "anchor": "alliance_member",
  "attack_if_at_war": true,
  "attack_if_other_security_status_dropping": true,
  "attack_security_status_threshold": 0.1,
  "attack_standing_threshold": 0.1,
  "fuel_bay_take": "alliance_member",
  "fuel_bay_view": "alliance_member",
  "fuels": [
    {
      "quantity": 0,
      "type_id": 0
    }
  ],
  "offline": "alliance_member",
  "online": "alliance_member",
  "unanchor": "alliance_member",
  "use_alliance_standings": true
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|allow_alliance_members|boolean|true|none|none|
|allow_corporation_members|boolean|true|none|none|
|anchor|string|true|none|Who can anchor starbase (POS) and its structures|
|attack_if_at_war|boolean|true|none|none|
|attack_if_other_security_status_dropping|boolean|true|none|none|
|attack_security_status_threshold|number(double)|false|none|Starbase (POS) will attack if target's security standing is lower than this value|
|attack_standing_threshold|number(double)|false|none|Starbase (POS) will attack if target's standing is lower than this value|
|fuel_bay_take|string|true|none|Who can take fuel blocks out of the starbase (POS)'s fuel bay|
|fuel_bay_view|string|true|none|Who can view the starbase (POS)'s fule bay. Characters either need to have required role or belong to the starbase (POS) owner's corporation or alliance, as described by the enum, all other access settings follows the same scheme|
|fuels|[object]|false|none|Fuel blocks and other things that will be consumed when operating a starbase (POS)|
|» quantity|integer(int64)|true|none|none|
|» type_id|integer(int64)|true|none|none|
|offline|string|true|none|Who can offline starbase (POS) and its structures|
|online|string|true|none|Who can online starbase (POS) and its structures|
|unanchor|string|true|none|Who can unanchor starbase (POS) and its structures|
|use_alliance_standings|boolean|true|none|True if the starbase (POS) is using alliance standings, otherwise using corporation's|

#### Enumerated Values

|Property|Value|
|---|---|
|anchor|alliance_member|
|anchor|config_starbase_equipment_role|
|anchor|corporation_member|
|anchor|starbase_fuel_technician_role|
|fuel_bay_take|alliance_member|
|fuel_bay_take|config_starbase_equipment_role|
|fuel_bay_take|corporation_member|
|fuel_bay_take|starbase_fuel_technician_role|
|fuel_bay_view|alliance_member|
|fuel_bay_view|config_starbase_equipment_role|
|fuel_bay_view|corporation_member|
|fuel_bay_view|starbase_fuel_technician_role|
|offline|alliance_member|
|offline|config_starbase_equipment_role|
|offline|corporation_member|
|offline|starbase_fuel_technician_role|
|online|alliance_member|
|online|config_starbase_equipment_role|
|online|corporation_member|
|online|starbase_fuel_technician_role|
|unanchor|alliance_member|
|unanchor|config_starbase_equipment_role|
|unanchor|corporation_member|
|unanchor|starbase_fuel_technician_role|

<h2 id="tocS_CorporationsCorporationIdStructuresGet">CorporationsCorporationIdStructuresGet</h2>
<!-- backwards compatibility -->
<a id="schemacorporationscorporationidstructuresget"></a>
<a id="schema_CorporationsCorporationIdStructuresGet"></a>
<a id="tocScorporationscorporationidstructuresget"></a>
<a id="tocscorporationscorporationidstructuresget"></a>

```json
[
  {
    "corporation_id": 0,
    "fuel_expires": "2019-08-24T14:15:22Z",
    "name": "string",
    "next_reinforce_apply": "2019-08-24T14:15:22Z",
    "next_reinforce_hour": 0,
    "profile_id": 0,
    "reinforce_hour": 0,
    "services": [
      {
        "name": "string",
        "state": "online"
      }
    ],
    "state": "anchor_vulnerable",
    "state_timer_end": "2019-08-24T14:15:22Z",
    "state_timer_start": "2019-08-24T14:15:22Z",
    "structure_id": 0,
    "system_id": 0,
    "type_id": 0,
    "unanchors_at": "2019-08-24T14:15:22Z"
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|corporation_id|integer(int64)|true|none|ID of the corporation that owns the structure|
|fuel_expires|string(date-time)|false|none|Date on which the structure will run out of fuel|
|name|string|false|none|The structure name|
|next_reinforce_apply|string(date-time)|false|none|The date and time when the structure's newly requested reinforcement times (e.g. next_reinforce_hour and next_reinforce_day) will take effect|
|next_reinforce_hour|integer(int64)|false|none|The requested change to reinforce_hour that will take effect at the time shown by next_reinforce_apply|
|profile_id|integer(int64)|true|none|The id of the ACL profile for this citadel|
|reinforce_hour|integer(int64)|false|none|The hour of day that determines the four hour window when the structure will randomly exit its reinforcement periods and become vulnerable to attack against its armor and/or hull. The structure will become vulnerable at a random time that is +/- 2 hours centered on the value of this property|
|services|[object]|false|none|Contains a list of service upgrades, and their state|
|» name|string|true|none|none|
|» state|string|true|none|none|
|state|string|true|none|none|
|state_timer_end|string(date-time)|false|none|Date at which the structure will move to it's next state|
|state_timer_start|string(date-time)|false|none|Date at which the structure entered it's current state|
|structure_id|integer(int64)|true|none|The Item ID of the structure|
|system_id|integer(int64)|true|none|The solar system the structure is in|
|type_id|integer(int64)|true|none|The type id of the structure|
|unanchors_at|string(date-time)|false|none|Date at which the structure will unanchor|

#### Enumerated Values

|Property|Value|
|---|---|
|state|online|
|state|offline|
|state|cleanup|
|state|anchor_vulnerable|
|state|anchoring|
|state|armor_reinforce|
|state|armor_vulnerable|
|state|deploy_vulnerable|
|state|fitting_invulnerable|
|state|hull_reinforce|
|state|hull_vulnerable|
|state|online_deprecated|
|state|onlining_vulnerable|
|state|shield_vulnerable|
|state|unanchored|
|state|unknown|

<h2 id="tocS_CorporationsCorporationIdTitlesGet">CorporationsCorporationIdTitlesGet</h2>
<!-- backwards compatibility -->
<a id="schemacorporationscorporationidtitlesget"></a>
<a id="schema_CorporationsCorporationIdTitlesGet"></a>
<a id="tocScorporationscorporationidtitlesget"></a>
<a id="tocscorporationscorporationidtitlesget"></a>

```json
[
  {
    "grantable_roles": [
      "Account_Take_1"
    ],
    "grantable_roles_at_base": [
      "Account_Take_1"
    ],
    "grantable_roles_at_hq": [
      "Account_Take_1"
    ],
    "grantable_roles_at_other": [
      "Account_Take_1"
    ],
    "name": "string",
    "roles": [
      "Account_Take_1"
    ],
    "roles_at_base": [
      "Account_Take_1"
    ],
    "roles_at_hq": [
      "Account_Take_1"
    ],
    "roles_at_other": [
      "Account_Take_1"
    ],
    "title_id": 0
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|grantable_roles|[string]|false|none|none|
|grantable_roles_at_base|[string]|false|none|none|
|grantable_roles_at_hq|[string]|false|none|none|
|grantable_roles_at_other|[string]|false|none|none|
|name|string|false|none|none|
|roles|[string]|false|none|none|
|roles_at_base|[string]|false|none|none|
|roles_at_hq|[string]|false|none|none|
|roles_at_other|[string]|false|none|none|
|title_id|integer(int64)|false|none|none|

<h2 id="tocS_CorporationsCorporationIdWalletsDivisionJournalGet">CorporationsCorporationIdWalletsDivisionJournalGet</h2>
<!-- backwards compatibility -->
<a id="schemacorporationscorporationidwalletsdivisionjournalget"></a>
<a id="schema_CorporationsCorporationIdWalletsDivisionJournalGet"></a>
<a id="tocScorporationscorporationidwalletsdivisionjournalget"></a>
<a id="tocscorporationscorporationidwalletsdivisionjournalget"></a>

```json
[
  {
    "amount": 0.1,
    "balance": 0.1,
    "context_id": 0,
    "context_id_type": "structure_id",
    "date": "2019-08-24T14:15:22Z",
    "description": "string",
    "first_party_id": 0,
    "id": 0,
    "reason": "string",
    "ref_type": "acceleration_gate_fee",
    "second_party_id": 0,
    "tax": 0.1,
    "tax_receiver_id": 0
  }
]

```

Journal entries

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|amount|number(double)|false|none|The amount of ISK given or taken from the wallet as a result of the given transaction. Positive when ISK is deposited into the wallet and negative when ISK is withdrawn|
|balance|number(double)|false|none|Wallet balance after transaction occurred|
|context_id|integer(int64)|false|none|An ID that gives extra context to the particular transaction. Because of legacy reasons the context is completely different per ref_type and means different things. It is also possible to not have a context_id|
|context_id_type|string|false|none|The type of the given context_id if present|
|date|string(date-time)|true|none|Date and time of transaction|
|description|string|true|none|The reason for the transaction, mirrors what is seen in the client|
|first_party_id|integer(int64)|false|none|The id of the first party involved in the transaction. This attribute has no consistency and is different or non existant for particular ref_types. The description attribute will help make sense of what this attribute means. For more info about the given ID it can be dropped into the /universe/names/ ESI route to determine its type and name|
|id|integer(int64)|true|none|Unique journal reference ID|
|reason|string|false|none|The user stated reason for the transaction. Only applies to some ref_types|
|ref_type|string|true|none|"The transaction type for the given. transaction. Different transaction types will populate different attributes. Note: If you have an existing XML API application that is using ref_types, you will need to know which string ESI ref_type maps to which integer. You can look at the following file to see string->int mappings: https://github.com/ccpgames/eve-glue/blob/master/eve_glue/wallet_journal_ref.py"|
|second_party_id|integer(int64)|false|none|The id of the second party involved in the transaction. This attribute has no consistency and is different or non existant for particular ref_types. The description attribute will help make sense of what this attribute means. For more info about the given ID it can be dropped into the /universe/names/ ESI route to determine its type and name|
|tax|number(double)|false|none|Tax amount received. Only applies to tax related transactions|
|tax_receiver_id|integer(int64)|false|none|The corporation ID receiving any tax paid. Only applies to tax related transactions|

#### Enumerated Values

|Property|Value|
|---|---|
|context_id_type|structure_id|
|context_id_type|station_id|
|context_id_type|market_transaction_id|
|context_id_type|character_id|
|context_id_type|corporation_id|
|context_id_type|alliance_id|
|context_id_type|eve_system|
|context_id_type|industry_job_id|
|context_id_type|contract_id|
|context_id_type|planet_id|
|context_id_type|system_id|
|context_id_type|type_id|
|ref_type|acceleration_gate_fee|
|ref_type|advertisement_listing_fee|
|ref_type|agent_donation|
|ref_type|agent_location_services|
|ref_type|agent_miscellaneous|
|ref_type|agent_mission_collateral_paid|
|ref_type|agent_mission_collateral_refunded|
|ref_type|agent_mission_reward|
|ref_type|agent_mission_reward_corporation_tax|
|ref_type|agent_mission_time_bonus_reward|
|ref_type|agent_mission_time_bonus_reward_corporation_tax|
|ref_type|agent_security_services|
|ref_type|agent_services_rendered|
|ref_type|agents_preward|
|ref_type|air_career_program_reward|
|ref_type|alliance_maintainance_fee|
|ref_type|alliance_registration_fee|
|ref_type|allignment_based_gate_toll|
|ref_type|asset_safety_recovery_tax|
|ref_type|bounty|
|ref_type|bounty_prize|
|ref_type|bounty_prize_corporation_tax|
|ref_type|bounty_prizes|
|ref_type|bounty_reimbursement|
|ref_type|bounty_surcharge|
|ref_type|brokers_fee|
|ref_type|clone_activation|
|ref_type|clone_transfer|
|ref_type|contraband_fine|
|ref_type|contract_auction_bid|
|ref_type|contract_auction_bid_corp|
|ref_type|contract_auction_bid_refund|
|ref_type|contract_auction_sold|
|ref_type|contract_brokers_fee|
|ref_type|contract_brokers_fee_corp|
|ref_type|contract_collateral|
|ref_type|contract_collateral_deposited_corp|
|ref_type|contract_collateral_payout|
|ref_type|contract_collateral_refund|
|ref_type|contract_deposit|
|ref_type|contract_deposit_corp|
|ref_type|contract_deposit_refund|
|ref_type|contract_deposit_sales_tax|
|ref_type|contract_price|
|ref_type|contract_price_payment_corp|
|ref_type|contract_reversal|
|ref_type|contract_reward|
|ref_type|contract_reward_deposited|
|ref_type|contract_reward_deposited_corp|
|ref_type|contract_reward_refund|
|ref_type|contract_sales_tax|
|ref_type|copying|
|ref_type|corporate_reward_payout|
|ref_type|corporate_reward_tax|
|ref_type|corporation_account_withdrawal|
|ref_type|corporation_bulk_payment|
|ref_type|corporation_dividend_payment|
|ref_type|corporation_liquidation|
|ref_type|corporation_logo_change_cost|
|ref_type|corporation_payment|
|ref_type|corporation_registration_fee|
|ref_type|cosmetic_market_component_item_purchase|
|ref_type|cosmetic_market_skin_purchase|
|ref_type|cosmetic_market_skin_sale|
|ref_type|cosmetic_market_skin_sale_broker_fee|
|ref_type|cosmetic_market_skin_sale_tax|
|ref_type|cosmetic_market_skin_transaction|
|ref_type|courier_mission_escrow|
|ref_type|cspa|
|ref_type|cspaofflinerefund|
|ref_type|daily_challenge_reward|
|ref_type|daily_goal_payouts|
|ref_type|daily_goal_payouts_tax|
|ref_type|datacore_fee|
|ref_type|dna_modification_fee|
|ref_type|docking_fee|
|ref_type|duel_wager_escrow|
|ref_type|duel_wager_payment|
|ref_type|duel_wager_refund|
|ref_type|ess_escrow_transfer|
|ref_type|external_trade_delivery|
|ref_type|external_trade_freeze|
|ref_type|external_trade_thaw|
|ref_type|factory_slot_rental_fee|
|ref_type|flux_payout|
|ref_type|flux_tax|
|ref_type|flux_ticket_repayment|
|ref_type|flux_ticket_sale|
|ref_type|freelance_jobs_broadcasting_fee|
|ref_type|freelance_jobs_duration_fee|
|ref_type|freelance_jobs_escrow_refund|
|ref_type|freelance_jobs_reward|
|ref_type|freelance_jobs_reward_corporation_tax|
|ref_type|freelance_jobs_reward_escrow|
|ref_type|gm_cash_transfer|
|ref_type|gm_plex_fee_refund|
|ref_type|industry_job_tax|
|ref_type|infrastructure_hub_maintenance|
|ref_type|inheritance|
|ref_type|insurance|
|ref_type|insurgency_corruption_contribution_reward|
|ref_type|insurgency_suppression_contribution_reward|
|ref_type|item_trader_payment|
|ref_type|jump_clone_activation_fee|
|ref_type|jump_clone_installation_fee|
|ref_type|kill_right_fee|
|ref_type|lp_store|
|ref_type|manufacturing|
|ref_type|market_escrow|
|ref_type|market_fine_paid|
|ref_type|market_provider_tax|
|ref_type|market_transaction|
|ref_type|medal_creation|
|ref_type|medal_issued|
|ref_type|milestone_reward_payment|
|ref_type|mission_completion|
|ref_type|mission_cost|
|ref_type|mission_expiration|
|ref_type|mission_reward|
|ref_type|office_rental_fee|
|ref_type|operation_bonus|
|ref_type|opportunity_reward|
|ref_type|planetary_construction|
|ref_type|planetary_export_tax|
|ref_type|planetary_import_tax|
|ref_type|player_donation|
|ref_type|player_trading|
|ref_type|project_discovery_reward|
|ref_type|project_discovery_tax|
|ref_type|project_payouts|
|ref_type|reaction|
|ref_type|redeemed_isk_token|
|ref_type|release_of_impounded_property|
|ref_type|repair_bill|
|ref_type|reprocessing_tax|
|ref_type|researching_material_productivity|
|ref_type|researching_technology|
|ref_type|researching_time_productivity|
|ref_type|resource_wars_reward|
|ref_type|reverse_engineering|
|ref_type|season_challenge_reward|
|ref_type|security_processing_fee|
|ref_type|shares|
|ref_type|skill_purchase|
|ref_type|skyhook_claim_fee|
|ref_type|sovereignity_bill|
|ref_type|store_purchase|
|ref_type|store_purchase_refund|
|ref_type|structure_gate_jump|
|ref_type|transaction_tax|
|ref_type|under_construction|
|ref_type|upkeep_adjustment_fee|
|ref_type|war_ally_contract|
|ref_type|war_fee|
|ref_type|war_fee_surrender|

<h2 id="tocS_CorporationsCorporationIdWalletsDivisionTransactionsGet">CorporationsCorporationIdWalletsDivisionTransactionsGet</h2>
<!-- backwards compatibility -->
<a id="schemacorporationscorporationidwalletsdivisiontransactionsget"></a>
<a id="schema_CorporationsCorporationIdWalletsDivisionTransactionsGet"></a>
<a id="tocScorporationscorporationidwalletsdivisiontransactionsget"></a>
<a id="tocscorporationscorporationidwalletsdivisiontransactionsget"></a>

```json
[
  {
    "client_id": 0,
    "date": "2019-08-24T14:15:22Z",
    "is_buy": true,
    "journal_ref_id": 0,
    "location_id": 0,
    "quantity": 0,
    "transaction_id": 0,
    "type_id": 0,
    "unit_price": 0.1
  }
]

```

Wallet transactions

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|client_id|integer(int64)|true|none|none|
|date|string(date-time)|true|none|Date and time of transaction|
|is_buy|boolean|true|none|none|
|journal_ref_id|integer(int64)|true|none|-1 if there is no corresponding wallet journal entry|
|location_id|integer(int64)|true|none|none|
|quantity|integer(int64)|true|none|none|
|transaction_id|integer(int64)|true|none|Unique transaction ID|
|type_id|integer(int64)|true|none|none|
|unit_price|number(double)|true|none|Amount paid per unit|

<h2 id="tocS_CorporationsCorporationIdWalletsGet">CorporationsCorporationIdWalletsGet</h2>
<!-- backwards compatibility -->
<a id="schemacorporationscorporationidwalletsget"></a>
<a id="schema_CorporationsCorporationIdWalletsGet"></a>
<a id="tocScorporationscorporationidwalletsget"></a>
<a id="tocscorporationscorporationidwalletsget"></a>

```json
[
  {
    "balance": 0.1,
    "division": 0
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|balance|number(double)|true|none|none|
|division|integer(int64)|true|none|none|

<h2 id="tocS_CorporationsNpccorpsGet">CorporationsNpccorpsGet</h2>
<!-- backwards compatibility -->
<a id="schemacorporationsnpccorpsget"></a>
<a id="schema_CorporationsNpccorpsGet"></a>
<a id="tocScorporationsnpccorpsget"></a>
<a id="tocscorporationsnpccorpsget"></a>

```json
[
  0
]

```

### Properties

*None*

<h2 id="tocS_CorporationsProjectsContribution">CorporationsProjectsContribution</h2>
<!-- backwards compatibility -->
<a id="schemacorporationsprojectscontribution"></a>
<a id="schema_CorporationsProjectsContribution"></a>
<a id="tocScorporationsprojectscontribution"></a>
<a id="tocscorporationsprojectscontribution"></a>

```json
{
  "contributed": 10,
  "last_modified": "2025-08-26T00:00:00Z"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|contributed|integer(int64)|true|none|Your contribution|
|last_modified|string(date-time)|false|none|Moment this information was last modified|

<h2 id="tocS_CorporationsProjectsContributors">CorporationsProjectsContributors</h2>
<!-- backwards compatibility -->
<a id="schemacorporationsprojectscontributors"></a>
<a id="schema_CorporationsProjectsContributors"></a>
<a id="tocScorporationsprojectscontributors"></a>
<a id="tocscorporationsprojectscontributors"></a>

```json
{
  "contributors": [
    {
      "contributed": 10,
      "id": 90000001,
      "name": "Contributor Name"
    }
  ],
  "cursor": {
    "after": "string",
    "before": "string"
  }
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|contributors|[[CorporationsProjectsContributorsContributor](#schemacorporationsprojectscontributorscontributor)]|true|none|List of contributors|
|cursor|[Cursor](#schemacursor)|false|none|none|

<h2 id="tocS_CorporationsProjectsContributorsContributor">CorporationsProjectsContributorsContributor</h2>
<!-- backwards compatibility -->
<a id="schemacorporationsprojectscontributorscontributor"></a>
<a id="schema_CorporationsProjectsContributorsContributor"></a>
<a id="tocScorporationsprojectscontributorscontributor"></a>
<a id="tocscorporationsprojectscontributorscontributor"></a>

```json
{
  "contributed": 10,
  "id": 90000001,
  "name": "Contributor Name"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|contributed|integer(int64)|true|none|Contributor's contributed progress|
|id|[CharacterID](#schemacharacterid)|true|none|Contributor's character ID|
|name|string|true|none|Contributor's name|

<h2 id="tocS_CorporationsProjectsDetail">CorporationsProjectsDetail</h2>
<!-- backwards compatibility -->
<a id="schemacorporationsprojectsdetail"></a>
<a id="schema_CorporationsProjectsDetail"></a>
<a id="tocScorporationsprojectsdetail"></a>
<a id="tocscorporationsprojectsdetail"></a>

```json
{
  "configuration": {
    "capture_fw_complex": {
      "archetypes": [
        {
          "archetype_id": 33
        }
      ],
      "factions": [
        {
          "faction_id": 500002
        }
      ],
      "locations": [
        {
          "solar_system_id": 30000001
        }
      ]
    }
  },
  "contribution": {
    "participation_limit": 1000,
    "reward_per_contribution": 123.5,
    "submission_limit": 100,
    "submission_multiplier": 1.5
  },
  "creator": {
    "id": 90000001,
    "name": "Creator Name"
  },
  "details": {
    "career": "Explorer",
    "created": "2025-06-01T00:00:00Z",
    "description": "Project Description",
    "expires": "2025-06-01T00:01:00Z",
    "finished": "2025-06-01T00:00:00Z"
  },
  "id": "3868eaed-8278-4cb7-9709-7d7de9c20dc7",
  "last_modified": "2025-06-01T00:00:00Z",
  "name": "Project Name",
  "progress": {
    "current": 50,
    "desired": 100
  },
  "reward": {
    "initial": 12345.5,
    "remaining": 5432.1
  },
  "state": "Active"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|configuration|any|true|none|Project's configuration|

oneOf

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» capture_fw_complex|[CorporationsProjectsDetailConfigurationcapturefwcomplex](#schemacorporationsprojectsdetailconfigurationcapturefwcomplex)|false|none|Capture factional warfare complex|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» damage_ship|[CorporationsProjectsDetailConfigurationdamageship](#schemacorporationsprojectsdetailconfigurationdamageship)|false|none|Damage ship|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» defend_fw_complex|[CorporationsProjectsDetailConfigurationdefendfwcomplex](#schemacorporationsprojectsdetailconfigurationdefendfwcomplex)|false|none|Defend factional warfare complex|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» deliver_item|[CorporationsProjectsDetailConfigurationdeliveritem](#schemacorporationsprojectsdetailconfigurationdeliveritem)|false|none|Deliver item|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» destroy_npc|[CorporationsProjectsDetailConfigurationdestroynpc](#schemacorporationsprojectsdetailconfigurationdestroynpc)|false|none|Destroy NPC|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» destroy_ship|[CorporationsProjectsDetailConfigurationdestroyship](#schemacorporationsprojectsdetailconfigurationdestroyship)|false|none|Destroy ship|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» earn_loyalty_point|[CorporationsProjectsDetailConfigurationearnloyaltypoints](#schemacorporationsprojectsdetailconfigurationearnloyaltypoints)|false|none|Earn loyalty point|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» lost_ship|[CorporationsProjectsDetailConfigurationlostship](#schemacorporationsprojectsdetailconfigurationlostship)|false|none|Lost ship|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» manual|[CorporationsProjectsDetailConfigurationmanual](#schemacorporationsprojectsdetailconfigurationmanual)|false|none|Manual contribution|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» manufacture_item|[CorporationsProjectsDetailConfigurationmanufactureitem](#schemacorporationsprojectsdetailconfigurationmanufactureitem)|false|none|Manufacture item|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» mine_material|[CorporationsProjectsDetailConfigurationminematerial](#schemacorporationsprojectsdetailconfigurationminematerial)|false|none|Mine material|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» remote_boost_shield|[CorporationsProjectsDetailConfigurationremoteboostshield](#schemacorporationsprojectsdetailconfigurationremoteboostshield)|false|none|Remote boost shield|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» remote_repair_armor|[CorporationsProjectsDetailConfigurationremoterepairarmor](#schemacorporationsprojectsdetailconfigurationremoterepairarmor)|false|none|Remote repair armor|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» salvage_wreck|[CorporationsProjectsDetailConfigurationsalvagewreck](#schemacorporationsprojectsdetailconfigurationsalvagewreck)|false|none|Salvage wreck|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» scan_signature|[CorporationsProjectsDetailConfigurationscansignature](#schemacorporationsprojectsdetailconfigurationscansignature)|false|none|Scan signature|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» ship_insurance|[CorporationsProjectsDetailConfigurationshipinsurance](#schemacorporationsprojectsdetailconfigurationshipinsurance)|false|none|Ship insurance|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» unknown|[CorporationsProjectsDetailConfigurationunknown](#schemacorporationsprojectsdetailconfigurationunknown)|false|none|Unknown|

continued

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|contribution|[CorporationsProjectsDetailContribution](#schemacorporationsprojectsdetailcontribution)|false|none|Project's contribution settings|
|creator|[CorporationsProjectsDetailCreator](#schemacorporationsprojectsdetailcreator)|true|none|Project's creator|
|details|[CorporationsProjectsDetailDetails](#schemacorporationsprojectsdetaildetails)|true|none|Project's details|
|id|[UUID](#schemauuid)|true|none|Project's ID|
|last_modified|string(date-time)|true|none|Moment this project was last modified. Project contributions also count as a modification|
|name|string|true|none|Project's name|
|progress|[CorporationsProjectsDetailProgress](#schemacorporationsprojectsdetailprogress)|true|none|Project's progress|
|reward|[CorporationsProjectsDetailReward](#schemacorporationsprojectsdetailreward)|false|none|Project's reward|
|state|string|true|none|Project's current state|

#### Enumerated Values

|Property|Value|
|---|---|
|state|Unspecified|
|state|Active|
|state|Closed|
|state|Completed|
|state|Expired|
|state|Deleted|

<h2 id="tocS_CorporationsProjectsDetailConfigurationcapturefwcomplex">CorporationsProjectsDetailConfigurationcapturefwcomplex</h2>
<!-- backwards compatibility -->
<a id="schemacorporationsprojectsdetailconfigurationcapturefwcomplex"></a>
<a id="schema_CorporationsProjectsDetailConfigurationcapturefwcomplex"></a>
<a id="tocScorporationsprojectsdetailconfigurationcapturefwcomplex"></a>
<a id="tocscorporationsprojectsdetailconfigurationcapturefwcomplex"></a>

```json
{
  "archetypes": [
    {
      "archetype_id": 33
    }
  ],
  "factions": [
    {
      "faction_id": 500002
    }
  ],
  "locations": [
    {
      "solar_system_id": 30000001
    }
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|archetypes|[[CorporationsProjectsDetailConfigurationmatcherarchetype](#schemacorporationsprojectsdetailconfigurationmatcherarchetype)]|false|none|Archetype of complex|
|factions|[[CorporationsProjectsDetailConfigurationmatcherfaction](#schemacorporationsprojectsdetailconfigurationmatcherfaction)]|false|none|Faction to capture for|
|locations|[oneOf]|false|none|Location of complex|

oneOf

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» solar_system_id|[SolarSystemID](#schemasolarsystemid)|false|none|Solar system's ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» constellation_id|[ConstellationID](#schemaconstellationid)|false|none|Constellation's ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» region_id|[RegionID](#schemaregionid)|false|none|Region's ID|

<h2 id="tocS_CorporationsProjectsDetailConfigurationdamageship">CorporationsProjectsDetailConfigurationdamageship</h2>
<!-- backwards compatibility -->
<a id="schemacorporationsprojectsdetailconfigurationdamageship"></a>
<a id="schema_CorporationsProjectsDetailConfigurationdamageship"></a>
<a id="tocScorporationsprojectsdetailconfigurationdamageship"></a>
<a id="tocscorporationsprojectsdetailconfigurationdamageship"></a>

```json
{
  "identities": [
    {
      "character_id": 90000001
    }
  ],
  "locations": [
    {
      "solar_system_id": 30000001
    }
  ],
  "ships": [
    {
      "type_id": 587
    }
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|identities|[oneOf]|false|none|Identity of capsuleer|

oneOf

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» character_id|[CharacterID](#schemacharacterid)|false|none|Character's ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» corporation_id|[CorporationID](#schemacorporationid)|false|none|Corporation's ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» alliance_id|[AllianceID](#schemaallianceid)|false|none|Alliance's ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» faction_id|[FactionID](#schemafactionid)|false|none|Faction's ID|

continued

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|locations|[oneOf]|false|none|Location of capsuleer's ship|

oneOf

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» solar_system_id|[SolarSystemID](#schemasolarsystemid)|false|none|Solar system's ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» constellation_id|[ConstellationID](#schemaconstellationid)|false|none|Constellation's ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» region_id|[RegionID](#schemaregionid)|false|none|Region's ID|

continued

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|ships|[oneOf]|false|none|Ship-type of capsuleer's ship|

oneOf

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» type_id|[TypeID](#schematypeid)|false|none|Ship's type ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» group_id|[ShipTreeGroupID](#schemashiptreegroupid)|false|none|Ship's ship tree group ID|

<h2 id="tocS_CorporationsProjectsDetailConfigurationdefendfwcomplex">CorporationsProjectsDetailConfigurationdefendfwcomplex</h2>
<!-- backwards compatibility -->
<a id="schemacorporationsprojectsdetailconfigurationdefendfwcomplex"></a>
<a id="schema_CorporationsProjectsDetailConfigurationdefendfwcomplex"></a>
<a id="tocScorporationsprojectsdetailconfigurationdefendfwcomplex"></a>
<a id="tocscorporationsprojectsdetailconfigurationdefendfwcomplex"></a>

```json
{
  "archetypes": [
    {
      "archetype_id": 33
    }
  ],
  "factions": [
    {
      "faction_id": 500002
    }
  ],
  "locations": [
    {
      "solar_system_id": 30000001
    }
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|archetypes|[[CorporationsProjectsDetailConfigurationmatcherarchetype](#schemacorporationsprojectsdetailconfigurationmatcherarchetype)]|false|none|Archetype of complex|
|factions|[[CorporationsProjectsDetailConfigurationmatcherfaction](#schemacorporationsprojectsdetailconfigurationmatcherfaction)]|false|none|Faction to defend for|
|locations|[oneOf]|false|none|Location of complex|

oneOf

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» solar_system_id|[SolarSystemID](#schemasolarsystemid)|false|none|Solar system's ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» constellation_id|[ConstellationID](#schemaconstellationid)|false|none|Constellation's ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» region_id|[RegionID](#schemaregionid)|false|none|Region's ID|

<h2 id="tocS_CorporationsProjectsDetailConfigurationdeliveritem">CorporationsProjectsDetailConfigurationdeliveritem</h2>
<!-- backwards compatibility -->
<a id="schemacorporationsprojectsdetailconfigurationdeliveritem"></a>
<a id="schema_CorporationsProjectsDetailConfigurationdeliveritem"></a>
<a id="tocScorporationsprojectsdetailconfigurationdeliveritem"></a>
<a id="tocscorporationsprojectsdetailconfigurationdeliveritem"></a>

```json
{
  "docking_locations": [
    {
      "structure_id": 1000000000001
    }
  ],
  "items": [
    {
      "type_id": 587
    }
  ],
  "office_id": 1000000000001
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|docking_locations|[oneOf]|false|none|Docking location to deliver to|

oneOf

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» structure_id|[ItemID](#schemaitemid)|false|none|Structure's ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» station_id|[StationID](#schemastationid)|false|none|Station's ID|

continued

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|items|[oneOf]|false|none|Item to deliver|

oneOf

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» type_id|[TypeID](#schematypeid)|false|none|Item's type ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» group_id|[GroupID](#schemagroupid)|false|none|Item's group ID|

continued

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|office_id|[ItemID](#schemaitemid)|false|none|Office to deliver to|

<h2 id="tocS_CorporationsProjectsDetailConfigurationdestroynpc">CorporationsProjectsDetailConfigurationdestroynpc</h2>
<!-- backwards compatibility -->
<a id="schemacorporationsprojectsdetailconfigurationdestroynpc"></a>
<a id="schema_CorporationsProjectsDetailConfigurationdestroynpc"></a>
<a id="tocScorporationsprojectsdetailconfigurationdestroynpc"></a>
<a id="tocscorporationsprojectsdetailconfigurationdestroynpc"></a>

```json
{
  "locations": [
    {
      "solar_system_id": 30000001
    }
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|locations|[oneOf]|false|none|Location of non-capsuleer|

oneOf

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» solar_system_id|[SolarSystemID](#schemasolarsystemid)|false|none|Solar system's ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» constellation_id|[ConstellationID](#schemaconstellationid)|false|none|Constellation's ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» region_id|[RegionID](#schemaregionid)|false|none|Region's ID|

<h2 id="tocS_CorporationsProjectsDetailConfigurationdestroyship">CorporationsProjectsDetailConfigurationdestroyship</h2>
<!-- backwards compatibility -->
<a id="schemacorporationsprojectsdetailconfigurationdestroyship"></a>
<a id="schema_CorporationsProjectsDetailConfigurationdestroyship"></a>
<a id="tocScorporationsprojectsdetailconfigurationdestroyship"></a>
<a id="tocscorporationsprojectsdetailconfigurationdestroyship"></a>

```json
{
  "identities": [
    {
      "character_id": 90000001
    }
  ],
  "locations": [
    {
      "solar_system_id": 30000001
    }
  ],
  "ships": [
    {
      "type_id": 587
    }
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|identities|[oneOf]|false|none|Identity of capsuleer|

oneOf

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» character_id|[CharacterID](#schemacharacterid)|false|none|Character's ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» corporation_id|[CorporationID](#schemacorporationid)|false|none|Corporation's ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» alliance_id|[AllianceID](#schemaallianceid)|false|none|Alliance's ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» faction_id|[FactionID](#schemafactionid)|false|none|Faction's ID|

continued

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|locations|[oneOf]|false|none|Location of capsuleer's ship|

oneOf

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» solar_system_id|[SolarSystemID](#schemasolarsystemid)|false|none|Solar system's ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» constellation_id|[ConstellationID](#schemaconstellationid)|false|none|Constellation's ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» region_id|[RegionID](#schemaregionid)|false|none|Region's ID|

continued

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|ships|[oneOf]|false|none|Ship-type of capsuleer's ship|

oneOf

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» type_id|[TypeID](#schematypeid)|false|none|Ship's type ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» group_id|[ShipTreeGroupID](#schemashiptreegroupid)|false|none|Ship's ship tree group ID|

<h2 id="tocS_CorporationsProjectsDetailConfigurationearnloyaltypoints">CorporationsProjectsDetailConfigurationearnloyaltypoints</h2>
<!-- backwards compatibility -->
<a id="schemacorporationsprojectsdetailconfigurationearnloyaltypoints"></a>
<a id="schema_CorporationsProjectsDetailConfigurationearnloyaltypoints"></a>
<a id="tocScorporationsprojectsdetailconfigurationearnloyaltypoints"></a>
<a id="tocscorporationsprojectsdetailconfigurationearnloyaltypoints"></a>

```json
{
  "corporations": [
    {
      "corporation_id": 98777771
    }
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|corporations|[[CorporationsProjectsDetailConfigurationmatchercorporation](#schemacorporationsprojectsdetailconfigurationmatchercorporation)]|false|none|Corporation issuing loyalty points|

<h2 id="tocS_CorporationsProjectsDetailConfigurationlostship">CorporationsProjectsDetailConfigurationlostship</h2>
<!-- backwards compatibility -->
<a id="schemacorporationsprojectsdetailconfigurationlostship"></a>
<a id="schema_CorporationsProjectsDetailConfigurationlostship"></a>
<a id="tocScorporationsprojectsdetailconfigurationlostship"></a>
<a id="tocscorporationsprojectsdetailconfigurationlostship"></a>

```json
{
  "identities": [
    {
      "character_id": 90000001
    }
  ],
  "locations": [
    {
      "solar_system_id": 30000001
    }
  ],
  "ships": [
    {
      "type_id": 587
    }
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|identities|[oneOf]|false|none|Identity of killer|

oneOf

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» character_id|[CharacterID](#schemacharacterid)|false|none|Character's ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» corporation_id|[CorporationID](#schemacorporationid)|false|none|Corporation's ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» alliance_id|[AllianceID](#schemaallianceid)|false|none|Alliance's ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» faction_id|[FactionID](#schemafactionid)|false|none|Faction's ID|

continued

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|locations|[oneOf]|false|none|Location of lost ship|

oneOf

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» solar_system_id|[SolarSystemID](#schemasolarsystemid)|false|none|Solar system's ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» constellation_id|[ConstellationID](#schemaconstellationid)|false|none|Constellation's ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» region_id|[RegionID](#schemaregionid)|false|none|Region's ID|

continued

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|ships|[oneOf]|false|none|Ship-type of lost ship|

oneOf

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» type_id|[TypeID](#schematypeid)|false|none|Ship's type ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» group_id|[ShipTreeGroupID](#schemashiptreegroupid)|false|none|Ship's ship tree group ID|

<h2 id="tocS_CorporationsProjectsDetailConfigurationmanual">CorporationsProjectsDetailConfigurationmanual</h2>
<!-- backwards compatibility -->
<a id="schemacorporationsprojectsdetailconfigurationmanual"></a>
<a id="schema_CorporationsProjectsDetailConfigurationmanual"></a>
<a id="tocScorporationsprojectsdetailconfigurationmanual"></a>
<a id="tocscorporationsprojectsdetailconfigurationmanual"></a>

```json
{}

```

### Properties

*None*

<h2 id="tocS_CorporationsProjectsDetailConfigurationmanufactureitem">CorporationsProjectsDetailConfigurationmanufactureitem</h2>
<!-- backwards compatibility -->
<a id="schemacorporationsprojectsdetailconfigurationmanufactureitem"></a>
<a id="schema_CorporationsProjectsDetailConfigurationmanufactureitem"></a>
<a id="tocScorporationsprojectsdetailconfigurationmanufactureitem"></a>
<a id="tocscorporationsprojectsdetailconfigurationmanufactureitem"></a>

```json
{
  "docking_locations": [
    {
      "structure_id": 1000000000001
    }
  ],
  "items": [
    {
      "type_id": 587
    }
  ],
  "owner": "Any"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|docking_locations|[oneOf]|false|none|Station / structure to manufacture in|

oneOf

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» structure_id|[ItemID](#schemaitemid)|false|none|Structure's ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» station_id|[StationID](#schemastationid)|false|none|Station's ID|

continued

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|items|[oneOf]|false|none|Item to manufacture|

oneOf

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» type_id|[TypeID](#schematypeid)|false|none|Item's type ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» group_id|[GroupID](#schemagroupid)|false|none|Item's group ID|

continued

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|owner|string|true|none|Manufacture for|

#### Enumerated Values

|Property|Value|
|---|---|
|owner|Any|
|owner|Corporation|
|owner|Character|

<h2 id="tocS_CorporationsProjectsDetailConfigurationmatcherarchetype">CorporationsProjectsDetailConfigurationmatcherarchetype</h2>
<!-- backwards compatibility -->
<a id="schemacorporationsprojectsdetailconfigurationmatcherarchetype"></a>
<a id="schema_CorporationsProjectsDetailConfigurationmatcherarchetype"></a>
<a id="tocScorporationsprojectsdetailconfigurationmatcherarchetype"></a>
<a id="tocscorporationsprojectsdetailconfigurationmatcherarchetype"></a>

```json
{
  "archetype_id": 33
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|archetype_id|[ArchetypeID](#schemaarchetypeid)|false|none|Archetype's ID|

<h2 id="tocS_CorporationsProjectsDetailConfigurationmatchercorporation">CorporationsProjectsDetailConfigurationmatchercorporation</h2>
<!-- backwards compatibility -->
<a id="schemacorporationsprojectsdetailconfigurationmatchercorporation"></a>
<a id="schema_CorporationsProjectsDetailConfigurationmatchercorporation"></a>
<a id="tocScorporationsprojectsdetailconfigurationmatchercorporation"></a>
<a id="tocscorporationsprojectsdetailconfigurationmatchercorporation"></a>

```json
{
  "corporation_id": 98777771
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|corporation_id|[CorporationID](#schemacorporationid)|false|none|Corporation's ID|

<h2 id="tocS_CorporationsProjectsDetailConfigurationmatcherfaction">CorporationsProjectsDetailConfigurationmatcherfaction</h2>
<!-- backwards compatibility -->
<a id="schemacorporationsprojectsdetailconfigurationmatcherfaction"></a>
<a id="schema_CorporationsProjectsDetailConfigurationmatcherfaction"></a>
<a id="tocScorporationsprojectsdetailconfigurationmatcherfaction"></a>
<a id="tocscorporationsprojectsdetailconfigurationmatcherfaction"></a>

```json
{
  "faction_id": 500002
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|faction_id|[FactionID](#schemafactionid)|false|none|Faction's ID|

<h2 id="tocS_CorporationsProjectsDetailConfigurationmatchersignature">CorporationsProjectsDetailConfigurationmatchersignature</h2>
<!-- backwards compatibility -->
<a id="schemacorporationsprojectsdetailconfigurationmatchersignature"></a>
<a id="schema_CorporationsProjectsDetailConfigurationmatchersignature"></a>
<a id="tocScorporationsprojectsdetailconfigurationmatchersignature"></a>
<a id="tocscorporationsprojectsdetailconfigurationmatchersignature"></a>

```json
{
  "signature_type_id": 209
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|signature_type_id|[AttributeID](#schemaattributeid)|false|none|Signature type's ID|

<h2 id="tocS_CorporationsProjectsDetailConfigurationminematerial">CorporationsProjectsDetailConfigurationminematerial</h2>
<!-- backwards compatibility -->
<a id="schemacorporationsprojectsdetailconfigurationminematerial"></a>
<a id="schema_CorporationsProjectsDetailConfigurationminematerial"></a>
<a id="tocScorporationsprojectsdetailconfigurationminematerial"></a>
<a id="tocscorporationsprojectsdetailconfigurationminematerial"></a>

```json
{
  "locations": [
    {
      "solar_system_id": 30000001
    }
  ],
  "materials": [
    {
      "type_id": 587
    }
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|locations|[oneOf]|false|none|Location to mine|

oneOf

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» solar_system_id|[SolarSystemID](#schemasolarsystemid)|false|none|Solar system's ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» constellation_id|[ConstellationID](#schemaconstellationid)|false|none|Constellation's ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» region_id|[RegionID](#schemaregionid)|false|none|Region's ID|

continued

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|materials|[oneOf]|false|none|Materials to mine|

oneOf

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» type_id|[TypeID](#schematypeid)|false|none|Ore's type ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» group_id|[GroupID](#schemagroupid)|false|none|Ore's group ID|

<h2 id="tocS_CorporationsProjectsDetailConfigurationremoteboostshield">CorporationsProjectsDetailConfigurationremoteboostshield</h2>
<!-- backwards compatibility -->
<a id="schemacorporationsprojectsdetailconfigurationremoteboostshield"></a>
<a id="schema_CorporationsProjectsDetailConfigurationremoteboostshield"></a>
<a id="tocScorporationsprojectsdetailconfigurationremoteboostshield"></a>
<a id="tocscorporationsprojectsdetailconfigurationremoteboostshield"></a>

```json
{
  "identities": [
    {
      "character_id": 90000001
    }
  ],
  "locations": [
    {
      "solar_system_id": 30000001
    }
  ],
  "ships": [
    {
      "type_id": 587
    }
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|identities|[oneOf]|false|none|Identity of capsuleer to boost|

oneOf

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» character_id|[CharacterID](#schemacharacterid)|false|none|Character's ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» corporation_id|[CorporationID](#schemacorporationid)|false|none|Corporation's ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» alliance_id|[AllianceID](#schemaallianceid)|false|none|Alliance's ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» faction_id|[FactionID](#schemafactionid)|false|none|Faction's ID|

continued

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|locations|[oneOf]|false|none|Location of capsuleer's ship to boost|

oneOf

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» solar_system_id|[SolarSystemID](#schemasolarsystemid)|false|none|Solar system's ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» constellation_id|[ConstellationID](#schemaconstellationid)|false|none|Constellation's ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» region_id|[RegionID](#schemaregionid)|false|none|Region's ID|

continued

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|ships|[oneOf]|false|none|Ship-type of capsuleer's ship to boost|

oneOf

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» type_id|[TypeID](#schematypeid)|false|none|Ship's type ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» group_id|[ShipTreeGroupID](#schemashiptreegroupid)|false|none|Ship's ship tree group ID|

<h2 id="tocS_CorporationsProjectsDetailConfigurationremoterepairarmor">CorporationsProjectsDetailConfigurationremoterepairarmor</h2>
<!-- backwards compatibility -->
<a id="schemacorporationsprojectsdetailconfigurationremoterepairarmor"></a>
<a id="schema_CorporationsProjectsDetailConfigurationremoterepairarmor"></a>
<a id="tocScorporationsprojectsdetailconfigurationremoterepairarmor"></a>
<a id="tocscorporationsprojectsdetailconfigurationremoterepairarmor"></a>

```json
{
  "identities": [
    {
      "character_id": 90000001
    }
  ],
  "locations": [
    {
      "solar_system_id": 30000001
    }
  ],
  "ships": [
    {
      "type_id": 587
    }
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|identities|[oneOf]|false|none|Identity of capsuleer to repair|

oneOf

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» character_id|[CharacterID](#schemacharacterid)|false|none|Character's ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» corporation_id|[CorporationID](#schemacorporationid)|false|none|Corporation's ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» alliance_id|[AllianceID](#schemaallianceid)|false|none|Alliance's ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» faction_id|[FactionID](#schemafactionid)|false|none|Faction's ID|

continued

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|locations|[oneOf]|false|none|Location of capsuleer's ship to repair|

oneOf

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» solar_system_id|[SolarSystemID](#schemasolarsystemid)|false|none|Solar system's ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» constellation_id|[ConstellationID](#schemaconstellationid)|false|none|Constellation's ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» region_id|[RegionID](#schemaregionid)|false|none|Region's ID|

continued

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|ships|[oneOf]|false|none|Ship-type of capsuleer's ship to repair|

oneOf

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» type_id|[TypeID](#schematypeid)|false|none|Ship's type ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» group_id|[ShipTreeGroupID](#schemashiptreegroupid)|false|none|Ship's ship tree group ID|

<h2 id="tocS_CorporationsProjectsDetailConfigurationsalvagewreck">CorporationsProjectsDetailConfigurationsalvagewreck</h2>
<!-- backwards compatibility -->
<a id="schemacorporationsprojectsdetailconfigurationsalvagewreck"></a>
<a id="schema_CorporationsProjectsDetailConfigurationsalvagewreck"></a>
<a id="tocScorporationsprojectsdetailconfigurationsalvagewreck"></a>
<a id="tocscorporationsprojectsdetailconfigurationsalvagewreck"></a>

```json
{
  "locations": [
    {
      "solar_system_id": 30000001
    }
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|locations|[oneOf]|false|none|Location of wreck|

oneOf

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» solar_system_id|[SolarSystemID](#schemasolarsystemid)|false|none|Solar system's ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» constellation_id|[ConstellationID](#schemaconstellationid)|false|none|Constellation's ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» region_id|[RegionID](#schemaregionid)|false|none|Region's ID|

<h2 id="tocS_CorporationsProjectsDetailConfigurationscansignature">CorporationsProjectsDetailConfigurationscansignature</h2>
<!-- backwards compatibility -->
<a id="schemacorporationsprojectsdetailconfigurationscansignature"></a>
<a id="schema_CorporationsProjectsDetailConfigurationscansignature"></a>
<a id="tocScorporationsprojectsdetailconfigurationscansignature"></a>
<a id="tocscorporationsprojectsdetailconfigurationscansignature"></a>

```json
{
  "locations": [
    {
      "solar_system_id": 30000001
    }
  ],
  "signatures": [
    {
      "signature_type_id": 209
    }
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|locations|[oneOf]|false|none|Locations of signatures|

oneOf

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» solar_system_id|[SolarSystemID](#schemasolarsystemid)|false|none|Solar system's ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» constellation_id|[ConstellationID](#schemaconstellationid)|false|none|Constellation's ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» region_id|[RegionID](#schemaregionid)|false|none|Region's ID|

continued

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|signatures|[[CorporationsProjectsDetailConfigurationmatchersignature](#schemacorporationsprojectsdetailconfigurationmatchersignature)]|false|none|Signatures to scan|

<h2 id="tocS_CorporationsProjectsDetailConfigurationshipinsurance">CorporationsProjectsDetailConfigurationshipinsurance</h2>
<!-- backwards compatibility -->
<a id="schemacorporationsprojectsdetailconfigurationshipinsurance"></a>
<a id="schema_CorporationsProjectsDetailConfigurationshipinsurance"></a>
<a id="tocScorporationsprojectsdetailconfigurationshipinsurance"></a>
<a id="tocscorporationsprojectsdetailconfigurationshipinsurance"></a>

```json
{
  "conflict_type": "Any",
  "identities": [
    {
      "character_id": 90000001
    }
  ],
  "locations": [
    {
      "solar_system_id": 30000001
    }
  ],
  "reimburse_implants": true,
  "ships": [
    {
      "type_id": 587
    }
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|conflict_type|string|true|none|Conflict type|
|identities|[oneOf]|false|none|Identity of killer|

oneOf

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» character_id|[CharacterID](#schemacharacterid)|false|none|Character's ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» corporation_id|[CorporationID](#schemacorporationid)|false|none|Corporation's ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» alliance_id|[AllianceID](#schemaallianceid)|false|none|Alliance's ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» faction_id|[FactionID](#schemafactionid)|false|none|Faction's ID|

continued

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|locations|[oneOf]|false|none|Location of lost ship|

oneOf

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» solar_system_id|[SolarSystemID](#schemasolarsystemid)|false|none|Solar system's ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» constellation_id|[ConstellationID](#schemaconstellationid)|false|none|Constellation's ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» region_id|[RegionID](#schemaregionid)|false|none|Region's ID|

continued

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|reimburse_implants|boolean|true|none|Reimburse implants|
|ships|[oneOf]|false|none|Ship-type of lost ship|

oneOf

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» type_id|[TypeID](#schematypeid)|false|none|Ship's type ID|

xor

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|object|false|none|none|
|»» group_id|[ShipTreeGroupID](#schemashiptreegroupid)|false|none|Ship's ship tree group ID|

#### Enumerated Values

|Property|Value|
|---|---|
|conflict_type|Any|
|conflict_type|Pvp|
|conflict_type|Pve|

<h2 id="tocS_CorporationsProjectsDetailConfigurationunknown">CorporationsProjectsDetailConfigurationunknown</h2>
<!-- backwards compatibility -->
<a id="schemacorporationsprojectsdetailconfigurationunknown"></a>
<a id="schema_CorporationsProjectsDetailConfigurationunknown"></a>
<a id="tocScorporationsprojectsdetailconfigurationunknown"></a>
<a id="tocscorporationsprojectsdetailconfigurationunknown"></a>

```json
{
  "data": {},
  "type": "projectType"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|data|any|true|none|JSON-encoded configuration|
|type|string|true|none|Configuration type|

<h2 id="tocS_CorporationsProjectsDetailContribution">CorporationsProjectsDetailContribution</h2>
<!-- backwards compatibility -->
<a id="schemacorporationsprojectsdetailcontribution"></a>
<a id="schema_CorporationsProjectsDetailContribution"></a>
<a id="tocScorporationsprojectsdetailcontribution"></a>
<a id="tocscorporationsprojectsdetailcontribution"></a>

```json
{
  "participation_limit": 1000,
  "reward_per_contribution": 123.5,
  "submission_limit": 100,
  "submission_multiplier": 1.5
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|participation_limit|integer(int64)|false|none|Limit on the contribution of the individual participant|
|reward_per_contribution|number(double)|false|none|ISK reward per contribution|
|submission_limit|integer(int64)|false|none|Limit on amount of contribution per submission|
|submission_multiplier|number(double)|false|none|Multiplier towards progress per contribution|

<h2 id="tocS_CorporationsProjectsDetailCreator">CorporationsProjectsDetailCreator</h2>
<!-- backwards compatibility -->
<a id="schemacorporationsprojectsdetailcreator"></a>
<a id="schema_CorporationsProjectsDetailCreator"></a>
<a id="tocScorporationsprojectsdetailcreator"></a>
<a id="tocscorporationsprojectsdetailcreator"></a>

```json
{
  "id": 90000001,
  "name": "Creator Name"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|[CharacterID](#schemacharacterid)|true|none|Creator's character ID|
|name|string|true|none|Creator's name|

<h2 id="tocS_CorporationsProjectsDetailDetails">CorporationsProjectsDetailDetails</h2>
<!-- backwards compatibility -->
<a id="schemacorporationsprojectsdetaildetails"></a>
<a id="schema_CorporationsProjectsDetailDetails"></a>
<a id="tocScorporationsprojectsdetaildetails"></a>
<a id="tocscorporationsprojectsdetaildetails"></a>

```json
{
  "career": "Explorer",
  "created": "2025-06-01T00:00:00Z",
  "description": "Project Description",
  "expires": "2025-06-01T00:01:00Z",
  "finished": "2025-06-01T00:00:00Z"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|career|string|true|none|Assigned career path|
|created|string(date-time)|true|none|Moment this project was created|
|description|string|true|none|Description|
|expires|string(date-time)|false|none|Moment this project expires|
|finished|string(date-time)|false|none|Moment this project transitioned to a non-active state.|

#### Enumerated Values

|Property|Value|
|---|---|
|career|Unspecified|
|career|Explorer|
|career|Industrialist|
|career|Enforcer|
|career|Soldier of Fortune|

<h2 id="tocS_CorporationsProjectsDetailProgress">CorporationsProjectsDetailProgress</h2>
<!-- backwards compatibility -->
<a id="schemacorporationsprojectsdetailprogress"></a>
<a id="schema_CorporationsProjectsDetailProgress"></a>
<a id="tocScorporationsprojectsdetailprogress"></a>
<a id="tocscorporationsprojectsdetailprogress"></a>

```json
{
  "current": 50,
  "desired": 100
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|current|integer(int64)|true|none|Current progress|
|desired|integer(int64)|true|none|Desired progress|

<h2 id="tocS_CorporationsProjectsDetailProject">CorporationsProjectsDetailProject</h2>
<!-- backwards compatibility -->
<a id="schemacorporationsprojectsdetailproject"></a>
<a id="schema_CorporationsProjectsDetailProject"></a>
<a id="tocScorporationsprojectsdetailproject"></a>
<a id="tocscorporationsprojectsdetailproject"></a>

```json
{
  "id": "3868eaed-8278-4cb7-9709-7d7de9c20dc7",
  "last_modified": "2025-06-01T00:00:00Z",
  "name": "Project Name",
  "progress": {
    "current": 50,
    "desired": 100
  },
  "reward": {
    "initial": 12345.5,
    "remaining": 5432.1
  },
  "state": "Active"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|[UUID](#schemauuid)|true|none|Project's ID|
|last_modified|string(date-time)|true|none|Moment this project was last modified. Project contributions also count as a modification|
|name|string|true|none|Project's name|
|progress|[CorporationsProjectsDetailProgress](#schemacorporationsprojectsdetailprogress)|true|none|Project's progress|
|reward|[CorporationsProjectsDetailReward](#schemacorporationsprojectsdetailreward)|false|none|Project's reward|
|state|string|true|none|Project's current state|

#### Enumerated Values

|Property|Value|
|---|---|
|state|Unspecified|
|state|Active|
|state|Closed|
|state|Completed|
|state|Expired|
|state|Deleted|

<h2 id="tocS_CorporationsProjectsDetailReward">CorporationsProjectsDetailReward</h2>
<!-- backwards compatibility -->
<a id="schemacorporationsprojectsdetailreward"></a>
<a id="schema_CorporationsProjectsDetailReward"></a>
<a id="tocScorporationsprojectsdetailreward"></a>
<a id="tocscorporationsprojectsdetailreward"></a>

```json
{
  "initial": 12345.5,
  "remaining": 5432.1
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|initial|number(double)|true|none|Original amount of ISK that was reserved for this project|
|remaining|number(double)|true|none|Remaining ISK to be awarded|

<h2 id="tocS_CorporationsProjectsListing">CorporationsProjectsListing</h2>
<!-- backwards compatibility -->
<a id="schemacorporationsprojectslisting"></a>
<a id="schema_CorporationsProjectsListing"></a>
<a id="tocScorporationsprojectslisting"></a>
<a id="tocscorporationsprojectslisting"></a>

```json
{
  "cursor": {
    "after": "string",
    "before": "string"
  },
  "projects": [
    {
      "id": "3868eaed-8278-4cb7-9709-7d7de9c20dc7",
      "last_modified": "2025-06-01T00:00:00Z",
      "name": "Project Name",
      "progress": {
        "current": 50,
        "desired": 100
      },
      "reward": {
        "initial": 12345.5,
        "remaining": 5432.1
      },
      "state": "Active"
    }
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|cursor|[Cursor](#schemacursor)|false|none|none|
|projects|[[CorporationsProjectsDetailProject](#schemacorporationsprojectsdetailproject)]|true|none|List of projects|

<h2 id="tocS_Cursor">Cursor</h2>
<!-- backwards compatibility -->
<a id="schemacursor"></a>
<a id="schema_Cursor"></a>
<a id="tocScursor"></a>
<a id="tocscursor"></a>

```json
{
  "after": "string",
  "before": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|after|string|false|none|Cursor to use as 'after' in your next request, to continue walking forwards in time.|
|before|string|false|none|Cursor to use as 'before' in your next request, to continue walking backwards in time.|

<h2 id="tocS_DogmaAttributesAttributeIdGet">DogmaAttributesAttributeIdGet</h2>
<!-- backwards compatibility -->
<a id="schemadogmaattributesattributeidget"></a>
<a id="schema_DogmaAttributesAttributeIdGet"></a>
<a id="tocSdogmaattributesattributeidget"></a>
<a id="tocsdogmaattributesattributeidget"></a>

```json
{
  "attribute_id": 0,
  "default_value": 0.1,
  "description": "string",
  "display_name": "string",
  "high_is_good": true,
  "icon_id": 0,
  "name": "string",
  "published": true,
  "stackable": true,
  "unit_id": 0
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|attribute_id|integer(int64)|true|none|none|
|default_value|number(double)|false|none|none|
|description|string|false|none|none|
|display_name|string|false|none|none|
|high_is_good|boolean|false|none|none|
|icon_id|integer(int64)|false|none|none|
|name|string|false|none|none|
|published|boolean|false|none|none|
|stackable|boolean|false|none|none|
|unit_id|integer(int64)|false|none|none|

<h2 id="tocS_DogmaAttributesGet">DogmaAttributesGet</h2>
<!-- backwards compatibility -->
<a id="schemadogmaattributesget"></a>
<a id="schema_DogmaAttributesGet"></a>
<a id="tocSdogmaattributesget"></a>
<a id="tocsdogmaattributesget"></a>

```json
[
  0
]

```

### Properties

*None*

<h2 id="tocS_DogmaDynamicItemsTypeIdItemIdGet">DogmaDynamicItemsTypeIdItemIdGet</h2>
<!-- backwards compatibility -->
<a id="schemadogmadynamicitemstypeiditemidget"></a>
<a id="schema_DogmaDynamicItemsTypeIdItemIdGet"></a>
<a id="tocSdogmadynamicitemstypeiditemidget"></a>
<a id="tocsdogmadynamicitemstypeiditemidget"></a>

```json
{
  "created_by": 0,
  "dogma_attributes": [
    {
      "attribute_id": 0,
      "value": 0.1
    }
  ],
  "dogma_effects": [
    {
      "effect_id": 0,
      "is_default": true
    }
  ],
  "mutator_type_id": 0,
  "source_type_id": 0
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|created_by|integer(int64)|true|none|The ID of the character who created the item|
|dogma_attributes|[object]|true|none|none|
|» attribute_id|integer(int64)|true|none|none|
|» value|number(double)|true|none|none|
|dogma_effects|[object]|true|none|none|
|» effect_id|integer(int64)|true|none|none|
|» is_default|boolean|true|none|none|
|mutator_type_id|integer(int64)|true|none|The type ID of the mutator used to generate the dynamic item.|
|source_type_id|integer(int64)|true|none|The type ID of the source item the mutator was applied to create the dynamic item.|

<h2 id="tocS_DogmaEffectsEffectIdGet">DogmaEffectsEffectIdGet</h2>
<!-- backwards compatibility -->
<a id="schemadogmaeffectseffectidget"></a>
<a id="schema_DogmaEffectsEffectIdGet"></a>
<a id="tocSdogmaeffectseffectidget"></a>
<a id="tocsdogmaeffectseffectidget"></a>

```json
{
  "description": "string",
  "disallow_auto_repeat": true,
  "discharge_attribute_id": 0,
  "display_name": "string",
  "duration_attribute_id": 0,
  "effect_category": 0,
  "effect_id": 0,
  "electronic_chance": true,
  "falloff_attribute_id": 0,
  "icon_id": 0,
  "is_assistance": true,
  "is_offensive": true,
  "is_warp_safe": true,
  "modifiers": [
    {
      "domain": "string",
      "effect_id": 0,
      "func": "string",
      "modified_attribute_id": 0,
      "modifying_attribute_id": 0,
      "operator": 0
    }
  ],
  "name": "string",
  "post_expression": 0,
  "pre_expression": 0,
  "published": true,
  "range_attribute_id": 0,
  "range_chance": true,
  "tracking_speed_attribute_id": 0
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|description|string|false|none|none|
|disallow_auto_repeat|boolean|false|none|none|
|discharge_attribute_id|integer(int64)|false|none|none|
|display_name|string|false|none|none|
|duration_attribute_id|integer(int64)|false|none|none|
|effect_category|integer(int64)|false|none|none|
|effect_id|integer(int64)|true|none|none|
|electronic_chance|boolean|false|none|none|
|falloff_attribute_id|integer(int64)|false|none|none|
|icon_id|integer(int64)|false|none|none|
|is_assistance|boolean|false|none|none|
|is_offensive|boolean|false|none|none|
|is_warp_safe|boolean|false|none|none|
|modifiers|[object]|false|none|none|
|» domain|string|false|none|none|
|» effect_id|integer(int64)|false|none|none|
|» func|string|true|none|none|
|» modified_attribute_id|integer(int64)|false|none|none|
|» modifying_attribute_id|integer(int64)|false|none|none|
|» operator|integer(int64)|false|none|none|
|name|string|false|none|none|
|post_expression|integer(int64)|false|none|none|
|pre_expression|integer(int64)|false|none|none|
|published|boolean|false|none|none|
|range_attribute_id|integer(int64)|false|none|none|
|range_chance|boolean|false|none|none|
|tracking_speed_attribute_id|integer(int64)|false|none|none|

<h2 id="tocS_DogmaEffectsGet">DogmaEffectsGet</h2>
<!-- backwards compatibility -->
<a id="schemadogmaeffectsget"></a>
<a id="schema_DogmaEffectsGet"></a>
<a id="tocSdogmaeffectsget"></a>
<a id="tocsdogmaeffectsget"></a>

```json
[
  0
]

```

### Properties

*None*

<h2 id="tocS_Error">Error</h2>
<!-- backwards compatibility -->
<a id="schemaerror"></a>
<a id="schema_Error"></a>
<a id="tocSerror"></a>
<a id="tocserror"></a>

```json
{
  "details": [
    {
      "location": "string",
      "message": "string",
      "value": null
    }
  ],
  "error": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|details|[[ErrorDetail](#schemaerrordetail)]|false|none|List of individual error details.|
|error|string|true|none|Error message.|

<h2 id="tocS_ErrorDetail">ErrorDetail</h2>
<!-- backwards compatibility -->
<a id="schemaerrordetail"></a>
<a id="schema_ErrorDetail"></a>
<a id="tocSerrordetail"></a>
<a id="tocserrordetail"></a>

```json
{
  "location": "string",
  "message": "string",
  "value": null
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|location|string|false|none|Where the error occurred, e.g. 'body.items[3].tags' or 'path.thing-id'|
|message|string|false|none|Error message text|
|value|any|false|none|The value at the given location|

<h2 id="tocS_FactionID">FactionID</h2>
<!-- backwards compatibility -->
<a id="schemafactionid"></a>
<a id="schema_FactionID"></a>
<a id="tocSfactionid"></a>
<a id="tocsfactionid"></a>

```json
500002

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|integer(int64)|false|none|none|

<h2 id="tocS_FleetsFleetIdGet">FleetsFleetIdGet</h2>
<!-- backwards compatibility -->
<a id="schemafleetsfleetidget"></a>
<a id="schema_FleetsFleetIdGet"></a>
<a id="tocSfleetsfleetidget"></a>
<a id="tocsfleetsfleetidget"></a>

```json
{
  "is_free_move": true,
  "is_registered": true,
  "is_voice_enabled": true,
  "motd": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|is_free_move|boolean|true|none|Is free-move enabled|
|is_registered|boolean|true|none|Does the fleet have an active fleet advertisement|
|is_voice_enabled|boolean|true|none|Is EVE Voice enabled|
|motd|string|true|none|Fleet MOTD in CCP flavoured HTML|

<h2 id="tocS_FleetsFleetIdMembersGet">FleetsFleetIdMembersGet</h2>
<!-- backwards compatibility -->
<a id="schemafleetsfleetidmembersget"></a>
<a id="schema_FleetsFleetIdMembersGet"></a>
<a id="tocSfleetsfleetidmembersget"></a>
<a id="tocsfleetsfleetidmembersget"></a>

```json
[
  {
    "character_id": 0,
    "join_time": "2019-08-24T14:15:22Z",
    "role": "fleet_commander",
    "role_name": "string",
    "ship_type_id": 0,
    "solar_system_id": 0,
    "squad_id": 0,
    "station_id": 0,
    "takes_fleet_warp": true,
    "wing_id": 0
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|character_id|integer(int64)|true|none|none|
|join_time|string(date-time)|true|none|none|
|role|string|true|none|Member’s role in fleet|
|role_name|string|true|none|Localized role names|
|ship_type_id|integer(int64)|true|none|none|
|solar_system_id|integer(int64)|true|none|Solar system the member is located in|
|squad_id|integer(int64)|true|none|ID of the squad the member is in. If not applicable, will be set to -1|
|station_id|integer(int64)|false|none|Station in which the member is docked in, if applicable|
|takes_fleet_warp|boolean|true|none|Whether the member take fleet warps|
|wing_id|integer(int64)|true|none|ID of the wing the member is in. If not applicable, will be set to -1|

#### Enumerated Values

|Property|Value|
|---|---|
|role|fleet_commander|
|role|wing_commander|
|role|squad_commander|
|role|squad_member|

<h2 id="tocS_FleetsFleetIdWingsGet">FleetsFleetIdWingsGet</h2>
<!-- backwards compatibility -->
<a id="schemafleetsfleetidwingsget"></a>
<a id="schema_FleetsFleetIdWingsGet"></a>
<a id="tocSfleetsfleetidwingsget"></a>
<a id="tocsfleetsfleetidwingsget"></a>

```json
[
  {
    "id": 0,
    "name": "string",
    "squads": [
      {
        "id": 0,
        "name": "string"
      }
    ]
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|integer(int64)|true|none|none|
|name|string|true|none|none|
|squads|[object]|true|none|none|
|» id|integer(int64)|true|none|none|
|» name|string|true|none|none|

<h2 id="tocS_FleetsFleetIdWingsPost">FleetsFleetIdWingsPost</h2>
<!-- backwards compatibility -->
<a id="schemafleetsfleetidwingspost"></a>
<a id="schema_FleetsFleetIdWingsPost"></a>
<a id="tocSfleetsfleetidwingspost"></a>
<a id="tocsfleetsfleetidwingspost"></a>

```json
{
  "wing_id": 0
}

```

201 created object

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|wing_id|integer(int64)|true|none|The wing_id of the newly created wing|

<h2 id="tocS_FleetsFleetIdWingsWingIdSquadsPost">FleetsFleetIdWingsWingIdSquadsPost</h2>
<!-- backwards compatibility -->
<a id="schemafleetsfleetidwingswingidsquadspost"></a>
<a id="schema_FleetsFleetIdWingsWingIdSquadsPost"></a>
<a id="tocSfleetsfleetidwingswingidsquadspost"></a>
<a id="tocsfleetsfleetidwingswingidsquadspost"></a>

```json
{
  "squad_id": 0
}

```

201 created object

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|squad_id|integer(int64)|true|none|The squad_id of the newly created squad|

<h2 id="tocS_FwLeaderboardsCharactersGet">FwLeaderboardsCharactersGet</h2>
<!-- backwards compatibility -->
<a id="schemafwleaderboardscharactersget"></a>
<a id="schema_FwLeaderboardsCharactersGet"></a>
<a id="tocSfwleaderboardscharactersget"></a>
<a id="tocsfwleaderboardscharactersget"></a>

```json
{
  "kills": {
    "active_total": [
      {
        "amount": 0,
        "character_id": 0
      }
    ],
    "last_week": [
      {
        "amount": 0,
        "character_id": 0
      }
    ],
    "yesterday": [
      {
        "amount": 0,
        "character_id": 0
      }
    ]
  },
  "victory_points": {
    "active_total": [
      {
        "amount": 0,
        "character_id": 0
      }
    ],
    "last_week": [
      {
        "amount": 0,
        "character_id": 0
      }
    ],
    "yesterday": [
      {
        "amount": 0,
        "character_id": 0
      }
    ]
  }
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|kills|object|true|none|Top 100 rankings of pilots by number of kills from yesterday, last week and in total|
|» active_total|[object]|true|none|Top 100 ranking of pilots active in faction warfare by total kills. A pilot is considered "active" if they have participated in faction warfare in the past 14 days|
|»» amount|integer(int64)|false|none|Amount of kills|
|»» character_id|integer(int64)|false|none|none|
|» last_week|[object]|true|none|Top 100 ranking of pilots by kills in the past week|
|»» amount|integer(int64)|false|none|Amount of kills|
|»» character_id|integer(int64)|false|none|none|
|» yesterday|[object]|true|none|Top 100 ranking of pilots by kills in the past day|
|»» amount|integer(int64)|false|none|Amount of kills|
|»» character_id|integer(int64)|false|none|none|
|victory_points|object|true|none|Top 100 rankings of pilots by victory points from yesterday, last week and in total|
|» active_total|[object]|true|none|Top 100 ranking of pilots active in faction warfare by total victory points. A pilot is considered "active" if they have participated in faction warfare in the past 14 days|
|»» amount|integer(int64)|false|none|Amount of victory points|
|»» character_id|integer(int64)|false|none|none|
|» last_week|[object]|true|none|Top 100 ranking of pilots by victory points in the past week|
|»» amount|integer(int64)|false|none|Amount of victory points|
|»» character_id|integer(int64)|false|none|none|
|» yesterday|[object]|true|none|Top 100 ranking of pilots by victory points in the past day|
|»» amount|integer(int64)|false|none|Amount of victory points|
|»» character_id|integer(int64)|false|none|none|

<h2 id="tocS_FwLeaderboardsCorporationsGet">FwLeaderboardsCorporationsGet</h2>
<!-- backwards compatibility -->
<a id="schemafwleaderboardscorporationsget"></a>
<a id="schema_FwLeaderboardsCorporationsGet"></a>
<a id="tocSfwleaderboardscorporationsget"></a>
<a id="tocsfwleaderboardscorporationsget"></a>

```json
{
  "kills": {
    "active_total": [
      {
        "amount": 0,
        "corporation_id": 0
      }
    ],
    "last_week": [
      {
        "amount": 0,
        "corporation_id": 0
      }
    ],
    "yesterday": [
      {
        "amount": 0,
        "corporation_id": 0
      }
    ]
  },
  "victory_points": {
    "active_total": [
      {
        "amount": 0,
        "corporation_id": 0
      }
    ],
    "last_week": [
      {
        "amount": 0,
        "corporation_id": 0
      }
    ],
    "yesterday": [
      {
        "amount": 0,
        "corporation_id": 0
      }
    ]
  }
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|kills|object|true|none|Top 10 rankings of corporations by number of kills from yesterday, last week and in total|
|» active_total|[object]|true|none|Top 10 ranking of corporations active in faction warfare by total kills. A corporation is considered "active" if they have participated in faction warfare in the past 14 days|
|»» amount|integer(int64)|false|none|Amount of kills|
|»» corporation_id|integer(int64)|false|none|none|
|» last_week|[object]|true|none|Top 10 ranking of corporations by kills in the past week|
|»» amount|integer(int64)|false|none|Amount of kills|
|»» corporation_id|integer(int64)|false|none|none|
|» yesterday|[object]|true|none|Top 10 ranking of corporations by kills in the past day|
|»» amount|integer(int64)|false|none|Amount of kills|
|»» corporation_id|integer(int64)|false|none|none|
|victory_points|object|true|none|Top 10 rankings of corporations by victory points from yesterday, last week and in total|
|» active_total|[object]|true|none|Top 10 ranking of corporations active in faction warfare by total victory points. A corporation is considered "active" if they have participated in faction warfare in the past 14 days|
|»» amount|integer(int64)|false|none|Amount of victory points|
|»» corporation_id|integer(int64)|false|none|none|
|» last_week|[object]|true|none|Top 10 ranking of corporations by victory points in the past week|
|»» amount|integer(int64)|false|none|Amount of victory points|
|»» corporation_id|integer(int64)|false|none|none|
|» yesterday|[object]|true|none|Top 10 ranking of corporations by victory points in the past day|
|»» amount|integer(int64)|false|none|Amount of victory points|
|»» corporation_id|integer(int64)|false|none|none|

<h2 id="tocS_FwLeaderboardsGet">FwLeaderboardsGet</h2>
<!-- backwards compatibility -->
<a id="schemafwleaderboardsget"></a>
<a id="schema_FwLeaderboardsGet"></a>
<a id="tocSfwleaderboardsget"></a>
<a id="tocsfwleaderboardsget"></a>

```json
{
  "kills": {
    "active_total": [
      {
        "amount": 0,
        "faction_id": 0
      }
    ],
    "last_week": [
      {
        "amount": 0,
        "faction_id": 0
      }
    ],
    "yesterday": [
      {
        "amount": 0,
        "faction_id": 0
      }
    ]
  },
  "victory_points": {
    "active_total": [
      {
        "amount": 0,
        "faction_id": 0
      }
    ],
    "last_week": [
      {
        "amount": 0,
        "faction_id": 0
      }
    ],
    "yesterday": [
      {
        "amount": 0,
        "faction_id": 0
      }
    ]
  }
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|kills|object|true|none|Top 4 rankings of factions by number of kills from yesterday, last week and in total|
|» active_total|[object]|true|none|Top 4 ranking of factions active in faction warfare by total kills. A faction is considered "active" if they have participated in faction warfare in the past 14 days|
|»» amount|integer(int64)|false|none|Amount of kills|
|»» faction_id|integer(int64)|false|none|none|
|» last_week|[object]|true|none|Top 4 ranking of factions by kills in the past week|
|»» amount|integer(int64)|false|none|Amount of kills|
|»» faction_id|integer(int64)|false|none|none|
|» yesterday|[object]|true|none|Top 4 ranking of factions by kills in the past day|
|»» amount|integer(int64)|false|none|Amount of kills|
|»» faction_id|integer(int64)|false|none|none|
|victory_points|object|true|none|Top 4 rankings of factions by victory points from yesterday, last week and in total|
|» active_total|[object]|true|none|Top 4 ranking of factions active in faction warfare by total victory points. A faction is considered "active" if they have participated in faction warfare in the past 14 days|
|»» amount|integer(int64)|false|none|Amount of victory points|
|»» faction_id|integer(int64)|false|none|none|
|» last_week|[object]|true|none|Top 4 ranking of factions by victory points in the past week|
|»» amount|integer(int64)|false|none|Amount of victory points|
|»» faction_id|integer(int64)|false|none|none|
|» yesterday|[object]|true|none|Top 4 ranking of factions by victory points in the past day|
|»» amount|integer(int64)|false|none|Amount of victory points|
|»» faction_id|integer(int64)|false|none|none|

<h2 id="tocS_FwStatsGet">FwStatsGet</h2>
<!-- backwards compatibility -->
<a id="schemafwstatsget"></a>
<a id="schema_FwStatsGet"></a>
<a id="tocSfwstatsget"></a>
<a id="tocsfwstatsget"></a>

```json
[
  {
    "faction_id": 0,
    "kills": {
      "last_week": 0,
      "total": 0,
      "yesterday": 0
    },
    "pilots": 0,
    "systems_controlled": 0,
    "victory_points": {
      "last_week": 0,
      "total": 0,
      "yesterday": 0
    }
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|faction_id|integer(int64)|true|none|none|
|kills|object|true|none|Summary of kills against an enemy faction for the given faction|
|» last_week|integer(int64)|true|none|Last week's total number of kills against enemy factions|
|» total|integer(int64)|true|none|Total number of kills against enemy factions since faction warfare began|
|» yesterday|integer(int64)|true|none|Yesterday's total number of kills against enemy factions|
|pilots|integer(int64)|true|none|How many pilots fight for the given faction|
|systems_controlled|integer(int64)|true|none|The number of solar systems controlled by the given faction|
|victory_points|object|true|none|Summary of victory points gained for the given faction|
|» last_week|integer(int64)|true|none|Last week's victory points gained|
|» total|integer(int64)|true|none|Total victory points gained since faction warfare began|
|» yesterday|integer(int64)|true|none|Yesterday's victory points gained|

<h2 id="tocS_FwSystemsGet">FwSystemsGet</h2>
<!-- backwards compatibility -->
<a id="schemafwsystemsget"></a>
<a id="schema_FwSystemsGet"></a>
<a id="tocSfwsystemsget"></a>
<a id="tocsfwsystemsget"></a>

```json
[
  {
    "contested": "captured",
    "occupier_faction_id": 0,
    "owner_faction_id": 0,
    "solar_system_id": 0,
    "victory_points": 0,
    "victory_points_threshold": 0
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|contested|string|true|none|none|
|occupier_faction_id|integer(int64)|true|none|none|
|owner_faction_id|integer(int64)|true|none|none|
|solar_system_id|integer(int64)|true|none|none|
|victory_points|integer(int64)|true|none|none|
|victory_points_threshold|integer(int64)|true|none|none|

#### Enumerated Values

|Property|Value|
|---|---|
|contested|captured|
|contested|contested|
|contested|uncontested|
|contested|vulnerable|

<h2 id="tocS_FwWarsGet">FwWarsGet</h2>
<!-- backwards compatibility -->
<a id="schemafwwarsget"></a>
<a id="schema_FwWarsGet"></a>
<a id="tocSfwwarsget"></a>
<a id="tocsfwwarsget"></a>

```json
[
  {
    "against_id": 0,
    "faction_id": 0
  }
]

```

List of factions at war

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|against_id|integer(int64)|true|none|The faction ID of the enemy faction.|
|faction_id|integer(int64)|true|none|none|

<h2 id="tocS_GroupID">GroupID</h2>
<!-- backwards compatibility -->
<a id="schemagroupid"></a>
<a id="schema_GroupID"></a>
<a id="tocSgroupid"></a>
<a id="tocsgroupid"></a>

```json
1559

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|integer(int64)|false|none|none|

<h2 id="tocS_IncursionsGet">IncursionsGet</h2>
<!-- backwards compatibility -->
<a id="schemaincursionsget"></a>
<a id="schema_IncursionsGet"></a>
<a id="tocSincursionsget"></a>
<a id="tocsincursionsget"></a>

```json
[
  {
    "constellation_id": 0,
    "faction_id": 0,
    "has_boss": true,
    "infested_solar_systems": [
      0
    ],
    "influence": 0.1,
    "staging_solar_system_id": 0,
    "state": "withdrawing",
    "type": "string"
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|constellation_id|integer(int64)|true|none|The constellation id in which this incursion takes place|
|faction_id|integer(int64)|true|none|The attacking faction's id|
|has_boss|boolean|true|none|Whether the final encounter has boss or not|
|infested_solar_systems|[integer]|true|none|A list of infested solar system ids that are a part of this incursion|
|influence|number(double)|true|none|Influence of this incursion as a float from 0 to 1|
|staging_solar_system_id|integer(int64)|true|none|Staging solar system for this incursion|
|state|string|true|none|The state of this incursion|
|type|string|true|none|The type of this incursion|

#### Enumerated Values

|Property|Value|
|---|---|
|state|withdrawing|
|state|mobilizing|
|state|established|

<h2 id="tocS_IndustryFacilitiesGet">IndustryFacilitiesGet</h2>
<!-- backwards compatibility -->
<a id="schemaindustryfacilitiesget"></a>
<a id="schema_IndustryFacilitiesGet"></a>
<a id="tocSindustryfacilitiesget"></a>
<a id="tocsindustryfacilitiesget"></a>

```json
[
  {
    "facility_id": 0,
    "owner_id": 0,
    "region_id": 0,
    "solar_system_id": 0,
    "tax": 0.1,
    "type_id": 0
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|facility_id|integer(int64)|true|none|ID of the facility|
|owner_id|integer(int64)|true|none|Owner of the facility|
|region_id|integer(int64)|true|none|Region ID where the facility is|
|solar_system_id|integer(int64)|true|none|Solar system ID where the facility is|
|tax|number(double)|false|none|Tax imposed by the facility|
|type_id|integer(int64)|true|none|Type ID of the facility|

<h2 id="tocS_IndustrySystemsGet">IndustrySystemsGet</h2>
<!-- backwards compatibility -->
<a id="schemaindustrysystemsget"></a>
<a id="schema_IndustrySystemsGet"></a>
<a id="tocSindustrysystemsget"></a>
<a id="tocsindustrysystemsget"></a>

```json
[
  {
    "cost_indices": [
      {
        "activity": "copying",
        "cost_index": 0.1
      }
    ],
    "solar_system_id": 0
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|cost_indices|[object]|true|none|none|
|» activity|string|true|none|none|
|» cost_index|number(double)|true|none|none|
|solar_system_id|integer(int64)|true|none|none|

#### Enumerated Values

|Property|Value|
|---|---|
|activity|copying|
|activity|duplicating|
|activity|invention|
|activity|manufacturing|
|activity|none|
|activity|reaction|
|activity|researching_material_efficiency|
|activity|researching_technology|
|activity|researching_time_efficiency|
|activity|reverse_engineering|

<h2 id="tocS_InsurancePricesGet">InsurancePricesGet</h2>
<!-- backwards compatibility -->
<a id="schemainsurancepricesget"></a>
<a id="schema_InsurancePricesGet"></a>
<a id="tocSinsurancepricesget"></a>
<a id="tocsinsurancepricesget"></a>

```json
[
  {
    "levels": [
      {
        "cost": 0.1,
        "name": "string",
        "payout": 0.1
      }
    ],
    "type_id": 0
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|levels|[object]|true|none|A list of a available insurance levels for this ship type|
|» cost|number(double)|true|none|none|
|» name|string|true|none|Localized insurance level|
|» payout|number(double)|true|none|none|
|type_id|integer(int64)|true|none|none|

<h2 id="tocS_ItemID">ItemID</h2>
<!-- backwards compatibility -->
<a id="schemaitemid"></a>
<a id="schema_ItemID"></a>
<a id="tocSitemid"></a>
<a id="tocsitemid"></a>

```json
1000000000001

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|integer(int64)|false|none|none|

<h2 id="tocS_KillmailsKillmailIdKillmailHashGet">KillmailsKillmailIdKillmailHashGet</h2>
<!-- backwards compatibility -->
<a id="schemakillmailskillmailidkillmailhashget"></a>
<a id="schema_KillmailsKillmailIdKillmailHashGet"></a>
<a id="tocSkillmailskillmailidkillmailhashget"></a>
<a id="tocskillmailskillmailidkillmailhashget"></a>

```json
{
  "attackers": [
    {
      "alliance_id": 0,
      "character_id": 0,
      "corporation_id": 0,
      "damage_done": 0,
      "faction_id": 0,
      "final_blow": true,
      "security_status": 0.1,
      "ship_type_id": 0,
      "weapon_type_id": 0
    }
  ],
  "killmail_id": 0,
  "killmail_time": "2019-08-24T14:15:22Z",
  "moon_id": 0,
  "solar_system_id": 0,
  "victim": {
    "alliance_id": 0,
    "character_id": 0,
    "corporation_id": 0,
    "damage_taken": 0,
    "faction_id": 0,
    "items": [
      {
        "flag": 0,
        "item_type_id": 0,
        "items": [
          {
            "flag": 0,
            "item_type_id": 0,
            "quantity_destroyed": 0,
            "quantity_dropped": 0,
            "singleton": 0
          }
        ],
        "quantity_destroyed": 0,
        "quantity_dropped": 0,
        "singleton": 0
      }
    ],
    "position": {
      "x": 0.1,
      "y": 0.1,
      "z": 0.1
    },
    "ship_type_id": 0
  },
  "war_id": 0
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|attackers|[object]|true|none|none|
|» alliance_id|integer(int64)|false|none|none|
|» character_id|integer(int64)|false|none|none|
|» corporation_id|integer(int64)|false|none|none|
|» damage_done|integer(int64)|true|none|none|
|» faction_id|integer(int64)|false|none|none|
|» final_blow|boolean|true|none|Was the attacker the one to achieve the final blow|
|» security_status|number(double)|true|none|Security status for the attacker|
|» ship_type_id|integer(int64)|false|none|What ship was the attacker flying|
|» weapon_type_id|integer(int64)|false|none|What weapon was used by the attacker for the kill|
|killmail_id|integer(int64)|true|none|ID of the killmail|
|killmail_time|string(date-time)|true|none|Time that the victim was killed and the killmail generated|
|moon_id|integer(int64)|false|none|Moon if the kill took place at one|
|solar_system_id|integer(int64)|true|none|Solar system that the kill took place in|
|victim|object|true|none|none|
|» alliance_id|integer(int64)|false|none|none|
|» character_id|integer(int64)|false|none|none|
|» corporation_id|integer(int64)|false|none|none|
|» damage_taken|integer(int64)|true|none|How much total damage was taken by the victim|
|» faction_id|integer(int64)|false|none|none|
|» items|[object]|false|none|none|
|»» flag|integer(int64)|true|none|Flag for the location of the item|
|»» item_type_id|integer(int64)|true|none|none|
|»» items|[object]|false|none|none|
|»»» flag|integer(int64)|true|none|none|
|»»» item_type_id|integer(int64)|true|none|none|
|»»» quantity_destroyed|integer(int64)|false|none|none|
|»»» quantity_dropped|integer(int64)|false|none|none|
|»»» singleton|integer(int64)|true|none|none|
|»» quantity_destroyed|integer(int64)|false|none|How many of the item were destroyed if any|
|»» quantity_dropped|integer(int64)|false|none|How many of the item were dropped if any|
|»» singleton|integer(int64)|true|none|none|
|» position|object|false|none|Coordinates of the victim in Cartesian space relative to the Sun|
|»» x|number(double)|true|none|none|
|»» y|number(double)|true|none|none|
|»» z|number(double)|true|none|none|
|» ship_type_id|integer(int64)|true|none|The ship that the victim was piloting and was destroyed|
|war_id|integer(int64)|false|none|War if the killmail is generated in relation to an official war|

<h2 id="tocS_LoyaltyStoresCorporationIdOffersGet">LoyaltyStoresCorporationIdOffersGet</h2>
<!-- backwards compatibility -->
<a id="schemaloyaltystorescorporationidoffersget"></a>
<a id="schema_LoyaltyStoresCorporationIdOffersGet"></a>
<a id="tocSloyaltystorescorporationidoffersget"></a>
<a id="tocsloyaltystorescorporationidoffersget"></a>

```json
[
  {
    "ak_cost": 0,
    "isk_cost": 0,
    "lp_cost": 0,
    "offer_id": 0,
    "quantity": 0,
    "required_items": [
      {
        "quantity": 0,
        "type_id": 0
      }
    ],
    "type_id": 0
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|ak_cost|integer(int64)|false|none|Analysis kredit cost|
|isk_cost|integer(int64)|true|none|none|
|lp_cost|integer(int64)|true|none|none|
|offer_id|integer(int64)|true|none|none|
|quantity|integer(int64)|true|none|none|
|required_items|[object]|true|none|none|
|» quantity|integer(int64)|true|none|none|
|» type_id|integer(int64)|true|none|none|
|type_id|integer(int64)|true|none|none|

<h2 id="tocS_MarketsGroupsGet">MarketsGroupsGet</h2>
<!-- backwards compatibility -->
<a id="schemamarketsgroupsget"></a>
<a id="schema_MarketsGroupsGet"></a>
<a id="tocSmarketsgroupsget"></a>
<a id="tocsmarketsgroupsget"></a>

```json
[
  0
]

```

### Properties

*None*

<h2 id="tocS_MarketsGroupsMarketGroupIdGet">MarketsGroupsMarketGroupIdGet</h2>
<!-- backwards compatibility -->
<a id="schemamarketsgroupsmarketgroupidget"></a>
<a id="schema_MarketsGroupsMarketGroupIdGet"></a>
<a id="tocSmarketsgroupsmarketgroupidget"></a>
<a id="tocsmarketsgroupsmarketgroupidget"></a>

```json
{
  "description": "string",
  "market_group_id": 0,
  "name": "string",
  "parent_group_id": 0,
  "types": [
    0
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|description|string|true|none|none|
|market_group_id|integer(int64)|true|none|none|
|name|string|true|none|none|
|parent_group_id|integer(int64)|false|none|none|
|types|[integer]|true|none|none|

<h2 id="tocS_MarketsPricesGet">MarketsPricesGet</h2>
<!-- backwards compatibility -->
<a id="schemamarketspricesget"></a>
<a id="schema_MarketsPricesGet"></a>
<a id="tocSmarketspricesget"></a>
<a id="tocsmarketspricesget"></a>

```json
[
  {
    "adjusted_price": 0.1,
    "average_price": 0.1,
    "type_id": 0
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|adjusted_price|number(double)|false|none|none|
|average_price|number(double)|false|none|none|
|type_id|integer(int64)|true|none|none|

<h2 id="tocS_MarketsRegionIdHistoryGet">MarketsRegionIdHistoryGet</h2>
<!-- backwards compatibility -->
<a id="schemamarketsregionidhistoryget"></a>
<a id="schema_MarketsRegionIdHistoryGet"></a>
<a id="tocSmarketsregionidhistoryget"></a>
<a id="tocsmarketsregionidhistoryget"></a>

```json
[
  {
    "average": 0.1,
    "date": "2019-08-24",
    "highest": 0.1,
    "lowest": 0.1,
    "order_count": 0,
    "volume": 0
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|average|number(double)|true|none|none|
|date|string(date)|true|none|The date of this historical statistic entry|
|highest|number(double)|true|none|none|
|lowest|number(double)|true|none|none|
|order_count|integer(int64)|true|none|Total number of orders happened that day|
|volume|integer(int64)|true|none|Total|

<h2 id="tocS_MarketsRegionIdOrdersGet">MarketsRegionIdOrdersGet</h2>
<!-- backwards compatibility -->
<a id="schemamarketsregionidordersget"></a>
<a id="schema_MarketsRegionIdOrdersGet"></a>
<a id="tocSmarketsregionidordersget"></a>
<a id="tocsmarketsregionidordersget"></a>

```json
[
  {
    "duration": 0,
    "is_buy_order": true,
    "issued": "2019-08-24T14:15:22Z",
    "location_id": 0,
    "min_volume": 0,
    "order_id": 0,
    "price": 0.1,
    "range": "station",
    "system_id": 0,
    "type_id": 0,
    "volume_remain": 0,
    "volume_total": 0
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|duration|integer(int64)|true|none|none|
|is_buy_order|boolean|true|none|none|
|issued|string(date-time)|true|none|none|
|location_id|integer(int64)|true|none|none|
|min_volume|integer(int64)|true|none|none|
|order_id|integer(int64)|true|none|none|
|price|number(double)|true|none|none|
|range|string|true|none|none|
|system_id|integer(int64)|true|none|The solar system this order was placed|
|type_id|integer(int64)|true|none|none|
|volume_remain|integer(int64)|true|none|none|
|volume_total|integer(int64)|true|none|none|

#### Enumerated Values

|Property|Value|
|---|---|
|range|station|
|range|region|
|range|solarsystem|
|range|1|
|range|2|
|range|3|
|range|4|
|range|5|
|range|10|
|range|20|
|range|30|
|range|40|

<h2 id="tocS_MarketsRegionIdTypesGet">MarketsRegionIdTypesGet</h2>
<!-- backwards compatibility -->
<a id="schemamarketsregionidtypesget"></a>
<a id="schema_MarketsRegionIdTypesGet"></a>
<a id="tocSmarketsregionidtypesget"></a>
<a id="tocsmarketsregionidtypesget"></a>

```json
[
  0
]

```

### Properties

*None*

<h2 id="tocS_MarketsStructuresStructureIdGet">MarketsStructuresStructureIdGet</h2>
<!-- backwards compatibility -->
<a id="schemamarketsstructuresstructureidget"></a>
<a id="schema_MarketsStructuresStructureIdGet"></a>
<a id="tocSmarketsstructuresstructureidget"></a>
<a id="tocsmarketsstructuresstructureidget"></a>

```json
[
  {
    "duration": 0,
    "is_buy_order": true,
    "issued": "2019-08-24T14:15:22Z",
    "location_id": 0,
    "min_volume": 0,
    "order_id": 0,
    "price": 0.1,
    "range": "station",
    "type_id": 0,
    "volume_remain": 0,
    "volume_total": 0
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|duration|integer(int64)|true|none|none|
|is_buy_order|boolean|true|none|none|
|issued|string(date-time)|true|none|none|
|location_id|integer(int64)|true|none|none|
|min_volume|integer(int64)|true|none|none|
|order_id|integer(int64)|true|none|none|
|price|number(double)|true|none|none|
|range|string|true|none|none|
|type_id|integer(int64)|true|none|none|
|volume_remain|integer(int64)|true|none|none|
|volume_total|integer(int64)|true|none|none|

#### Enumerated Values

|Property|Value|
|---|---|
|range|station|
|range|region|
|range|solarsystem|
|range|1|
|range|2|
|range|3|
|range|4|
|range|5|
|range|10|
|range|20|
|range|30|
|range|40|

<h2 id="tocS_MetaChangelog">MetaChangelog</h2>
<!-- backwards compatibility -->
<a id="schemametachangelog"></a>
<a id="schema_MetaChangelog"></a>
<a id="tocSmetachangelog"></a>
<a id="tocsmetachangelog"></a>

```json
{
  "changelog": {
    "property1": [
      {
        "compatibility_date": "2025-08-26",
        "description": "Updated response schema.",
        "method": "GET",
        "path": "/meta/changelog",
        "type": "breaking"
      }
    ],
    "property2": [
      {
        "compatibility_date": "2025-08-26",
        "description": "Updated response schema.",
        "method": "GET",
        "path": "/meta/changelog",
        "type": "breaking"
      }
    ]
  }
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|changelog|object|true|none|Per date, list changes for that date|
|» **additionalProperties**|[[MetaChangelogEntry](#schemametachangelogentry)]|false|none|none|

<h2 id="tocS_MetaChangelogEntry">MetaChangelogEntry</h2>
<!-- backwards compatibility -->
<a id="schemametachangelogentry"></a>
<a id="schema_MetaChangelogEntry"></a>
<a id="tocSmetachangelogentry"></a>
<a id="tocsmetachangelogentry"></a>

```json
{
  "compatibility_date": "2025-08-26",
  "description": "Updated response schema.",
  "method": "GET",
  "path": "/meta/changelog",
  "type": "breaking"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|compatibility_date|[CompatibilityDate](#schemacompatibilitydate)|true|none|Compatibility date of the route|
|description|string|true|none|Description|
|method|string|true|none|HTTP method of the route|
|path|string|true|none|Path of the route|
|type|string|true|none|Type of the change|

#### Enumerated Values

|Property|Value|
|---|---|
|method|GET|
|method|POST|
|method|PUT|
|method|DELETE|
|type|breaking|
|type|changed|
|type|new|
|type|removed|

<h2 id="tocS_MetaCompatibilityDates">MetaCompatibilityDates</h2>
<!-- backwards compatibility -->
<a id="schemametacompatibilitydates"></a>
<a id="schema_MetaCompatibilityDates"></a>
<a id="tocSmetacompatibilitydates"></a>
<a id="tocsmetacompatibilitydates"></a>

```json
{
  "compatibility_dates": [
    "2025-08-26"
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|compatibility_dates|[[CompatibilityDate](#schemacompatibilitydate)]|true|none|List of compatibility dates.|

<h2 id="tocS_MetaStatus">MetaStatus</h2>
<!-- backwards compatibility -->
<a id="schemametastatus"></a>
<a id="schema_MetaStatus"></a>
<a id="tocSmetastatus"></a>
<a id="tocsmetastatus"></a>

```json
{
  "routes": [
    {
      "method": "GET",
      "path": "string",
      "status": "Unknown"
    }
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|routes|[[MetaStatusRoutestatus](#schemametastatusroutestatus)]|true|none|List of all API routes and their health status|

<h2 id="tocS_MetaStatusRoutestatus">MetaStatusRoutestatus</h2>
<!-- backwards compatibility -->
<a id="schemametastatusroutestatus"></a>
<a id="schema_MetaStatusRoutestatus"></a>
<a id="tocSmetastatusroutestatus"></a>
<a id="tocsmetastatusroutestatus"></a>

```json
{
  "method": "GET",
  "path": "string",
  "status": "Unknown"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|method|string|true|none|Route's HTTP method|
|path|string|true|none|Route's HTTP path|
|status|string|true|none|Route's health status|

#### Enumerated Values

|Property|Value|
|---|---|
|method|GET|
|method|POST|
|method|PUT|
|method|DELETE|
|status|Unknown|
|status|OK|
|status|Degraded|
|status|Down|
|status|Recovering|

<h2 id="tocS_RegionID">RegionID</h2>
<!-- backwards compatibility -->
<a id="schemaregionid"></a>
<a id="schema_RegionID"></a>
<a id="tocSregionid"></a>
<a id="tocsregionid"></a>

```json
10000001

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|integer(int64)|false|none|none|

<h2 id="tocS_Route">Route</h2>
<!-- backwards compatibility -->
<a id="schemaroute"></a>
<a id="schema_Route"></a>
<a id="tocSroute"></a>
<a id="tocsroute"></a>

```json
{
  "route": [
    30000001
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|route|[[SolarSystemID](#schemasolarsystemid)]|true|none|The route between the origin and destination systems|

<h2 id="tocS_RouteConnection">RouteConnection</h2>
<!-- backwards compatibility -->
<a id="schemarouteconnection"></a>
<a id="schema_RouteConnection"></a>
<a id="tocSrouteconnection"></a>
<a id="tocsrouteconnection"></a>

```json
{
  "from": 30000001,
  "to": 30000001
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|from|[SolarSystemID](#schemasolarsystemid)|true|none|From which system|
|to|[SolarSystemID](#schemasolarsystemid)|true|none|To which system|

<h2 id="tocS_RouteRequestBody">RouteRequestBody</h2>
<!-- backwards compatibility -->
<a id="schemarouterequestbody"></a>
<a id="schema_RouteRequestBody"></a>
<a id="tocSrouterequestbody"></a>
<a id="tocsrouterequestbody"></a>

```json
{
  "avoid_systems": [
    30000001
  ],
  "connections": [
    {
      "from": 30000001,
      "to": 30000001
    }
  ],
  "preference": "Shorter",
  "security_penalty": 50
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|avoid_systems|[[SolarSystemID](#schemasolarsystemid)]|false|none|Systems to avoid|
|connections|[[RouteConnection](#schemarouteconnection)]|false|none|Additional one-way connections (like Jump Bridges) between systems|
|preference|string|false|none|Preference for the route|
|security_penalty|integer(int64)|false|none|Strictness of the path preference|

#### Enumerated Values

|Property|Value|
|---|---|
|preference|Shorter|
|preference|Safer|
|preference|LessSecure|

<h2 id="tocS_ShipTreeGroupID">ShipTreeGroupID</h2>
<!-- backwards compatibility -->
<a id="schemashiptreegroupid"></a>
<a id="schema_ShipTreeGroupID"></a>
<a id="tocSshiptreegroupid"></a>
<a id="tocsshiptreegroupid"></a>

```json
1559

```

Ship tree group identifier.

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|integer(int64)|false|none|Ship tree group identifier.|

<h2 id="tocS_SolarSystemID">SolarSystemID</h2>
<!-- backwards compatibility -->
<a id="schemasolarsystemid"></a>
<a id="schema_SolarSystemID"></a>
<a id="tocSsolarsystemid"></a>
<a id="tocssolarsystemid"></a>

```json
30000001

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|integer(int64)|false|none|none|

<h2 id="tocS_SovereigntyCampaignsGet">SovereigntyCampaignsGet</h2>
<!-- backwards compatibility -->
<a id="schemasovereigntycampaignsget"></a>
<a id="schema_SovereigntyCampaignsGet"></a>
<a id="tocSsovereigntycampaignsget"></a>
<a id="tocssovereigntycampaignsget"></a>

```json
[
  {
    "attackers_score": 0.1,
    "campaign_id": 0,
    "constellation_id": 0,
    "defender_id": 0,
    "defender_score": 0.1,
    "event_type": "tcu_defense",
    "participants": [
      {
        "alliance_id": 0,
        "score": 0.1
      }
    ],
    "solar_system_id": 0,
    "start_time": "2019-08-24T14:15:22Z",
    "structure_id": 0
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|attackers_score|number(double)|false|none|Score for all attacking parties, only present in Defense Events.|
|campaign_id|integer(int64)|true|none|Unique ID for this campaign.|
|constellation_id|integer(int64)|true|none|The constellation in which the campaign will take place.|
|defender_id|integer(int64)|false|none|Defending alliance, only present in Defense Events|
|defender_score|number(double)|false|none|Score for the defending alliance, only present in Defense Events.|
|event_type|string|true|none|Type of event this campaign is for. tcu_defense, ihub_defense and station_defense are referred to as "Defense Events", station_freeport as "Freeport Events".|
|participants|[object]|false|none|Alliance participating and their respective scores, only present in Freeport Events.|
|» alliance_id|integer(int64)|true|none|none|
|» score|number(double)|true|none|none|
|solar_system_id|integer(int64)|true|none|The solar system the structure is located in.|
|start_time|string(date-time)|true|none|Time the event is scheduled to start.|
|structure_id|integer(int64)|true|none|The structure item ID that is related to this campaign.|

#### Enumerated Values

|Property|Value|
|---|---|
|event_type|tcu_defense|
|event_type|ihub_defense|
|event_type|station_defense|
|event_type|station_freeport|

<h2 id="tocS_SovereigntyMapGet">SovereigntyMapGet</h2>
<!-- backwards compatibility -->
<a id="schemasovereigntymapget"></a>
<a id="schema_SovereigntyMapGet"></a>
<a id="tocSsovereigntymapget"></a>
<a id="tocssovereigntymapget"></a>

```json
[
  {
    "alliance_id": 0,
    "corporation_id": 0,
    "faction_id": 0,
    "system_id": 0
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|alliance_id|integer(int64)|false|none|none|
|corporation_id|integer(int64)|false|none|none|
|faction_id|integer(int64)|false|none|none|
|system_id|integer(int64)|true|none|none|

<h2 id="tocS_SovereigntyStructuresGet">SovereigntyStructuresGet</h2>
<!-- backwards compatibility -->
<a id="schemasovereigntystructuresget"></a>
<a id="schema_SovereigntyStructuresGet"></a>
<a id="tocSsovereigntystructuresget"></a>
<a id="tocssovereigntystructuresget"></a>

```json
[
  {
    "alliance_id": 0,
    "solar_system_id": 0,
    "structure_id": 0,
    "structure_type_id": 0,
    "vulnerability_occupancy_level": 0.1,
    "vulnerable_end_time": "2019-08-24T14:15:22Z",
    "vulnerable_start_time": "2019-08-24T14:15:22Z"
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|alliance_id|integer(int64)|true|none|The alliance that owns the structure.|
|solar_system_id|integer(int64)|true|none|Solar system in which the structure is located.|
|structure_id|integer(int64)|true|none|Unique item ID for this structure.|
|structure_type_id|integer(int64)|true|none|A reference to the type of structure this is.|
|vulnerability_occupancy_level|number(double)|false|none|The occupancy level for the next or current vulnerability window. This takes into account all development indexes and capital system bonuses. Also known as Activity Defense Multiplier from in the client. It increases the time that attackers must spend using their entosis links on the structure.|
|vulnerable_end_time|string(date-time)|false|none|The time at which the next or current vulnerability window ends. At the end of a vulnerability window the next window is recalculated and locked in along with the vulnerabilityOccupancyLevel. If the structure is not in 100% entosis control of the defender, it will go in to 'overtime' and stay vulnerable for as long as that situation persists. Only once the defenders have 100% entosis control and has the vulnerableEndTime passed does the vulnerability interval expire and a new one is calculated.|
|vulnerable_start_time|string(date-time)|false|none|The next time at which the structure will become vulnerable. Or the start time of the current window if current time is between this and vulnerableEndTime.|

<h2 id="tocS_StationID">StationID</h2>
<!-- backwards compatibility -->
<a id="schemastationid"></a>
<a id="schema_StationID"></a>
<a id="tocSstationid"></a>
<a id="tocsstationid"></a>

```json
60000001

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|integer(int64)|false|none|none|

<h2 id="tocS_StatusGet">StatusGet</h2>
<!-- backwards compatibility -->
<a id="schemastatusget"></a>
<a id="schema_StatusGet"></a>
<a id="tocSstatusget"></a>
<a id="tocsstatusget"></a>

```json
{
  "players": 0,
  "server_version": "string",
  "start_time": "2019-08-24T14:15:22Z",
  "vip": true
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|players|integer|true|none|Current online player count|
|server_version|string|true|none|Running version as string|
|start_time|string(date-time)|true|none|Server start timestamp|
|vip|boolean|false|none|If the server is in VIP mode|

<h2 id="tocS_TypeID">TypeID</h2>
<!-- backwards compatibility -->
<a id="schematypeid"></a>
<a id="schema_TypeID"></a>
<a id="tocStypeid"></a>
<a id="tocstypeid"></a>

```json
587

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|integer(int64)|false|none|none|

<h2 id="tocS_UUID">UUID</h2>
<!-- backwards compatibility -->
<a id="schemauuid"></a>
<a id="schema_UUID"></a>
<a id="tocSuuid"></a>
<a id="tocsuuid"></a>

```json
"3868eaed-8278-4cb7-9709-7d7de9c20dc7"

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|string(uuid)|false|none|none|

<h2 id="tocS_UniverseAncestriesGet">UniverseAncestriesGet</h2>
<!-- backwards compatibility -->
<a id="schemauniverseancestriesget"></a>
<a id="schema_UniverseAncestriesGet"></a>
<a id="tocSuniverseancestriesget"></a>
<a id="tocsuniverseancestriesget"></a>

```json
[
  {
    "bloodline_id": 0,
    "description": "string",
    "icon_id": 0,
    "id": 0,
    "name": "string",
    "short_description": "string"
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|bloodline_id|integer(int64)|true|none|The bloodline associated with this ancestry|
|description|string|true|none|none|
|icon_id|integer(int64)|false|none|none|
|id|integer(int64)|true|none|none|
|name|string|true|none|none|
|short_description|string|false|none|none|

<h2 id="tocS_UniverseAsteroidBeltsAsteroidBeltIdGet">UniverseAsteroidBeltsAsteroidBeltIdGet</h2>
<!-- backwards compatibility -->
<a id="schemauniverseasteroidbeltsasteroidbeltidget"></a>
<a id="schema_UniverseAsteroidBeltsAsteroidBeltIdGet"></a>
<a id="tocSuniverseasteroidbeltsasteroidbeltidget"></a>
<a id="tocsuniverseasteroidbeltsasteroidbeltidget"></a>

```json
{
  "name": "string",
  "position": {
    "x": 0.1,
    "y": 0.1,
    "z": 0.1
  },
  "system_id": 0
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|name|string|true|none|none|
|position|object|true|none|none|
|» x|number(double)|true|none|none|
|» y|number(double)|true|none|none|
|» z|number(double)|true|none|none|
|system_id|integer(int64)|true|none|The solar system this asteroid belt is in|

<h2 id="tocS_UniverseBloodlinesGet">UniverseBloodlinesGet</h2>
<!-- backwards compatibility -->
<a id="schemauniversebloodlinesget"></a>
<a id="schema_UniverseBloodlinesGet"></a>
<a id="tocSuniversebloodlinesget"></a>
<a id="tocsuniversebloodlinesget"></a>

```json
[
  {
    "bloodline_id": 0,
    "charisma": 0,
    "corporation_id": 0,
    "description": "string",
    "intelligence": 0,
    "memory": 0,
    "name": "string",
    "perception": 0,
    "race_id": 0,
    "ship_type_id": 0,
    "willpower": 0
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|bloodline_id|integer(int64)|true|none|none|
|charisma|integer(int64)|true|none|none|
|corporation_id|integer(int64)|true|none|none|
|description|string|true|none|none|
|intelligence|integer(int64)|true|none|none|
|memory|integer(int64)|true|none|none|
|name|string|true|none|none|
|perception|integer(int64)|true|none|none|
|race_id|integer(int64)|true|none|none|
|ship_type_id|integer(int64)|true|none|none|
|willpower|integer(int64)|true|none|none|

<h2 id="tocS_UniverseCategoriesCategoryIdGet">UniverseCategoriesCategoryIdGet</h2>
<!-- backwards compatibility -->
<a id="schemauniversecategoriescategoryidget"></a>
<a id="schema_UniverseCategoriesCategoryIdGet"></a>
<a id="tocSuniversecategoriescategoryidget"></a>
<a id="tocsuniversecategoriescategoryidget"></a>

```json
{
  "category_id": 0,
  "groups": [
    0
  ],
  "name": "string",
  "published": true
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|category_id|integer(int64)|true|none|none|
|groups|[integer]|true|none|none|
|name|string|true|none|none|
|published|boolean|true|none|none|

<h2 id="tocS_UniverseCategoriesGet">UniverseCategoriesGet</h2>
<!-- backwards compatibility -->
<a id="schemauniversecategoriesget"></a>
<a id="schema_UniverseCategoriesGet"></a>
<a id="tocSuniversecategoriesget"></a>
<a id="tocsuniversecategoriesget"></a>

```json
[
  0
]

```

### Properties

*None*

<h2 id="tocS_UniverseConstellationsConstellationIdGet">UniverseConstellationsConstellationIdGet</h2>
<!-- backwards compatibility -->
<a id="schemauniverseconstellationsconstellationidget"></a>
<a id="schema_UniverseConstellationsConstellationIdGet"></a>
<a id="tocSuniverseconstellationsconstellationidget"></a>
<a id="tocsuniverseconstellationsconstellationidget"></a>

```json
{
  "constellation_id": 0,
  "name": "string",
  "position": {
    "x": 0.1,
    "y": 0.1,
    "z": 0.1
  },
  "region_id": 0,
  "systems": [
    0
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|constellation_id|integer(int64)|true|none|none|
|name|string|true|none|none|
|position|object|true|none|none|
|» x|number(double)|true|none|none|
|» y|number(double)|true|none|none|
|» z|number(double)|true|none|none|
|region_id|integer(int64)|true|none|The region this constellation is in|
|systems|[integer]|true|none|none|

<h2 id="tocS_UniverseConstellationsGet">UniverseConstellationsGet</h2>
<!-- backwards compatibility -->
<a id="schemauniverseconstellationsget"></a>
<a id="schema_UniverseConstellationsGet"></a>
<a id="tocSuniverseconstellationsget"></a>
<a id="tocsuniverseconstellationsget"></a>

```json
[
  0
]

```

### Properties

*None*

<h2 id="tocS_UniverseFactionsGet">UniverseFactionsGet</h2>
<!-- backwards compatibility -->
<a id="schemauniversefactionsget"></a>
<a id="schema_UniverseFactionsGet"></a>
<a id="tocSuniversefactionsget"></a>
<a id="tocsuniversefactionsget"></a>

```json
[
  {
    "corporation_id": 0,
    "description": "string",
    "faction_id": 0,
    "is_unique": true,
    "militia_corporation_id": 0,
    "name": "string",
    "size_factor": 0.1,
    "solar_system_id": 0,
    "station_count": 0,
    "station_system_count": 0
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|corporation_id|integer(int64)|false|none|none|
|description|string|true|none|none|
|faction_id|integer(int64)|true|none|none|
|is_unique|boolean|true|none|none|
|militia_corporation_id|integer(int64)|false|none|none|
|name|string|true|none|none|
|size_factor|number(double)|true|none|none|
|solar_system_id|integer(int64)|false|none|none|
|station_count|integer(int64)|true|none|none|
|station_system_count|integer(int64)|true|none|none|

<h2 id="tocS_UniverseGraphicsGet">UniverseGraphicsGet</h2>
<!-- backwards compatibility -->
<a id="schemauniversegraphicsget"></a>
<a id="schema_UniverseGraphicsGet"></a>
<a id="tocSuniversegraphicsget"></a>
<a id="tocsuniversegraphicsget"></a>

```json
[
  0
]

```

### Properties

*None*

<h2 id="tocS_UniverseGraphicsGraphicIdGet">UniverseGraphicsGraphicIdGet</h2>
<!-- backwards compatibility -->
<a id="schemauniversegraphicsgraphicidget"></a>
<a id="schema_UniverseGraphicsGraphicIdGet"></a>
<a id="tocSuniversegraphicsgraphicidget"></a>
<a id="tocsuniversegraphicsgraphicidget"></a>

```json
{
  "collision_file": "string",
  "graphic_file": "string",
  "graphic_id": 0,
  "icon_folder": "string",
  "sof_dna": "string",
  "sof_fation_name": "string",
  "sof_hull_name": "string",
  "sof_race_name": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|collision_file|string|false|none|none|
|graphic_file|string|false|none|none|
|graphic_id|integer(int64)|true|none|none|
|icon_folder|string|false|none|none|
|sof_dna|string|false|none|none|
|sof_fation_name|string|false|none|none|
|sof_hull_name|string|false|none|none|
|sof_race_name|string|false|none|none|

<h2 id="tocS_UniverseGroupsGet">UniverseGroupsGet</h2>
<!-- backwards compatibility -->
<a id="schemauniversegroupsget"></a>
<a id="schema_UniverseGroupsGet"></a>
<a id="tocSuniversegroupsget"></a>
<a id="tocsuniversegroupsget"></a>

```json
[
  0
]

```

### Properties

*None*

<h2 id="tocS_UniverseGroupsGroupIdGet">UniverseGroupsGroupIdGet</h2>
<!-- backwards compatibility -->
<a id="schemauniversegroupsgroupidget"></a>
<a id="schema_UniverseGroupsGroupIdGet"></a>
<a id="tocSuniversegroupsgroupidget"></a>
<a id="tocsuniversegroupsgroupidget"></a>

```json
{
  "category_id": 0,
  "group_id": 0,
  "name": "string",
  "published": true,
  "types": [
    0
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|category_id|integer(int64)|true|none|none|
|group_id|integer(int64)|true|none|none|
|name|string|true|none|none|
|published|boolean|true|none|none|
|types|[integer]|true|none|none|

<h2 id="tocS_UniverseIdsPost">UniverseIdsPost</h2>
<!-- backwards compatibility -->
<a id="schemauniverseidspost"></a>
<a id="schema_UniverseIdsPost"></a>
<a id="tocSuniverseidspost"></a>
<a id="tocsuniverseidspost"></a>

```json
{
  "agents": [
    {
      "id": 0,
      "name": "string"
    }
  ],
  "alliances": [
    {
      "id": 0,
      "name": "string"
    }
  ],
  "characters": [
    {
      "id": 0,
      "name": "string"
    }
  ],
  "constellations": [
    {
      "id": 0,
      "name": "string"
    }
  ],
  "corporations": [
    {
      "id": 0,
      "name": "string"
    }
  ],
  "factions": [
    {
      "id": 0,
      "name": "string"
    }
  ],
  "inventory_types": [
    {
      "id": 0,
      "name": "string"
    }
  ],
  "regions": [
    {
      "id": 0,
      "name": "string"
    }
  ],
  "stations": [
    {
      "id": 0,
      "name": "string"
    }
  ],
  "systems": [
    {
      "id": 0,
      "name": "string"
    }
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|agents|[object]|false|none|none|
|» id|integer(int64)|false|none|none|
|» name|string|false|none|none|
|alliances|[object]|false|none|none|
|» id|integer(int64)|false|none|none|
|» name|string|false|none|none|
|characters|[object]|false|none|none|
|» id|integer(int64)|false|none|none|
|» name|string|false|none|none|
|constellations|[object]|false|none|none|
|» id|integer(int64)|false|none|none|
|» name|string|false|none|none|
|corporations|[object]|false|none|none|
|» id|integer(int64)|false|none|none|
|» name|string|false|none|none|
|factions|[object]|false|none|none|
|» id|integer(int64)|false|none|none|
|» name|string|false|none|none|
|inventory_types|[object]|false|none|none|
|» id|integer(int64)|false|none|none|
|» name|string|false|none|none|
|regions|[object]|false|none|none|
|» id|integer(int64)|false|none|none|
|» name|string|false|none|none|
|stations|[object]|false|none|none|
|» id|integer(int64)|false|none|none|
|» name|string|false|none|none|
|systems|[object]|false|none|none|
|» id|integer(int64)|false|none|none|
|» name|string|false|none|none|

<h2 id="tocS_UniverseMoonsMoonIdGet">UniverseMoonsMoonIdGet</h2>
<!-- backwards compatibility -->
<a id="schemauniversemoonsmoonidget"></a>
<a id="schema_UniverseMoonsMoonIdGet"></a>
<a id="tocSuniversemoonsmoonidget"></a>
<a id="tocsuniversemoonsmoonidget"></a>

```json
{
  "moon_id": 0,
  "name": "string",
  "position": {
    "x": 0.1,
    "y": 0.1,
    "z": 0.1
  },
  "system_id": 0
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|moon_id|integer(int64)|true|none|none|
|name|string|true|none|none|
|position|object|true|none|none|
|» x|number(double)|true|none|none|
|» y|number(double)|true|none|none|
|» z|number(double)|true|none|none|
|system_id|integer(int64)|true|none|The solar system this moon is in|

<h2 id="tocS_UniverseNamesPost">UniverseNamesPost</h2>
<!-- backwards compatibility -->
<a id="schemauniversenamespost"></a>
<a id="schema_UniverseNamesPost"></a>
<a id="tocSuniversenamespost"></a>
<a id="tocsuniversenamespost"></a>

```json
[
  {
    "category": "alliance",
    "id": 0,
    "name": "string"
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|category|string|true|none|none|
|id|integer(int64)|true|none|none|
|name|string|true|none|none|

#### Enumerated Values

|Property|Value|
|---|---|
|category|alliance|
|category|character|
|category|constellation|
|category|corporation|
|category|inventory_type|
|category|region|
|category|solar_system|
|category|station|
|category|faction|

<h2 id="tocS_UniversePlanetsPlanetIdGet">UniversePlanetsPlanetIdGet</h2>
<!-- backwards compatibility -->
<a id="schemauniverseplanetsplanetidget"></a>
<a id="schema_UniversePlanetsPlanetIdGet"></a>
<a id="tocSuniverseplanetsplanetidget"></a>
<a id="tocsuniverseplanetsplanetidget"></a>

```json
{
  "name": "string",
  "planet_id": 0,
  "position": {
    "x": 0.1,
    "y": 0.1,
    "z": 0.1
  },
  "system_id": 0,
  "type_id": 0
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|name|string|true|none|none|
|planet_id|integer(int64)|true|none|none|
|position|object|true|none|none|
|» x|number(double)|true|none|none|
|» y|number(double)|true|none|none|
|» z|number(double)|true|none|none|
|system_id|integer(int64)|true|none|The solar system this planet is in|
|type_id|integer(int64)|true|none|none|

<h2 id="tocS_UniverseRacesGet">UniverseRacesGet</h2>
<!-- backwards compatibility -->
<a id="schemauniverseracesget"></a>
<a id="schema_UniverseRacesGet"></a>
<a id="tocSuniverseracesget"></a>
<a id="tocsuniverseracesget"></a>

```json
[
  {
    "alliance_id": 0,
    "description": "string",
    "name": "string",
    "race_id": 0
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|alliance_id|integer(int64)|true|none|The alliance generally associated with this race|
|description|string|true|none|none|
|name|string|true|none|none|
|race_id|integer(int64)|true|none|none|

<h2 id="tocS_UniverseRegionsGet">UniverseRegionsGet</h2>
<!-- backwards compatibility -->
<a id="schemauniverseregionsget"></a>
<a id="schema_UniverseRegionsGet"></a>
<a id="tocSuniverseregionsget"></a>
<a id="tocsuniverseregionsget"></a>

```json
[
  0
]

```

### Properties

*None*

<h2 id="tocS_UniverseRegionsRegionIdGet">UniverseRegionsRegionIdGet</h2>
<!-- backwards compatibility -->
<a id="schemauniverseregionsregionidget"></a>
<a id="schema_UniverseRegionsRegionIdGet"></a>
<a id="tocSuniverseregionsregionidget"></a>
<a id="tocsuniverseregionsregionidget"></a>

```json
{
  "constellations": [
    0
  ],
  "description": "string",
  "name": "string",
  "region_id": 0
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|constellations|[integer]|true|none|none|
|description|string|false|none|none|
|name|string|true|none|none|
|region_id|integer(int64)|true|none|none|

<h2 id="tocS_UniverseSchematicsSchematicIdGet">UniverseSchematicsSchematicIdGet</h2>
<!-- backwards compatibility -->
<a id="schemauniverseschematicsschematicidget"></a>
<a id="schema_UniverseSchematicsSchematicIdGet"></a>
<a id="tocSuniverseschematicsschematicidget"></a>
<a id="tocsuniverseschematicsschematicidget"></a>

```json
{
  "cycle_time": 0,
  "schematic_name": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|cycle_time|integer(int64)|true|none|Time in seconds to process a run|
|schematic_name|string|true|none|none|

<h2 id="tocS_UniverseStargatesStargateIdGet">UniverseStargatesStargateIdGet</h2>
<!-- backwards compatibility -->
<a id="schemauniversestargatesstargateidget"></a>
<a id="schema_UniverseStargatesStargateIdGet"></a>
<a id="tocSuniversestargatesstargateidget"></a>
<a id="tocsuniversestargatesstargateidget"></a>

```json
{
  "destination": {
    "stargate_id": 0,
    "system_id": 0
  },
  "name": "string",
  "position": {
    "x": 0.1,
    "y": 0.1,
    "z": 0.1
  },
  "stargate_id": 0,
  "system_id": 0,
  "type_id": 0
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|destination|object|true|none|none|
|» stargate_id|integer(int64)|true|none|The stargate this stargate connects to|
|» system_id|integer(int64)|true|none|The solar system this stargate connects to|
|name|string|true|none|none|
|position|object|true|none|none|
|» x|number(double)|true|none|none|
|» y|number(double)|true|none|none|
|» z|number(double)|true|none|none|
|stargate_id|integer(int64)|true|none|none|
|system_id|integer(int64)|true|none|The solar system this stargate is in|
|type_id|integer(int64)|true|none|none|

<h2 id="tocS_UniverseStarsStarIdGet">UniverseStarsStarIdGet</h2>
<!-- backwards compatibility -->
<a id="schemauniversestarsstaridget"></a>
<a id="schema_UniverseStarsStarIdGet"></a>
<a id="tocSuniversestarsstaridget"></a>
<a id="tocsuniversestarsstaridget"></a>

```json
{
  "age": 0,
  "luminosity": 0.1,
  "name": "string",
  "radius": 0,
  "solar_system_id": 0,
  "spectral_class": "K2 V",
  "temperature": 0,
  "type_id": 0
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|age|integer(int64)|true|none|Age of star in years|
|luminosity|number(double)|true|none|none|
|name|string|true|none|none|
|radius|integer(int64)|true|none|none|
|solar_system_id|integer(int64)|true|none|none|
|spectral_class|string|true|none|none|
|temperature|integer(int64)|true|none|none|
|type_id|integer(int64)|true|none|none|

#### Enumerated Values

|Property|Value|
|---|---|
|spectral_class|K2 V|
|spectral_class|K4 V|
|spectral_class|G2 V|
|spectral_class|G8 V|
|spectral_class|M7 V|
|spectral_class|K7 V|
|spectral_class|M2 V|
|spectral_class|K5 V|
|spectral_class|M3 V|
|spectral_class|G0 V|
|spectral_class|G7 V|
|spectral_class|G3 V|
|spectral_class|F9 V|
|spectral_class|G5 V|
|spectral_class|F6 V|
|spectral_class|K8 V|
|spectral_class|K9 V|
|spectral_class|K6 V|
|spectral_class|G9 V|
|spectral_class|G6 V|
|spectral_class|G4 VI|
|spectral_class|G4 V|
|spectral_class|F8 V|
|spectral_class|F2 V|
|spectral_class|F1 V|
|spectral_class|K3 V|
|spectral_class|F0 VI|
|spectral_class|G1 VI|
|spectral_class|G0 VI|
|spectral_class|K1 V|
|spectral_class|M4 V|
|spectral_class|M1 V|
|spectral_class|M6 V|
|spectral_class|M0 V|
|spectral_class|K2 IV|
|spectral_class|G2 VI|
|spectral_class|K0 V|
|spectral_class|K5 IV|
|spectral_class|F5 VI|
|spectral_class|G6 VI|
|spectral_class|F6 VI|
|spectral_class|F2 IV|
|spectral_class|G3 VI|
|spectral_class|M8 V|
|spectral_class|F1 VI|
|spectral_class|K1 IV|
|spectral_class|F7 V|
|spectral_class|G5 VI|
|spectral_class|M5 V|
|spectral_class|G7 VI|
|spectral_class|F5 V|
|spectral_class|F4 VI|
|spectral_class|F8 VI|
|spectral_class|K3 IV|
|spectral_class|F4 IV|
|spectral_class|F0 V|
|spectral_class|G7 IV|
|spectral_class|G8 VI|
|spectral_class|F2 VI|
|spectral_class|F4 V|
|spectral_class|F7 VI|
|spectral_class|F3 V|
|spectral_class|G1 V|
|spectral_class|G9 VI|
|spectral_class|F3 IV|
|spectral_class|F9 VI|
|spectral_class|M9 V|
|spectral_class|K0 IV|
|spectral_class|F1 IV|
|spectral_class|G4 IV|
|spectral_class|F3 VI|
|spectral_class|K4 IV|
|spectral_class|G5 IV|
|spectral_class|G3 IV|
|spectral_class|G1 IV|
|spectral_class|K7 IV|
|spectral_class|G0 IV|
|spectral_class|K6 IV|
|spectral_class|K9 IV|
|spectral_class|G2 IV|
|spectral_class|F9 IV|
|spectral_class|F0 IV|
|spectral_class|K8 IV|
|spectral_class|G8 IV|
|spectral_class|F6 IV|
|spectral_class|F5 IV|
|spectral_class|A0|
|spectral_class|A0IV|
|spectral_class|A0IV2|

<h2 id="tocS_UniverseStationsStationIdGet">UniverseStationsStationIdGet</h2>
<!-- backwards compatibility -->
<a id="schemauniversestationsstationidget"></a>
<a id="schema_UniverseStationsStationIdGet"></a>
<a id="tocSuniversestationsstationidget"></a>
<a id="tocsuniversestationsstationidget"></a>

```json
{
  "max_dockable_ship_volume": 0.1,
  "name": "string",
  "office_rental_cost": 0.1,
  "owner": 0,
  "position": {
    "x": 0.1,
    "y": 0.1,
    "z": 0.1
  },
  "race_id": 0,
  "reprocessing_efficiency": 0.1,
  "reprocessing_stations_take": 0.1,
  "services": [
    "bounty-missions"
  ],
  "station_id": 0,
  "system_id": 0,
  "type_id": 0
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|max_dockable_ship_volume|number(double)|true|none|none|
|name|string|true|none|none|
|office_rental_cost|number(double)|true|none|none|
|owner|integer(int64)|false|none|ID of the corporation that controls this station|
|position|object|true|none|none|
|» x|number(double)|true|none|none|
|» y|number(double)|true|none|none|
|» z|number(double)|true|none|none|
|race_id|integer(int64)|false|none|none|
|reprocessing_efficiency|number(double)|true|none|none|
|reprocessing_stations_take|number(double)|true|none|none|
|services|[string]|true|none|none|
|station_id|integer(int64)|true|none|none|
|system_id|integer(int64)|true|none|The solar system this station is in|
|type_id|integer(int64)|true|none|none|

<h2 id="tocS_UniverseStructuresGet">UniverseStructuresGet</h2>
<!-- backwards compatibility -->
<a id="schemauniversestructuresget"></a>
<a id="schema_UniverseStructuresGet"></a>
<a id="tocSuniversestructuresget"></a>
<a id="tocsuniversestructuresget"></a>

```json
[
  0
]

```

### Properties

*None*

<h2 id="tocS_UniverseStructuresStructureIdGet">UniverseStructuresStructureIdGet</h2>
<!-- backwards compatibility -->
<a id="schemauniversestructuresstructureidget"></a>
<a id="schema_UniverseStructuresStructureIdGet"></a>
<a id="tocSuniversestructuresstructureidget"></a>
<a id="tocsuniversestructuresstructureidget"></a>

```json
{
  "name": "string",
  "owner_id": 0,
  "position": {
    "x": 0.1,
    "y": 0.1,
    "z": 0.1
  },
  "solar_system_id": 0,
  "type_id": 0
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|name|string|true|none|The full name of the structure|
|owner_id|integer(int64)|true|none|The ID of the corporation who owns this particular structure|
|position|object|false|none|Coordinates of the structure in Cartesian space relative to the Sun, in metres.|
|» x|number(double)|true|none|none|
|» y|number(double)|true|none|none|
|» z|number(double)|true|none|none|
|solar_system_id|integer(int64)|true|none|none|
|type_id|integer(int64)|false|none|none|

<h2 id="tocS_UniverseSystemJumpsGet">UniverseSystemJumpsGet</h2>
<!-- backwards compatibility -->
<a id="schemauniversesystemjumpsget"></a>
<a id="schema_UniverseSystemJumpsGet"></a>
<a id="tocSuniversesystemjumpsget"></a>
<a id="tocsuniversesystemjumpsget"></a>

```json
[
  {
    "ship_jumps": 0,
    "system_id": 0
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|ship_jumps|integer(int64)|true|none|none|
|system_id|integer(int64)|true|none|none|

<h2 id="tocS_UniverseSystemKillsGet">UniverseSystemKillsGet</h2>
<!-- backwards compatibility -->
<a id="schemauniversesystemkillsget"></a>
<a id="schema_UniverseSystemKillsGet"></a>
<a id="tocSuniversesystemkillsget"></a>
<a id="tocsuniversesystemkillsget"></a>

```json
[
  {
    "npc_kills": 0,
    "pod_kills": 0,
    "ship_kills": 0,
    "system_id": 0
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|npc_kills|integer(int64)|true|none|Number of NPC ships killed in this system|
|pod_kills|integer(int64)|true|none|Number of pods killed in this system|
|ship_kills|integer(int64)|true|none|Number of player ships killed in this system|
|system_id|integer(int64)|true|none|none|

<h2 id="tocS_UniverseSystemsGet">UniverseSystemsGet</h2>
<!-- backwards compatibility -->
<a id="schemauniversesystemsget"></a>
<a id="schema_UniverseSystemsGet"></a>
<a id="tocSuniversesystemsget"></a>
<a id="tocsuniversesystemsget"></a>

```json
[
  0
]

```

### Properties

*None*

<h2 id="tocS_UniverseSystemsSystemIdGet">UniverseSystemsSystemIdGet</h2>
<!-- backwards compatibility -->
<a id="schemauniversesystemssystemidget"></a>
<a id="schema_UniverseSystemsSystemIdGet"></a>
<a id="tocSuniversesystemssystemidget"></a>
<a id="tocsuniversesystemssystemidget"></a>

```json
{
  "constellation_id": 0,
  "name": "string",
  "planets": [
    {
      "asteroid_belts": [
        0
      ],
      "moons": [
        0
      ],
      "planet_id": 0
    }
  ],
  "position": {
    "x": 0.1,
    "y": 0.1,
    "z": 0.1
  },
  "security_class": "string",
  "security_status": 0.1,
  "star_id": 0,
  "stargates": [
    0
  ],
  "stations": [
    0
  ],
  "system_id": 0
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|constellation_id|integer(int64)|true|none|The constellation this solar system is in|
|name|string|true|none|none|
|planets|[object]|false|none|none|
|» asteroid_belts|[integer]|false|none|none|
|» moons|[integer]|false|none|none|
|» planet_id|integer(int64)|true|none|none|
|position|object|true|none|none|
|» x|number(double)|true|none|none|
|» y|number(double)|true|none|none|
|» z|number(double)|true|none|none|
|security_class|string|false|none|none|
|security_status|number(double)|true|none|none|
|star_id|integer(int64)|false|none|none|
|stargates|[integer]|false|none|none|
|stations|[integer]|false|none|none|
|system_id|integer(int64)|true|none|none|

<h2 id="tocS_UniverseTypesGet">UniverseTypesGet</h2>
<!-- backwards compatibility -->
<a id="schemauniversetypesget"></a>
<a id="schema_UniverseTypesGet"></a>
<a id="tocSuniversetypesget"></a>
<a id="tocsuniversetypesget"></a>

```json
[
  0
]

```

### Properties

*None*

<h2 id="tocS_UniverseTypesTypeIdGet">UniverseTypesTypeIdGet</h2>
<!-- backwards compatibility -->
<a id="schemauniversetypestypeidget"></a>
<a id="schema_UniverseTypesTypeIdGet"></a>
<a id="tocSuniversetypestypeidget"></a>
<a id="tocsuniversetypestypeidget"></a>

```json
{
  "capacity": 0.1,
  "description": "string",
  "dogma_attributes": [
    {
      "attribute_id": 0,
      "value": 0.1
    }
  ],
  "dogma_effects": [
    {
      "effect_id": 0,
      "is_default": true
    }
  ],
  "graphic_id": 0,
  "group_id": 0,
  "icon_id": 0,
  "market_group_id": 0,
  "mass": 0.1,
  "name": "string",
  "packaged_volume": 0.1,
  "portion_size": 0,
  "published": true,
  "radius": 0.1,
  "type_id": 0,
  "volume": 0.1
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|capacity|number(double)|false|none|none|
|description|string|true|none|none|
|dogma_attributes|[object]|false|none|none|
|» attribute_id|integer(int64)|true|none|none|
|» value|number(double)|true|none|none|
|dogma_effects|[object]|false|none|none|
|» effect_id|integer(int64)|true|none|none|
|» is_default|boolean|true|none|none|
|graphic_id|integer(int64)|false|none|none|
|group_id|integer(int64)|true|none|none|
|icon_id|integer(int64)|false|none|none|
|market_group_id|integer(int64)|false|none|This only exists for types that can be put on the market|
|mass|number(double)|false|none|none|
|name|string|true|none|none|
|packaged_volume|number(double)|false|none|none|
|portion_size|integer(int64)|false|none|none|
|published|boolean|true|none|none|
|radius|number(double)|false|none|none|
|type_id|integer(int64)|true|none|none|
|volume|number(double)|false|none|none|

<h2 id="tocS_WarsGet">WarsGet</h2>
<!-- backwards compatibility -->
<a id="schemawarsget"></a>
<a id="schema_WarsGet"></a>
<a id="tocSwarsget"></a>
<a id="tocswarsget"></a>

```json
[
  0
]

```

### Properties

*None*

<h2 id="tocS_WarsWarIdGet">WarsWarIdGet</h2>
<!-- backwards compatibility -->
<a id="schemawarswaridget"></a>
<a id="schema_WarsWarIdGet"></a>
<a id="tocSwarswaridget"></a>
<a id="tocswarswaridget"></a>

```json
{
  "aggressor": {
    "alliance_id": 0,
    "corporation_id": 0,
    "isk_destroyed": 0.1,
    "ships_killed": 0
  },
  "allies": [
    {
      "alliance_id": 0,
      "corporation_id": 0
    }
  ],
  "declared": "2019-08-24T14:15:22Z",
  "defender": {
    "alliance_id": 0,
    "corporation_id": 0,
    "isk_destroyed": 0.1,
    "ships_killed": 0
  },
  "finished": "2019-08-24T14:15:22Z",
  "id": 0,
  "mutual": true,
  "open_for_allies": true,
  "retracted": "2019-08-24T14:15:22Z",
  "started": "2019-08-24T14:15:22Z"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|aggressor|object|true|none|The aggressor corporation or alliance that declared this war, only contains either corporation_id or alliance_id|
|» alliance_id|integer(int64)|false|none|Alliance ID if and only if the aggressor is an alliance|
|» corporation_id|integer(int64)|false|none|Corporation ID if and only if the aggressor is a corporation|
|» isk_destroyed|number(double)|true|none|ISK value of ships the aggressor has destroyed|
|» ships_killed|integer(int64)|true|none|The number of ships the aggressor has killed|
|allies|[object]|false|none|allied corporations or alliances, each object contains either corporation_id or alliance_id|
|» alliance_id|integer(int64)|false|none|Alliance ID if and only if this ally is an alliance|
|» corporation_id|integer(int64)|false|none|Corporation ID if and only if this ally is a corporation|
|declared|string(date-time)|true|none|Time that the war was declared|
|defender|object|true|none|The defending corporation or alliance that declared this war, only contains either corporation_id or alliance_id|
|» alliance_id|integer(int64)|false|none|Alliance ID if and only if the defender is an alliance|
|» corporation_id|integer(int64)|false|none|Corporation ID if and only if the defender is a corporation|
|» isk_destroyed|number(double)|true|none|ISK value of ships the defender has killed|
|» ships_killed|integer(int64)|true|none|The number of ships the defender has killed|
|finished|string(date-time)|false|none|Time the war ended and shooting was no longer allowed|
|id|integer(int64)|true|none|ID of the specified war|
|mutual|boolean|true|none|Was the war declared mutual by both parties|
|open_for_allies|boolean|true|none|Is the war currently open for allies or not|
|retracted|string(date-time)|false|none|Time the war was retracted but both sides could still shoot each other|
|started|string(date-time)|false|none|Time when the war started and both sides could shoot each other|

<h2 id="tocS_WarsWarIdKillmailsGet">WarsWarIdKillmailsGet</h2>
<!-- backwards compatibility -->
<a id="schemawarswaridkillmailsget"></a>
<a id="schema_WarsWarIdKillmailsGet"></a>
<a id="tocSwarswaridkillmailsget"></a>
<a id="tocswarswaridkillmailsget"></a>

```json
[
  {
    "killmail_hash": "string",
    "killmail_id": 0
  }
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|killmail_hash|string|true|none|A hash of this killmail|
|killmail_id|integer(int64)|true|none|ID of this killmail|

