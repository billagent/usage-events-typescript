# UsageEventsAgainApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**usageTermMatcherServiceIntakeUsageEvent**](#usagetermmatcherserviceintakeusageevent) | **POST** /product/usage-intake | Process a usage event|

# **usageTermMatcherServiceIntakeUsageEvent**
> V1IntakeUsageEventResponse usageTermMatcherServiceIntakeUsageEvent(body)

Matches usage events to contract terms and returns event price and matched term metadata.

### Example

```typescript
import {
    UsageEventsAgainApi,
    Configuration,
    V1IntakeUsageEventRequest
} from '@billagent/usage-events';

const configuration = new Configuration();
const apiInstance = new UsageEventsAgainApi(configuration);

let body: V1IntakeUsageEventRequest; //

const { status, data } = await apiInstance.usageTermMatcherServiceIntakeUsageEvent(
    body
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **body** | **V1IntakeUsageEventRequest**|  | |


### Return type

**V1IntakeUsageEventResponse**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | A successful response. |  -  |
|**0** | An unexpected error response. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

