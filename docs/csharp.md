# SaisonManager.Api.V2

Official Client for the SaisonManager API.

# SaisonManager.Api.V2.Api.SaisonManagerApi

All URIs are relative to *https://saisonmanager.de*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**ApiV2AdminLeaguesLeagueIdAdditionalReferencesJsonGet**](#apiv2adminleaguesleagueidadditionalreferencesjsonget) | **GET** /api/v2/admin/leagues/{leagueId}/additional_references.json |  |
| [**ApiV2GameOperationsGameOperationIdLeaguesJsonGet**](#apiv2gameoperationsgameoperationidleaguesjsonget) | **GET** /api/v2/game_operations/{gameOperationId}/leagues.json |  |
| [**ApiV2GamesGameIdJsonGet**](#apiv2gamesgameidjsonget) | **GET** /api/v2/games/{gameId}.json |  |
| [**ApiV2GamesJsonGet**](#apiv2gamesjsonget) | **GET** /api/v2/games.json |  |
| [**ApiV2InitJsonGet**](#apiv2initjsonget) | **GET** /api/v2/init.json |  |
| [**ApiV2LeaguesJsonGet**](#apiv2leaguesjsonget) | **GET** /api/v2/leagues.json |  |
| [**ApiV2LeaguesLeagueIdGameDaysCurrentScheduleJsonGet**](#apiv2leaguesleagueidgamedayscurrentschedulejsonget) | **GET** /api/v2/leagues/{leagueId}/game_days/current/schedule.json |  |
| [**ApiV2LeaguesLeagueIdGameDaysGameDayNumberScheduleJsonGet**](#apiv2leaguesleagueidgamedaysgamedaynumberschedulejsonget) | **GET** /api/v2/leagues/{leagueId}/game_days/{gameDayNumber}/schedule.json |  |
| [**ApiV2LeaguesLeagueIdGroupedTableJsonGet**](#apiv2leaguesleagueidgroupedtablejsonget) | **GET** /api/v2/leagues/{leagueId}/grouped_table.json |  |
| [**ApiV2LeaguesLeagueIdJsonGet**](#apiv2leaguesleagueidjsonget) | **GET** /api/v2/leagues/{leagueId}.json |  |
| [**ApiV2LeaguesLeagueIdScheduleJsonGet**](#apiv2leaguesleagueidschedulejsonget) | **GET** /api/v2/leagues/{leagueId}/schedule.json |  |
| [**ApiV2LeaguesLeagueIdScorerJsonGet**](#apiv2leaguesleagueidscorerjsonget) | **GET** /api/v2/leagues/{leagueId}/scorer.json |  |
| [**ApiV2LeaguesLeagueIdTableJsonGet**](#apiv2leaguesleagueidtablejsonget) | **GET** /api/v2/leagues/{leagueId}/table.json |  |
| [**ApiV2PenaltiesJsonGet**](#apiv2penaltiesjsonget) | **GET** /api/v2/penalties.json |  |
| [**ApiV2PenaltyCodesJsonGet**](#apiv2penaltycodesjsonget) | **GET** /api/v2/penalty_codes.json |  |

<a id="apiv2adminleaguesleagueidadditionalreferencesjsonget"></a>
# **ApiV2AdminLeaguesLeagueIdAdditionalReferencesJsonGet**
> SmLeagueAdditionalReferencesResponse ApiV2AdminLeaguesLeagueIdAdditionalReferencesJsonGet (int leagueId)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using System.Net.Http;
using SaisonManager.Api.V2.Api;
using SaisonManager.Api.V2.Client;
using SaisonManager.Api.V2.Model;

namespace Example
{
    public class ApiV2AdminLeaguesLeagueIdAdditionalReferencesJsonGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://saisonmanager.de";
            // create instances of HttpClient, HttpClientHandler to be reused later with different Api classes
            HttpClient httpClient = new HttpClient();
            HttpClientHandler httpClientHandler = new HttpClientHandler();
            var apiInstance = new SaisonManagerApi(httpClient, config, httpClientHandler);
            var leagueId = 56;  // int | 

            try
            {
                SmLeagueAdditionalReferencesResponse result = apiInstance.ApiV2AdminLeaguesLeagueIdAdditionalReferencesJsonGet(leagueId);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SaisonManagerApi.ApiV2AdminLeaguesLeagueIdAdditionalReferencesJsonGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the ApiV2AdminLeaguesLeagueIdAdditionalReferencesJsonGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<SmLeagueAdditionalReferencesResponse> response = apiInstance.ApiV2AdminLeaguesLeagueIdAdditionalReferencesJsonGetWithHttpInfo(leagueId);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SaisonManagerApi.ApiV2AdminLeaguesLeagueIdAdditionalReferencesJsonGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **leagueId** | **int** |  |  |

### Return type

[**SmLeagueAdditionalReferencesResponse**](#smleagueadditionalreferencesresponse)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="apiv2gameoperationsgameoperationidleaguesjsonget"></a>
# **ApiV2GameOperationsGameOperationIdLeaguesJsonGet**
> List&lt;SmV2BaseLeague&gt; ApiV2GameOperationsGameOperationIdLeaguesJsonGet (int gameOperationId)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using System.Net.Http;
using SaisonManager.Api.V2.Api;
using SaisonManager.Api.V2.Client;
using SaisonManager.Api.V2.Model;

namespace Example
{
    public class ApiV2GameOperationsGameOperationIdLeaguesJsonGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://saisonmanager.de";
            // create instances of HttpClient, HttpClientHandler to be reused later with different Api classes
            HttpClient httpClient = new HttpClient();
            HttpClientHandler httpClientHandler = new HttpClientHandler();
            var apiInstance = new SaisonManagerApi(httpClient, config, httpClientHandler);
            var gameOperationId = 56;  // int | 

            try
            {
                List<SmV2BaseLeague> result = apiInstance.ApiV2GameOperationsGameOperationIdLeaguesJsonGet(gameOperationId);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SaisonManagerApi.ApiV2GameOperationsGameOperationIdLeaguesJsonGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the ApiV2GameOperationsGameOperationIdLeaguesJsonGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<List<SmV2BaseLeague>> response = apiInstance.ApiV2GameOperationsGameOperationIdLeaguesJsonGetWithHttpInfo(gameOperationId);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SaisonManagerApi.ApiV2GameOperationsGameOperationIdLeaguesJsonGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameOperationId** | **int** |  |  |

### Return type

[**List&lt;SmV2BaseLeague&gt;**](#smv2baseleague)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="apiv2gamesgameidjsonget"></a>
# **ApiV2GamesGameIdJsonGet**
> SmGameResponse ApiV2GamesGameIdJsonGet (int gameId)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using System.Net.Http;
using SaisonManager.Api.V2.Api;
using SaisonManager.Api.V2.Client;
using SaisonManager.Api.V2.Model;

namespace Example
{
    public class ApiV2GamesGameIdJsonGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://saisonmanager.de";
            // create instances of HttpClient, HttpClientHandler to be reused later with different Api classes
            HttpClient httpClient = new HttpClient();
            HttpClientHandler httpClientHandler = new HttpClientHandler();
            var apiInstance = new SaisonManagerApi(httpClient, config, httpClientHandler);
            var gameId = 56;  // int | 

            try
            {
                SmGameResponse result = apiInstance.ApiV2GamesGameIdJsonGet(gameId);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SaisonManagerApi.ApiV2GamesGameIdJsonGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the ApiV2GamesGameIdJsonGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<SmGameResponse> response = apiInstance.ApiV2GamesGameIdJsonGetWithHttpInfo(gameId);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SaisonManagerApi.ApiV2GamesGameIdJsonGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **gameId** | **int** |  |  |

### Return type

[**SmGameResponse**](#smgameresponse)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="apiv2gamesjsonget"></a>
# **ApiV2GamesJsonGet**
> List&lt;SmV2GamePreview&gt; ApiV2GamesJsonGet ()



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using System.Net.Http;
using SaisonManager.Api.V2.Api;
using SaisonManager.Api.V2.Client;
using SaisonManager.Api.V2.Model;

namespace Example
{
    public class ApiV2GamesJsonGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://saisonmanager.de";
            // create instances of HttpClient, HttpClientHandler to be reused later with different Api classes
            HttpClient httpClient = new HttpClient();
            HttpClientHandler httpClientHandler = new HttpClientHandler();
            var apiInstance = new SaisonManagerApi(httpClient, config, httpClientHandler);

            try
            {
                List<SmV2GamePreview> result = apiInstance.ApiV2GamesJsonGet();
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SaisonManagerApi.ApiV2GamesJsonGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the ApiV2GamesJsonGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<List<SmV2GamePreview>> response = apiInstance.ApiV2GamesJsonGetWithHttpInfo();
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SaisonManagerApi.ApiV2GamesJsonGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters
This endpoint does not need any parameter.
### Return type

[**List&lt;SmV2GamePreview&gt;**](#smv2gamepreview)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="apiv2initjsonget"></a>
# **ApiV2InitJsonGet**
> SmInitResponse ApiV2InitJsonGet ()



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using System.Net.Http;
using SaisonManager.Api.V2.Api;
using SaisonManager.Api.V2.Client;
using SaisonManager.Api.V2.Model;

namespace Example
{
    public class ApiV2InitJsonGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://saisonmanager.de";
            // create instances of HttpClient, HttpClientHandler to be reused later with different Api classes
            HttpClient httpClient = new HttpClient();
            HttpClientHandler httpClientHandler = new HttpClientHandler();
            var apiInstance = new SaisonManagerApi(httpClient, config, httpClientHandler);

            try
            {
                SmInitResponse result = apiInstance.ApiV2InitJsonGet();
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SaisonManagerApi.ApiV2InitJsonGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the ApiV2InitJsonGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<SmInitResponse> response = apiInstance.ApiV2InitJsonGetWithHttpInfo();
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SaisonManagerApi.ApiV2InitJsonGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters
This endpoint does not need any parameter.
### Return type

[**SmInitResponse**](#sminitresponse)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="apiv2leaguesjsonget"></a>
# **ApiV2LeaguesJsonGet**
> List&lt;SmV2LeaguePreview&gt; ApiV2LeaguesJsonGet ()



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using System.Net.Http;
using SaisonManager.Api.V2.Api;
using SaisonManager.Api.V2.Client;
using SaisonManager.Api.V2.Model;

namespace Example
{
    public class ApiV2LeaguesJsonGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://saisonmanager.de";
            // create instances of HttpClient, HttpClientHandler to be reused later with different Api classes
            HttpClient httpClient = new HttpClient();
            HttpClientHandler httpClientHandler = new HttpClientHandler();
            var apiInstance = new SaisonManagerApi(httpClient, config, httpClientHandler);

            try
            {
                List<SmV2LeaguePreview> result = apiInstance.ApiV2LeaguesJsonGet();
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SaisonManagerApi.ApiV2LeaguesJsonGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the ApiV2LeaguesJsonGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<List<SmV2LeaguePreview>> response = apiInstance.ApiV2LeaguesJsonGetWithHttpInfo();
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SaisonManagerApi.ApiV2LeaguesJsonGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters
This endpoint does not need any parameter.
### Return type

[**List&lt;SmV2LeaguePreview&gt;**](#smv2leaguepreview)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="apiv2leaguesleagueidgamedayscurrentschedulejsonget"></a>
# **ApiV2LeaguesLeagueIdGameDaysCurrentScheduleJsonGet**
> List&lt;SmV2ScheduledGame&gt; ApiV2LeaguesLeagueIdGameDaysCurrentScheduleJsonGet (int leagueId)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using System.Net.Http;
using SaisonManager.Api.V2.Api;
using SaisonManager.Api.V2.Client;
using SaisonManager.Api.V2.Model;

namespace Example
{
    public class ApiV2LeaguesLeagueIdGameDaysCurrentScheduleJsonGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://saisonmanager.de";
            // create instances of HttpClient, HttpClientHandler to be reused later with different Api classes
            HttpClient httpClient = new HttpClient();
            HttpClientHandler httpClientHandler = new HttpClientHandler();
            var apiInstance = new SaisonManagerApi(httpClient, config, httpClientHandler);
            var leagueId = 56;  // int | 

            try
            {
                List<SmV2ScheduledGame> result = apiInstance.ApiV2LeaguesLeagueIdGameDaysCurrentScheduleJsonGet(leagueId);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SaisonManagerApi.ApiV2LeaguesLeagueIdGameDaysCurrentScheduleJsonGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the ApiV2LeaguesLeagueIdGameDaysCurrentScheduleJsonGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<List<SmV2ScheduledGame>> response = apiInstance.ApiV2LeaguesLeagueIdGameDaysCurrentScheduleJsonGetWithHttpInfo(leagueId);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SaisonManagerApi.ApiV2LeaguesLeagueIdGameDaysCurrentScheduleJsonGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **leagueId** | **int** |  |  |

### Return type

[**List&lt;SmV2ScheduledGame&gt;**](#smv2scheduledgame)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="apiv2leaguesleagueidgamedaysgamedaynumberschedulejsonget"></a>
# **ApiV2LeaguesLeagueIdGameDaysGameDayNumberScheduleJsonGet**
> List&lt;SmV2ScheduledGame&gt; ApiV2LeaguesLeagueIdGameDaysGameDayNumberScheduleJsonGet (int leagueId, ApiV2LeaguesLeagueIdGameDaysGameDayNumberScheduleJsonGetGameDayNumberParameter gameDayNumber)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using System.Net.Http;
using SaisonManager.Api.V2.Api;
using SaisonManager.Api.V2.Client;
using SaisonManager.Api.V2.Model;

namespace Example
{
    public class ApiV2LeaguesLeagueIdGameDaysGameDayNumberScheduleJsonGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://saisonmanager.de";
            // create instances of HttpClient, HttpClientHandler to be reused later with different Api classes
            HttpClient httpClient = new HttpClient();
            HttpClientHandler httpClientHandler = new HttpClientHandler();
            var apiInstance = new SaisonManagerApi(httpClient, config, httpClientHandler);
            var leagueId = 56;  // int | 
            var gameDayNumber = new ApiV2LeaguesLeagueIdGameDaysGameDayNumberScheduleJsonGetGameDayNumberParameter();  // ApiV2LeaguesLeagueIdGameDaysGameDayNumberScheduleJsonGetGameDayNumberParameter | 

            try
            {
                List<SmV2ScheduledGame> result = apiInstance.ApiV2LeaguesLeagueIdGameDaysGameDayNumberScheduleJsonGet(leagueId, gameDayNumber);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SaisonManagerApi.ApiV2LeaguesLeagueIdGameDaysGameDayNumberScheduleJsonGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the ApiV2LeaguesLeagueIdGameDaysGameDayNumberScheduleJsonGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<List<SmV2ScheduledGame>> response = apiInstance.ApiV2LeaguesLeagueIdGameDaysGameDayNumberScheduleJsonGetWithHttpInfo(leagueId, gameDayNumber);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SaisonManagerApi.ApiV2LeaguesLeagueIdGameDaysGameDayNumberScheduleJsonGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **leagueId** | **int** |  |  |
| **gameDayNumber** | **ApiV2LeaguesLeagueIdGameDaysGameDayNumberScheduleJsonGetGameDayNumberParameter** |  |  |

### Return type

[**List&lt;SmV2ScheduledGame&gt;**](#smv2scheduledgame)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="apiv2leaguesleagueidgroupedtablejsonget"></a>
# **ApiV2LeaguesLeagueIdGroupedTableJsonGet**
> Dictionary&lt;string, SmV2TableGroup&gt; ApiV2LeaguesLeagueIdGroupedTableJsonGet (int leagueId)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using System.Net.Http;
using SaisonManager.Api.V2.Api;
using SaisonManager.Api.V2.Client;
using SaisonManager.Api.V2.Model;

namespace Example
{
    public class ApiV2LeaguesLeagueIdGroupedTableJsonGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://saisonmanager.de";
            // create instances of HttpClient, HttpClientHandler to be reused later with different Api classes
            HttpClient httpClient = new HttpClient();
            HttpClientHandler httpClientHandler = new HttpClientHandler();
            var apiInstance = new SaisonManagerApi(httpClient, config, httpClientHandler);
            var leagueId = 56;  // int | 

            try
            {
                Dictionary<string, SmV2TableGroup> result = apiInstance.ApiV2LeaguesLeagueIdGroupedTableJsonGet(leagueId);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SaisonManagerApi.ApiV2LeaguesLeagueIdGroupedTableJsonGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the ApiV2LeaguesLeagueIdGroupedTableJsonGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<Dictionary<string, SmV2TableGroup>> response = apiInstance.ApiV2LeaguesLeagueIdGroupedTableJsonGetWithHttpInfo(leagueId);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SaisonManagerApi.ApiV2LeaguesLeagueIdGroupedTableJsonGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **leagueId** | **int** |  |  |

### Return type

[**Dictionary&lt;string, SmV2TableGroup&gt;**](#smv2tablegroup)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="apiv2leaguesleagueidjsonget"></a>
# **ApiV2LeaguesLeagueIdJsonGet**
> SmLeagueResponse ApiV2LeaguesLeagueIdJsonGet (int leagueId)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using System.Net.Http;
using SaisonManager.Api.V2.Api;
using SaisonManager.Api.V2.Client;
using SaisonManager.Api.V2.Model;

namespace Example
{
    public class ApiV2LeaguesLeagueIdJsonGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://saisonmanager.de";
            // create instances of HttpClient, HttpClientHandler to be reused later with different Api classes
            HttpClient httpClient = new HttpClient();
            HttpClientHandler httpClientHandler = new HttpClientHandler();
            var apiInstance = new SaisonManagerApi(httpClient, config, httpClientHandler);
            var leagueId = 56;  // int | 

            try
            {
                SmLeagueResponse result = apiInstance.ApiV2LeaguesLeagueIdJsonGet(leagueId);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SaisonManagerApi.ApiV2LeaguesLeagueIdJsonGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the ApiV2LeaguesLeagueIdJsonGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<SmLeagueResponse> response = apiInstance.ApiV2LeaguesLeagueIdJsonGetWithHttpInfo(leagueId);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SaisonManagerApi.ApiV2LeaguesLeagueIdJsonGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **leagueId** | **int** |  |  |

### Return type

[**SmLeagueResponse**](#smleagueresponse)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="apiv2leaguesleagueidschedulejsonget"></a>
# **ApiV2LeaguesLeagueIdScheduleJsonGet**
> List&lt;SmV2ScheduledGame&gt; ApiV2LeaguesLeagueIdScheduleJsonGet (int leagueId)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using System.Net.Http;
using SaisonManager.Api.V2.Api;
using SaisonManager.Api.V2.Client;
using SaisonManager.Api.V2.Model;

namespace Example
{
    public class ApiV2LeaguesLeagueIdScheduleJsonGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://saisonmanager.de";
            // create instances of HttpClient, HttpClientHandler to be reused later with different Api classes
            HttpClient httpClient = new HttpClient();
            HttpClientHandler httpClientHandler = new HttpClientHandler();
            var apiInstance = new SaisonManagerApi(httpClient, config, httpClientHandler);
            var leagueId = 56;  // int | 

            try
            {
                List<SmV2ScheduledGame> result = apiInstance.ApiV2LeaguesLeagueIdScheduleJsonGet(leagueId);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SaisonManagerApi.ApiV2LeaguesLeagueIdScheduleJsonGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the ApiV2LeaguesLeagueIdScheduleJsonGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<List<SmV2ScheduledGame>> response = apiInstance.ApiV2LeaguesLeagueIdScheduleJsonGetWithHttpInfo(leagueId);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SaisonManagerApi.ApiV2LeaguesLeagueIdScheduleJsonGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **leagueId** | **int** |  |  |

### Return type

[**List&lt;SmV2ScheduledGame&gt;**](#smv2scheduledgame)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="apiv2leaguesleagueidscorerjsonget"></a>
# **ApiV2LeaguesLeagueIdScorerJsonGet**
> List&lt;SmV2ScorerPlayer&gt; ApiV2LeaguesLeagueIdScorerJsonGet (int leagueId)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using System.Net.Http;
using SaisonManager.Api.V2.Api;
using SaisonManager.Api.V2.Client;
using SaisonManager.Api.V2.Model;

namespace Example
{
    public class ApiV2LeaguesLeagueIdScorerJsonGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://saisonmanager.de";
            // create instances of HttpClient, HttpClientHandler to be reused later with different Api classes
            HttpClient httpClient = new HttpClient();
            HttpClientHandler httpClientHandler = new HttpClientHandler();
            var apiInstance = new SaisonManagerApi(httpClient, config, httpClientHandler);
            var leagueId = 56;  // int | 

            try
            {
                List<SmV2ScorerPlayer> result = apiInstance.ApiV2LeaguesLeagueIdScorerJsonGet(leagueId);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SaisonManagerApi.ApiV2LeaguesLeagueIdScorerJsonGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the ApiV2LeaguesLeagueIdScorerJsonGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<List<SmV2ScorerPlayer>> response = apiInstance.ApiV2LeaguesLeagueIdScorerJsonGetWithHttpInfo(leagueId);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SaisonManagerApi.ApiV2LeaguesLeagueIdScorerJsonGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **leagueId** | **int** |  |  |

### Return type

[**List&lt;SmV2ScorerPlayer&gt;**](#smv2scorerplayer)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="apiv2leaguesleagueidtablejsonget"></a>
# **ApiV2LeaguesLeagueIdTableJsonGet**
> List&lt;SmV2TableTeam&gt; ApiV2LeaguesLeagueIdTableJsonGet (int leagueId)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using System.Net.Http;
using SaisonManager.Api.V2.Api;
using SaisonManager.Api.V2.Client;
using SaisonManager.Api.V2.Model;

namespace Example
{
    public class ApiV2LeaguesLeagueIdTableJsonGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://saisonmanager.de";
            // create instances of HttpClient, HttpClientHandler to be reused later with different Api classes
            HttpClient httpClient = new HttpClient();
            HttpClientHandler httpClientHandler = new HttpClientHandler();
            var apiInstance = new SaisonManagerApi(httpClient, config, httpClientHandler);
            var leagueId = 56;  // int | 

            try
            {
                List<SmV2TableTeam> result = apiInstance.ApiV2LeaguesLeagueIdTableJsonGet(leagueId);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SaisonManagerApi.ApiV2LeaguesLeagueIdTableJsonGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the ApiV2LeaguesLeagueIdTableJsonGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<List<SmV2TableTeam>> response = apiInstance.ApiV2LeaguesLeagueIdTableJsonGetWithHttpInfo(leagueId);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SaisonManagerApi.ApiV2LeaguesLeagueIdTableJsonGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **leagueId** | **int** |  |  |

### Return type

[**List&lt;SmV2TableTeam&gt;**](#smv2tableteam)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="apiv2penaltiesjsonget"></a>
# **ApiV2PenaltiesJsonGet**
> List&lt;SmV2Penalty&gt; ApiV2PenaltiesJsonGet ()



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using System.Net.Http;
using SaisonManager.Api.V2.Api;
using SaisonManager.Api.V2.Client;
using SaisonManager.Api.V2.Model;

namespace Example
{
    public class ApiV2PenaltiesJsonGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://saisonmanager.de";
            // create instances of HttpClient, HttpClientHandler to be reused later with different Api classes
            HttpClient httpClient = new HttpClient();
            HttpClientHandler httpClientHandler = new HttpClientHandler();
            var apiInstance = new SaisonManagerApi(httpClient, config, httpClientHandler);

            try
            {
                List<SmV2Penalty> result = apiInstance.ApiV2PenaltiesJsonGet();
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SaisonManagerApi.ApiV2PenaltiesJsonGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the ApiV2PenaltiesJsonGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<List<SmV2Penalty>> response = apiInstance.ApiV2PenaltiesJsonGetWithHttpInfo();
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SaisonManagerApi.ApiV2PenaltiesJsonGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters
This endpoint does not need any parameter.
### Return type

[**List&lt;SmV2Penalty&gt;**](#smv2penalty)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="apiv2penaltycodesjsonget"></a>
# **ApiV2PenaltyCodesJsonGet**
> List&lt;SmV2PenaltyCode&gt; ApiV2PenaltyCodesJsonGet ()



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using System.Net.Http;
using SaisonManager.Api.V2.Api;
using SaisonManager.Api.V2.Client;
using SaisonManager.Api.V2.Model;

namespace Example
{
    public class ApiV2PenaltyCodesJsonGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://saisonmanager.de";
            // create instances of HttpClient, HttpClientHandler to be reused later with different Api classes
            HttpClient httpClient = new HttpClient();
            HttpClientHandler httpClientHandler = new HttpClientHandler();
            var apiInstance = new SaisonManagerApi(httpClient, config, httpClientHandler);

            try
            {
                List<SmV2PenaltyCode> result = apiInstance.ApiV2PenaltyCodesJsonGet();
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SaisonManagerApi.ApiV2PenaltyCodesJsonGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the ApiV2PenaltyCodesJsonGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<List<SmV2PenaltyCode>> response = apiInstance.ApiV2PenaltyCodesJsonGetWithHttpInfo();
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SaisonManagerApi.ApiV2PenaltyCodesJsonGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters
This endpoint does not need any parameter.
### Return type

[**List&lt;SmV2PenaltyCode&gt;**](#smv2penaltycode)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

