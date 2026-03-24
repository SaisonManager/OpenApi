# @saisonmanager/saisonmanager-api-v2

Official Client for the SaisonManager API.

# SaisonManagerApi

All URIs are relative to *https://saisonmanager.de*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**apiV2AdminLeaguesLeagueIdAdditionalReferencesJsonGet**](#apiv2adminleaguesleagueidadditionalreferencesjsonget) | **GET** /api/v2/admin/leagues/{leagueId}/additional_references.json |  |
| [**apiV2GameOperationsGameOperationIdLeaguesJsonGet**](#apiv2gameoperationsgameoperationidleaguesjsonget) | **GET** /api/v2/game_operations/{gameOperationId}/leagues.json |  |
| [**apiV2GamesGameIdJsonGet**](#apiv2gamesgameidjsonget) | **GET** /api/v2/games/{gameId}.json |  |
| [**apiV2GamesJsonGet**](#apiv2gamesjsonget) | **GET** /api/v2/games.json |  |
| [**apiV2InitJsonGet**](#apiv2initjsonget) | **GET** /api/v2/init.json |  |
| [**apiV2LeaguesJsonGet**](#apiv2leaguesjsonget) | **GET** /api/v2/leagues.json |  |
| [**apiV2LeaguesLeagueIdGameDaysCurrentScheduleJsonGet**](#apiv2leaguesleagueidgamedayscurrentschedulejsonget) | **GET** /api/v2/leagues/{leagueId}/game_days/current/schedule.json |  |
| [**apiV2LeaguesLeagueIdGameDaysGameDayNumberScheduleJsonGet**](#apiv2leaguesleagueidgamedaysgamedaynumberschedulejsonget) | **GET** /api/v2/leagues/{leagueId}/game_days/{gameDayNumber}/schedule.json |  |
| [**apiV2LeaguesLeagueIdGroupedTableJsonGet**](#apiv2leaguesleagueidgroupedtablejsonget) | **GET** /api/v2/leagues/{leagueId}/grouped_table.json |  |
| [**apiV2LeaguesLeagueIdJsonGet**](#apiv2leaguesleagueidjsonget) | **GET** /api/v2/leagues/{leagueId}.json |  |
| [**apiV2LeaguesLeagueIdScheduleJsonGet**](#apiv2leaguesleagueidschedulejsonget) | **GET** /api/v2/leagues/{leagueId}/schedule.json |  |
| [**apiV2LeaguesLeagueIdScorerJsonGet**](#apiv2leaguesleagueidscorerjsonget) | **GET** /api/v2/leagues/{leagueId}/scorer.json |  |
| [**apiV2LeaguesLeagueIdTableJsonGet**](#apiv2leaguesleagueidtablejsonget) | **GET** /api/v2/leagues/{leagueId}/table.json |  |
| [**apiV2PenaltiesJsonGet**](#apiv2penaltiesjsonget) | **GET** /api/v2/penalties.json |  |
| [**apiV2PenaltyCodesJsonGet**](#apiv2penaltycodesjsonget) | **GET** /api/v2/penalty_codes.json |  |



## apiV2AdminLeaguesLeagueIdAdditionalReferencesJsonGet

> SmLeagueAdditionalReferencesResponse apiV2AdminLeaguesLeagueIdAdditionalReferencesJsonGet(leagueId)



### Example

```ts
import {
  Configuration,
  SaisonManagerApi,
} from '@saisonmanager/saisonmanager-api-v2';
import type { ApiV2AdminLeaguesLeagueIdAdditionalReferencesJsonGetRequest } from '@saisonmanager/saisonmanager-api-v2';

async function example() {
  console.log("🚀 Testing @saisonmanager/saisonmanager-api-v2 SDK...");
  const api = new SaisonManagerApi();

  const body = {
    // number
    leagueId: 56,
  } satisfies ApiV2AdminLeaguesLeagueIdAdditionalReferencesJsonGetRequest;

  try {
    const data = await api.apiV2AdminLeaguesLeagueIdAdditionalReferencesJsonGet(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **leagueId** | `number` |  | [Defaults to `undefined`] |

### Return type

[**SmLeagueAdditionalReferencesResponse**](#smleagueadditionalreferencesresponse)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## apiV2GameOperationsGameOperationIdLeaguesJsonGet

> Array&lt;SmV2BaseLeague&gt; apiV2GameOperationsGameOperationIdLeaguesJsonGet(gameOperationId)



### Example

```ts
import {
  Configuration,
  SaisonManagerApi,
} from '@saisonmanager/saisonmanager-api-v2';
import type { ApiV2GameOperationsGameOperationIdLeaguesJsonGetRequest } from '@saisonmanager/saisonmanager-api-v2';

async function example() {
  console.log("🚀 Testing @saisonmanager/saisonmanager-api-v2 SDK...");
  const api = new SaisonManagerApi();

  const body = {
    // number
    gameOperationId: 56,
  } satisfies ApiV2GameOperationsGameOperationIdLeaguesJsonGetRequest;

  try {
    const data = await api.apiV2GameOperationsGameOperationIdLeaguesJsonGet(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **gameOperationId** | `number` |  | [Defaults to `undefined`] |

### Return type

[**Array&lt;SmV2BaseLeague&gt;**](#smv2baseleague)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## apiV2GamesGameIdJsonGet

> SmGameResponse apiV2GamesGameIdJsonGet(gameId)



### Example

```ts
import {
  Configuration,
  SaisonManagerApi,
} from '@saisonmanager/saisonmanager-api-v2';
import type { ApiV2GamesGameIdJsonGetRequest } from '@saisonmanager/saisonmanager-api-v2';

async function example() {
  console.log("🚀 Testing @saisonmanager/saisonmanager-api-v2 SDK...");
  const api = new SaisonManagerApi();

  const body = {
    // number
    gameId: 56,
  } satisfies ApiV2GamesGameIdJsonGetRequest;

  try {
    const data = await api.apiV2GamesGameIdJsonGet(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **gameId** | `number` |  | [Defaults to `undefined`] |

### Return type

[**SmGameResponse**](#smgameresponse)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## apiV2GamesJsonGet

> Array&lt;SmV2GamePreview&gt; apiV2GamesJsonGet()



### Example

```ts
import {
  Configuration,
  SaisonManagerApi,
} from '@saisonmanager/saisonmanager-api-v2';
import type { ApiV2GamesJsonGetRequest } from '@saisonmanager/saisonmanager-api-v2';

async function example() {
  console.log("🚀 Testing @saisonmanager/saisonmanager-api-v2 SDK...");
  const api = new SaisonManagerApi();

  try {
    const data = await api.apiV2GamesJsonGet();
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**Array&lt;SmV2GamePreview&gt;**](#smv2gamepreview)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## apiV2InitJsonGet

> SmInitResponse apiV2InitJsonGet()



### Example

```ts
import {
  Configuration,
  SaisonManagerApi,
} from '@saisonmanager/saisonmanager-api-v2';
import type { ApiV2InitJsonGetRequest } from '@saisonmanager/saisonmanager-api-v2';

async function example() {
  console.log("🚀 Testing @saisonmanager/saisonmanager-api-v2 SDK...");
  const api = new SaisonManagerApi();

  try {
    const data = await api.apiV2InitJsonGet();
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**SmInitResponse**](#sminitresponse)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## apiV2LeaguesJsonGet

> Array&lt;SmV2LeaguePreview&gt; apiV2LeaguesJsonGet()



### Example

```ts
import {
  Configuration,
  SaisonManagerApi,
} from '@saisonmanager/saisonmanager-api-v2';
import type { ApiV2LeaguesJsonGetRequest } from '@saisonmanager/saisonmanager-api-v2';

async function example() {
  console.log("🚀 Testing @saisonmanager/saisonmanager-api-v2 SDK...");
  const api = new SaisonManagerApi();

  try {
    const data = await api.apiV2LeaguesJsonGet();
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**Array&lt;SmV2LeaguePreview&gt;**](#smv2leaguepreview)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## apiV2LeaguesLeagueIdGameDaysCurrentScheduleJsonGet

> Array&lt;SmV2ScheduledGame&gt; apiV2LeaguesLeagueIdGameDaysCurrentScheduleJsonGet(leagueId)



### Example

```ts
import {
  Configuration,
  SaisonManagerApi,
} from '@saisonmanager/saisonmanager-api-v2';
import type { ApiV2LeaguesLeagueIdGameDaysCurrentScheduleJsonGetRequest } from '@saisonmanager/saisonmanager-api-v2';

async function example() {
  console.log("🚀 Testing @saisonmanager/saisonmanager-api-v2 SDK...");
  const api = new SaisonManagerApi();

  const body = {
    // number
    leagueId: 56,
  } satisfies ApiV2LeaguesLeagueIdGameDaysCurrentScheduleJsonGetRequest;

  try {
    const data = await api.apiV2LeaguesLeagueIdGameDaysCurrentScheduleJsonGet(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **leagueId** | `number` |  | [Defaults to `undefined`] |

### Return type

[**Array&lt;SmV2ScheduledGame&gt;**](#smv2scheduledgame)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## apiV2LeaguesLeagueIdGameDaysGameDayNumberScheduleJsonGet

> Array&lt;SmV2ScheduledGame&gt; apiV2LeaguesLeagueIdGameDaysGameDayNumberScheduleJsonGet(leagueId, gameDayNumber)



### Example

```ts
import {
  Configuration,
  SaisonManagerApi,
} from '@saisonmanager/saisonmanager-api-v2';
import type { ApiV2LeaguesLeagueIdGameDaysGameDayNumberScheduleJsonGetRequest } from '@saisonmanager/saisonmanager-api-v2';

async function example() {
  console.log("🚀 Testing @saisonmanager/saisonmanager-api-v2 SDK...");
  const api = new SaisonManagerApi();

  const body = {
    // number
    leagueId: 56,
    // ApiV2LeaguesLeagueIdGameDaysGameDayNumberScheduleJsonGetGameDayNumberParameter
    gameDayNumber: 56,
  } satisfies ApiV2LeaguesLeagueIdGameDaysGameDayNumberScheduleJsonGetRequest;

  try {
    const data = await api.apiV2LeaguesLeagueIdGameDaysGameDayNumberScheduleJsonGet(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **leagueId** | `number` |  | [Defaults to `undefined`] |
| **gameDayNumber** | [](.md) |  | [Defaults to `undefined`] |

### Return type

[**Array&lt;SmV2ScheduledGame&gt;**](#smv2scheduledgame)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## apiV2LeaguesLeagueIdGroupedTableJsonGet

> { [key: string]: SmV2TableGroup; } apiV2LeaguesLeagueIdGroupedTableJsonGet(leagueId)



### Example

```ts
import {
  Configuration,
  SaisonManagerApi,
} from '@saisonmanager/saisonmanager-api-v2';
import type { ApiV2LeaguesLeagueIdGroupedTableJsonGetRequest } from '@saisonmanager/saisonmanager-api-v2';

async function example() {
  console.log("🚀 Testing @saisonmanager/saisonmanager-api-v2 SDK...");
  const api = new SaisonManagerApi();

  const body = {
    // number
    leagueId: 56,
  } satisfies ApiV2LeaguesLeagueIdGroupedTableJsonGetRequest;

  try {
    const data = await api.apiV2LeaguesLeagueIdGroupedTableJsonGet(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **leagueId** | `number` |  | [Defaults to `undefined`] |

### Return type

[**{ [key: string]: SmV2TableGroup; }**](SmV2TableGroup.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## apiV2LeaguesLeagueIdJsonGet

> SmLeagueResponse apiV2LeaguesLeagueIdJsonGet(leagueId)



### Example

```ts
import {
  Configuration,
  SaisonManagerApi,
} from '@saisonmanager/saisonmanager-api-v2';
import type { ApiV2LeaguesLeagueIdJsonGetRequest } from '@saisonmanager/saisonmanager-api-v2';

async function example() {
  console.log("🚀 Testing @saisonmanager/saisonmanager-api-v2 SDK...");
  const api = new SaisonManagerApi();

  const body = {
    // number
    leagueId: 56,
  } satisfies ApiV2LeaguesLeagueIdJsonGetRequest;

  try {
    const data = await api.apiV2LeaguesLeagueIdJsonGet(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **leagueId** | `number` |  | [Defaults to `undefined`] |

### Return type

[**SmLeagueResponse**](#smleagueresponse)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## apiV2LeaguesLeagueIdScheduleJsonGet

> Array&lt;SmV2ScheduledGame&gt; apiV2LeaguesLeagueIdScheduleJsonGet(leagueId)



### Example

```ts
import {
  Configuration,
  SaisonManagerApi,
} from '@saisonmanager/saisonmanager-api-v2';
import type { ApiV2LeaguesLeagueIdScheduleJsonGetRequest } from '@saisonmanager/saisonmanager-api-v2';

async function example() {
  console.log("🚀 Testing @saisonmanager/saisonmanager-api-v2 SDK...");
  const api = new SaisonManagerApi();

  const body = {
    // number
    leagueId: 56,
  } satisfies ApiV2LeaguesLeagueIdScheduleJsonGetRequest;

  try {
    const data = await api.apiV2LeaguesLeagueIdScheduleJsonGet(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **leagueId** | `number` |  | [Defaults to `undefined`] |

### Return type

[**Array&lt;SmV2ScheduledGame&gt;**](#smv2scheduledgame)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## apiV2LeaguesLeagueIdScorerJsonGet

> Array&lt;SmV2ScorerPlayer&gt; apiV2LeaguesLeagueIdScorerJsonGet(leagueId)



### Example

```ts
import {
  Configuration,
  SaisonManagerApi,
} from '@saisonmanager/saisonmanager-api-v2';
import type { ApiV2LeaguesLeagueIdScorerJsonGetRequest } from '@saisonmanager/saisonmanager-api-v2';

async function example() {
  console.log("🚀 Testing @saisonmanager/saisonmanager-api-v2 SDK...");
  const api = new SaisonManagerApi();

  const body = {
    // number
    leagueId: 56,
  } satisfies ApiV2LeaguesLeagueIdScorerJsonGetRequest;

  try {
    const data = await api.apiV2LeaguesLeagueIdScorerJsonGet(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **leagueId** | `number` |  | [Defaults to `undefined`] |

### Return type

[**Array&lt;SmV2ScorerPlayer&gt;**](#smv2scorerplayer)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## apiV2LeaguesLeagueIdTableJsonGet

> Array&lt;SmV2TableTeam&gt; apiV2LeaguesLeagueIdTableJsonGet(leagueId)



### Example

```ts
import {
  Configuration,
  SaisonManagerApi,
} from '@saisonmanager/saisonmanager-api-v2';
import type { ApiV2LeaguesLeagueIdTableJsonGetRequest } from '@saisonmanager/saisonmanager-api-v2';

async function example() {
  console.log("🚀 Testing @saisonmanager/saisonmanager-api-v2 SDK...");
  const api = new SaisonManagerApi();

  const body = {
    // number
    leagueId: 56,
  } satisfies ApiV2LeaguesLeagueIdTableJsonGetRequest;

  try {
    const data = await api.apiV2LeaguesLeagueIdTableJsonGet(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **leagueId** | `number` |  | [Defaults to `undefined`] |

### Return type

[**Array&lt;SmV2TableTeam&gt;**](#smv2tableteam)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## apiV2PenaltiesJsonGet

> Array&lt;SmV2Penalty&gt; apiV2PenaltiesJsonGet()



### Example

```ts
import {
  Configuration,
  SaisonManagerApi,
} from '@saisonmanager/saisonmanager-api-v2';
import type { ApiV2PenaltiesJsonGetRequest } from '@saisonmanager/saisonmanager-api-v2';

async function example() {
  console.log("🚀 Testing @saisonmanager/saisonmanager-api-v2 SDK...");
  const api = new SaisonManagerApi();

  try {
    const data = await api.apiV2PenaltiesJsonGet();
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**Array&lt;SmV2Penalty&gt;**](#smv2penalty)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## apiV2PenaltyCodesJsonGet

> Array&lt;SmV2PenaltyCode&gt; apiV2PenaltyCodesJsonGet()



### Example

```ts
import {
  Configuration,
  SaisonManagerApi,
} from '@saisonmanager/saisonmanager-api-v2';
import type { ApiV2PenaltyCodesJsonGetRequest } from '@saisonmanager/saisonmanager-api-v2';

async function example() {
  console.log("🚀 Testing @saisonmanager/saisonmanager-api-v2 SDK...");
  const api = new SaisonManagerApi();

  try {
    const data = await api.apiV2PenaltyCodesJsonGet();
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**Array&lt;SmV2PenaltyCode&gt;**](#smv2penaltycode)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

